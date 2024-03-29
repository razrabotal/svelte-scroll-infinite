# Svelte Infinite Scroll
[![NPM version](https://img.shields.io/npm/v/svelte-viewpoint.svg?style=flat)](https://www.npmjs.com/package/svelte-scroll-infinite)

[Demo REPL](https://svelte.dev/repl/528e077fda1a4c95bfed72e76036e599?version=4.1.1)

## Install

```bash
npm i svelte-scroll-infinite --save-dev
```

## Props

| Name | Type | Description | Required | Default |
| --- | --- | --- | --- | --- |
| `hasMore` | `bool` | Indicator if there are any items to load | No | true |
| `threshold` | `number` | Threshold to call loadMore | No | 100 |

## Events

- `loadMore` - Call with offset

## Warning  
> ⚠️You also want to add the [intersection-observer](https://www.npmjs.com/package/intersection-observer) polyfill for full browser support.

## License

MIT &copy; [Taras Gordienko](https://github.com/razrabotal)
