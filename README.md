# babel-plugin-noob

My first babel plugin.

> Strip `console`, `alert`, and `debugger` statements from JavaScript code

Useful for making sure you didn't leave any logging in production code.

## Example

**In**

```js
function hey() {
  debugger
}
```

**Out**

```js
function hey() {}
```

## Installation

```sh
$ npm install babel-plugin-noob
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["noob"]
}
```

### Via CLI

```sh
$ babel --plugins noob script.js
```

### Via Node API

```javascript
require('babel-core').transform('code', {
  plugins: ['noob'],
})
```
