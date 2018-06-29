# nuxt-nest-boilerplate

> A nuxt.js project boiletplate for NestHQ

- Generic router example in `components/Nav.vue`
- Generic layout example in `layouts`
- Generic page structure in `pages`
- Generic config examples in `nuxt.config.js`
	- node-sass / sass-loader pulling in one scss file / compiles through nuxt / webpack
	- Google font loading
	- SEO title templating
	- Router active state optimised
- Kind skeleton / boilerplate styles loaded in (design tokens not yet working, precompiled sass-maps used)
- async data example in `music/index.vue` / `music/_id.vue`
	- Taken from example [here](https://nuxtjs.org/examples/async-data)

## @TODO / Untested
- Theo design tokens
- Fractal side by side
- CMS / database side by side
- Graphql integration examples

## Build Setup

``` bash
# install dependencies
$ yarn

# serve with hot reload at localhost:3000
$ yarn run dev

# build for production and launch server
$ yarn run build
$ yarn start

# generate static project
$ yarn run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).
