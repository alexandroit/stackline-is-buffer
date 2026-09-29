# @stackline/is-buffer

> Determine if an object is a Buffer.

[![npm version](https://img.shields.io/npm/v/@stackline/is-buffer.svg?style=flat-square)](https://www.npmjs.com/package/@stackline/is-buffer)
[![license](https://img.shields.io/npm/l/@stackline/is-buffer.svg?style=flat-square)](https://github.com/alexandroit/stackline-is-buffer)
[![GitHub repository](https://img.shields.io/badge/GitHub-repository-181717?style=flat-square&logo=github)](https://github.com/alexandroit/stackline-is-buffer)
[![Docs](https://img.shields.io/badge/docs-alexandro.net-0f766e?style=flat-square)](https://alexandro.net/docs/vanilla/is-buffer/)
[![Reddit community](https://img.shields.io/badge/community-r%2FStackline-ff4500?style=flat-square&logo=reddit&logoColor=white)](https://www.reddit.com/r/Stackline/)

**[Documentation](https://alexandro.net/docs/vanilla/is-buffer/)** | **[npm](https://www.npmjs.com/package/@stackline/is-buffer)** | **[Issues](https://github.com/alexandroit/stackline-is-buffer/issues)** | **[Repository](https://github.com/alexandroit/stackline-is-buffer)**

**Current package version:** `1.0.2`

---

## Why this package?

`@stackline/is-buffer` is the Stackline-maintained distribution of `is-buffer@2.0.5`. It is an independent continuation of [is-buffer](https://github.com/feross/is-buffer); original authors and licenses remain credited below.

## Compatibility

| Item | Value |
| :--- | :--- |
| Package | `@stackline/is-buffer@1.0.2` |
| API target | `is-buffer@2.0.5` |
| Supported Node.js | `>=4` |
| License | `MIT` |
| Main entry | `index.js` |
| Runtime dependencies | `none` |

## Installation

```bash
npm install @stackline/is-buffer
```

Preserve existing imports and plugin resolution with an npm alias:

```bash
npm install is-buffer@npm:@stackline/is-buffer
```

## Usage and API reference

### is-buffer [![travis][travis-image]][travis-url] [![npm][npm-image]][npm-url] [![downloads][downloads-image]][downloads-url] [![javascript style guide][standard-image]][standard-url]

[travis-image]: https://img.shields.io/travis/feross/is-buffer/master.svg
[travis-url]: https://travis-ci.org/feross/is-buffer
[npm-image]: https://img.shields.io/npm/v/is-buffer.svg
[npm-url]: https://npmjs.org/package/is-buffer
[downloads-image]: https://img.shields.io/npm/dm/is-buffer.svg
[downloads-url]: https://npmjs.org/package/is-buffer
[standard-image]: https://img.shields.io/badge/code_style-standard-brightgreen.svg
[standard-url]: https://standardjs.com

#### Determine if an object is a [`Buffer`](http://nodejs.org/api/buffer.html) (including the [browserify Buffer](https://github.com/feross/buffer))


[saucelabs-image]: https://saucelabs.com/browser-matrix/is-buffer.svg
[saucelabs-url]: https://saucelabs.com/u/is-buffer

## Why not use `Buffer.isBuffer`?

This module lets you check if an object is a `Buffer` without using `Buffer.isBuffer` (which includes the whole [buffer](https://github.com/feross/buffer) module in [browserify](http://browserify.org/)).

It's future-proof and works in node too!

## install

```bash
npm install @stackline/is-buffer
```

## usage

```js
var isBuffer = require('@stackline/is-buffer')

isBuffer(new Buffer(4)) // true
isBuffer(Buffer.alloc(4)) //true

isBuffer(undefined) // false
isBuffer(null) // false
isBuffer('') // false
isBuffer(true) // false
isBuffer(false) // false
isBuffer(0) // false
isBuffer(1) // false
isBuffer(1.0) // false
isBuffer('string') // false
isBuffer({}) // false
isBuffer(function foo () {}) // false
```

## license

MIT. Copyright (C) [Feross Aboukhadijeh](http://feross.org).

## Credits and original authors

- Original project: [is-buffer](https://github.com/feross/is-buffer).
- Feross Aboukhadijeh.
- Stackline maintenance: [Alexandro Paixao Marques](https://www.linkedin.com/in/aleinfo/) and [Stackline contributors](https://github.com/alexandroit).

Original copyright, license notices and contributor acknowledgements remain part of this distribution. Stackline maintenance does not replace authorship of the original work.

## License

`MIT`. See the license and notice files in the [repository](https://github.com/alexandroit/stackline-is-buffer).

## Community and Links

- [Stackline website](https://alexandro.net/)
- [GitHub projects](https://github.com/alexandroit)
- [npm packages](https://www.npmjs.com/~alex360qc)
- [Reddit community — r/Stackline](https://www.reddit.com/r/Stackline/)
- [Maintainer LinkedIn](https://www.linkedin.com/in/aleinfo/)

Use this repository's issue tracker for reproducible bugs and feature requests. Join r/Stackline for examples, usage questions and release discussions.
