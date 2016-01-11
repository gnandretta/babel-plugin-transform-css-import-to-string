# babel-plugin-transform-css-import-to-string

Turn CSS imports into strings.

## Example

Given the following _style.css_.

```css
body { background-color: red; }
```

#### in

```js
import css from './style.css';
```

#### out

```js
var css = 'body{background-color:red;}';
```


## Installation

```sh
$ npm install babel-plugin-transform-css-import-to-string
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-css-import-to-string"]
}
```

### Via CLI

```sh
$ babel --plugins transform-css-import-to-string script.js
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["transform-css-import-to-string"]
});
```
