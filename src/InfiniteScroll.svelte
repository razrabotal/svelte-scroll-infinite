<script>
  import { onMount, createEventDispatcher } from "svelte";
  export let threshold = 100;
  export let hasMore = true;
  const dispatch = createEventDispatcher();

  let component;
  let observer = new IntersectionObserver(observerCallback);

  function observerCallback(entries, observer) {
    entries.forEach(entry => {
      if (entry.isIntersecting && hasMore) {
        dispatch("loadMore");
      }
    });
  }

  $: hasMore || observer.unobserve(component);

  onMount(() => {
    observer.observe(component);
    return () => observer.unobserve(component);
  });
</script>

<div
  bind:this={component}
  style="width:0px; position: relative; top: -{threshold}px;" />
