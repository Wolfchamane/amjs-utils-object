# @amjs/utils 0.1.0

![Statements](https://img.shields.io/badge/Statements-100%25-brightgreen.svg) ![Branches](https://img.shields.io/badge/Branches-100%25-brightgreen.svg) ![Functions](https://img.shields.io/badge/Functions-100%25-brightgreen.svg) ![Lines](https://img.shields.io/badge/Lines-100%25-brightgreen.svg)

> Set of tools as dotProp, etc.

## Installation

```bash
$ npm i @amjs/utils-object
```
## Usage

#### dotProp

```javascript
const { dotProp } = require('@amjs/utils-object');

const context = {
    key : {
        value : 'value'
    }
};

// Interface: dotProp(ref = {}, prop = '', value = '')
// Use two arguments in order to return a value
console.log(dotProp(context, 'key.value')); // 'value'
// Use additional 3rd argument to assign new value
dotProp(context, 'key.value', 'foo');
console.log(dotProp(context, 'key.value')); // 'foo'
```
