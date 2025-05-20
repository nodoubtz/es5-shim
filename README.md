# es5-shim

A compatibility library that implements ECMAScript 5 (ES5) features for older JavaScript engines. This project ensures that legacy environments can use modern JavaScript methods and objects, increasing cross-browser and cross-platform compatibility for your web projects.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Contributing](#contributing)
- [License](#license)

## Overview

**es5-shim** provides polyfills for ES5 features that may not be natively supported in older browsers or JavaScript engines. This includes array methods, object methods, and other language enhancements introduced in ES5.

**Why use es5-shim?**
- Legacy browser support (IE8, old Android, etc.)
- Ensures consistent behavior across environments
- Simple to include and use

## Features

- Polyfills for ES5 methods such as:
  - `Array.prototype.forEach`, `map`, `filter`, `reduce`, etc.
  - `Object.create`, `Object.keys`, `Object.getOwnPropertyDescriptor`, etc.
  - `Date.now`, `Function.prototype.bind`
  - And many more

- Lightweight, modular codebase
- Safe: does not overwrite native implementations if they exist

## Installation

### npm

```sh
npm install es5-shim
```

### CDN

You can include the shim directly from a CDN:

```html
<script src="https://unpkg.com/es5-shim/es5-shim.min.js"></script>
```

### Manual

Download `es5-shim.min.js` from the [releases](https://github.com/nodoubtz/es5-shim/releases) or clone the repo and include the script in your project.

## Usage

Simply include the shim **before** your JavaScript code that relies on ES5 features.

```html
<script src="path/to/es5-shim.min.js"></script>
<script>
  // Your code using ES5 features
  var arr = [1, 2, 3];
  arr.forEach(function(item) {
    console.log(item);
  });
</script>
```

## API

es5-shim patches global objects and prototypes with missing ES5 features. No explicit API is needed. For details on which methods are polyfilled, see the [MDN ES5 documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) or review the source code.

## Contributing

Contributions are welcome! To contribute:

1. Fork this repository
2. Create a new branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a pull request

Please ensure your code follows the existing style and passes all tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Maintained by [nodoubtz](https://github.com/nodoubtz).**
