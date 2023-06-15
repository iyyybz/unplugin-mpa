# unplugin-mpa

unplugin multi pages mpa

[![NPM version](https://img.shields.io/npm/v/unplugin-mpa?color=a1b858&label=)](https://www.npmjs.com/package/unplugin-mpa)

## Install

```bash
npm i unplugin-mpa
```

<details>
<summary>Vite</summary><br>

```ts
// vite.config.ts
import Mock from 'unplugin-mpa/vite'

export default defineConfig({
  plugins: [
    Mock({
      /* options */
    }),
  ],
})
```

Example: [`playground/`](./playground/)

<br></details>

<details>
<summary>Rollup</summary><br>

```ts
// rollup.config.js
import Mock from 'unplugin-mpa/rollup'

export default {
  plugins: [
    Mock({
      /* options */
    }),
  ],
}
```

<br></details>

<details>
<summary>Webpack</summary><br>

```ts
// webpack.config.js
module.exports = {
  /* ... */
  plugins: [
    require('unplugin-mpa/webpack')({
      /* options */
    }),
  ],
}
```

<br></details>

<details>
<summary>Nuxt</summary><br>

```ts
// nuxt.config.js
export default {
  buildModules: [
    [
      'unplugin-mpa/nuxt',
      {
        /* options */
      },
    ],
  ],
}
```

> This module works for both Nuxt 2 and [Nuxt Vite](https://github.com/nuxt/vite)

<br></details>

<details>
<summary>Vue CLI</summary><br>

```ts
// vue.config.js
module.exports = {
  configureWebpack: {
    plugins: [
      require('unplugin-mpa/webpack')({
        /* options */
      }),
    ],
  },
}
```

<br></details>

<details>
<summary>esbuild</summary><br>

```ts
// esbuild.config.js
import { build } from 'esbuild'
import Mock from 'unplugin-mpa/esbuild'

build({
  plugins: [Mock()],
})
```

<br></details>

## Guide

To test plugin, run: `pnpm run dev`
To release a new version, run: `pnpm run release`


