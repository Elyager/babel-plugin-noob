# babel-plugin-noob

My first babel plugin.

## Example

**In**

```js
// input code
```

**Out**

```js
"use strict";

// output code
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
require("babel-core").transform("code", {
  plugins: ["noob"]
});
```
