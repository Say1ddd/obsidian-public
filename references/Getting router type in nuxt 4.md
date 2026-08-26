---
title: "Getting router type in nuxt 4"
summary:
date: "2026-08-26"
tags:
draft: true
---
> This option is enabled automatically in the upcoming `compatibilityVersion: 5` (Nuxt 5) as stated in ![Nuxt's official documentation](https://nuxt.com/docs/4.x/getting-started/upgrade#typed-pages-enabled-by-default)

# Syntax
Enable experimental option for `typedPages` in your Nuxt config:
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
type NuxttePath = keyof typeof Router[number]
```
# Gotchas

# Links
https://nuxt.com/docs/4.x/guide/going-further/experimental-features#typedpages