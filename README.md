# svelte-scroll-infinite
[![NPM version](https://img.shields.io/npm/v/svelte-viewpoint.svg?style=flat)](https://www.npmjs.com/package/svelte-scroll-infinite)

[Demo REPL](https://svelte.dev/repl/22e1305dea994aafac795c8e3d74b79c?version=3.19.1)

## Install

```bash
npm i svelte-inline-edit --save-dev
```

## Props

| Name | Type | Description | Required | Default |
| --- | --- | --- | --- | --- |
| `hasMore` | `bool` | Indicator if there are any items to load | No | true |
| `threshold` | `number` | Threshold to call loadMore | No | 100 |

## Events

- `loadMore` - Call with offset
