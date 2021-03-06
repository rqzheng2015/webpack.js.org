---
title: raw-loader
source: https://raw.githubusercontent.com/webpack/raw-loader/master/README.md
edit: https://github.com/webpack/raw-loader/edit/master/README.md
---
## Install

```bash
npm install --save-dev raw-loader
```

## Usage

Use the loader either via your webpack config, CLI or inline.

### Via webpack config (recommended)

**webpack.config.js**
```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.txt$/,
        use: 'raw-loader'
      }
    ]
  }
}
```

**In your application**
```js
import txt from 'file.txt';
```

### CLI

```bash
webpack --module-bind 'txt=raw-loader'
```

**In your application**
```js
import txt from 'file.txt';
```

### Inline

**In your application**
```js
import txt from 'raw-loader!./file.txt';
```

## Maintainers

<table>
  <tbody>
    <tr>
      <td align="center">
        <img width="150 height="150" src="https://github.com/sokra.png?s=150">
        <br>
        <a href="https://github.com/sokra">Tobias Koppers</a>
      </td>
    <tr>
  <tbody>
</table>

[npm]: https://img.shields.io/npm/v/raw-loader.svg
[npm-url]: https://npmjs.com/package/raw-loader

[node]: https://img.shields.io/node/v/raw-loader.svg
[node-url]: https://nodejs.org

[deps]: https://david-dm.org/webpack/raw-loader.svg
[deps-url]: https://david-dm.org/webpack/raw-loader

[tests]: http://img.shields.io/travis/webpack/raw-loader.svg
[tests-url]: https://travis-ci.org/webpack/raw-loader

[cover]: https://coveralls.io/repos/github/webpack/raw-loader/badge.svg
[cover-url]: https://coveralls.io/github/webpack/raw-loader

[chat]: https://badges.gitter.im/webpack/webpack.svg
[chat-url]: https://gitter.im/webpack/webpack

***

> 原文：https://webpack.js.org/loaders/raw-loader/