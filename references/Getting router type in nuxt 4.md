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

```
```

# Gotchas

# Links
https://nuxt.com/docs/4.x/guide/going-further/experimental-features#typedpages