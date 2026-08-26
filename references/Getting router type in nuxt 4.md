---
title: "Getting router type in nuxt 4"
summary:
date: "2026-08-26"
tags:
draft: true
---
# Syntax
Enable experimental option for `typedPages` in nuxt config:
```ts
// nuxt.config.ts
export default defineNuxtConfig({
  experimental: {
    typedPages: true,
  },
})
```

# Examples
After toggling experimental `typedPages` on, now you can have autocompletion on your IDE.

```vue
<script setup lang="ts">
const router = useRoute()
</script>

<template>
 <button @click="router.push('/about')">
 To about page
 </button>
</template>
```

Or you can expose a type that contains all of your route paths.
```ts
export type RoutePath = RouteNameMap[keyof RouteNameMap]['path']

// same as
type RoutePath = keyof typeof Router[number]
```
# Gotchas

# Links
https://nuxt.com/docs/4.x/guide/going-further/experimental-features#typedpages