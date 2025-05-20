# es5-shim

[![Build Status](https://img.shields.io/github/actions/workflow/status/nodoubtz/es5-shim/ci.yml?branch=Main)](https://github.com/nodoubtz/es5-shim/actions)
[![License](https://img.shields.io/github/license/nodoubtz/es5-shim)](LICENSE)

A robust JavaScript shim that provides compatibility for ECMAScript 5 features on legacy JavaScript engines.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

**es5-shim** ensures ECMAScript 5 methods are available in older JavaScript environments. It allows developers to write modern JavaScript code that runs reliably across old browsers and JavaScript engines that do not natively support ES5.

## Features

- Adds missing ES5 methods to built-in objects (`Array`, `Object`, `Function`, `Date`, etc.)
- Non-destructive: does not overwrite existing native implementations
- Lightweight and easy to use
- Broad browser compatibility, including IE6+
- Secure and robust implementation

## Installation

You can include **es5-shim** in your project via several methods:

### npm

```bash
npm install es5-shim
```

### CDN

```html
<script src="https://cdn.jsdelivr.net/npm/es5-shim/es5-shim.min.js"></script>
```

### Manual

Download the [latest release](https://github.com/nodoubtz/es5-shim/releases) and include `es5-shim.js` in your project.

## Usage

Simply include the shim at the top of your JavaScript bundle or HTML page:

```html
<script src="es5-shim.js"></script>
<script>
  // Your ES5 code here
</script>
```

**Node.js:**

```javascript
require('es5-shim');
// Your ES5 code here
```

## API

es5-shim polyfills the following ES5 features (not exhaustive):

- `Array.prototype.forEach`, `map`, `filter`, `reduce`, `some`, `every`
- `Object.create`, `Object.keys`, `Object.getPrototypeOf`, `Object.defineProperty`, etc.
- `Function.prototype.bind`
- `Date.now`
- And more

See [MDN ES5 Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference) for details.

## Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
2. Create your branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a new Pull Request

Please ensure code quality and security. Help us keep the shim robust!

## License

This project is licensed under the [MIT License](LICENSE).

---

**Author:** [nodoubtz](https://github.com/nodoubtz)

For questions or support, please open an [issue](https://github.com/nodoubtz/es5-shim/issues).
