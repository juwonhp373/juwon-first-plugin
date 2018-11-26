# JuwonFirstPlugin

[![npm](https://img.shields.io/npm/v/juwon-first-plugin.svg)](https://www.npmjs.com/package/juwon-first-plugin) [![vue2](https://img.shields.io/badge/vue-2.x-brightgreen.svg)](https://vuejs.org/)

> A Vue.js Plugin

## Installation

```bash
npm install --save juwon-first-plugin
```

## Usage

### Bundler (Webpack, Rollup)

```js
import Vue from 'vue'
import JuwonFirstPlugin from 'juwon-first-plugin'
// You need a specific loader for CSS files like https://github.com/webpack/css-loader
import 'juwon-first-plugin/dist/juwon-first-plugin.css'

Vue.use(JuwonFirstPlugin)
```

### Browser

```html
<!-- Include after Vue -->
<!-- Local files -->
<link rel="stylesheet" href="juwon-first-plugin/dist/juwon-first-plugin.css"></link>
<script src="juwon-first-plugin/dist/juwon-first-plugin.js"></script>

<!-- From CDN -->
<link rel="stylesheet" href="https://unpkg.com/juwon-first-plugin/dist/juwon-first-plugin.css"></link>
<script src="https://unpkg.com/juwon-first-plugin"></script>
```

## Development

### Launch visual tests

```bash
npm run dev
```

### Launch Karma with coverage

```bash
npm run dev:coverage
```

### Build

Bundle the js and css of to the `dist` folder:

```bash
npm run build
```


## Publishing

The `prepublish` hook will ensure dist files are created before publishing. This
way you don't need to commit them in your repository.

```bash
# Bump the version first
# It'll also commit it and create a tag
npm version
# Push the bumped package and tags
git push --follow-tags
# Ship it 🚀
npm publish
```

## License

[MIT](http://opensource.org/licenses/MIT)
