babel-plugin-transform-es3-helper-modules
=====================================

Externalize references to helpers using [babel-helper-modules-es3](https://www.npmjs.com/package/babel-helper-modules-es3).

If you want to externalize builtins too via [core-js](https://www.npmjs.com/package/core-js)'s library, see the official plugin [babel-plugin-transform-runtime](https://www.npmjs.com/package/babel-plugin-transform-runtime).

## Installation

```sh
$ npm install babel-plugin-transform-es3-helper-modules babel-helper-modules-es3
```

## Usage

Remember to also install [babel-helper-modules-es3](https://www.npmjs.com/package/babel-helper-modules-es3). when using the transpiled code.

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-es3-helper-modules"]
}
```

### Via CLI

```sh
$ babel --plugins transform-es3-helper-modules script.js
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["transform-es3-helper-modules"]
});
```
