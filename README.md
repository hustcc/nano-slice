# nano-slice

> Nano version for slice of string and array, just like Python.

[![Build Status](https://travis-ci.org/NanoPackage/nano-slice.svg?branch=master)](https://travis-ci.org/NanoPackage/nano-slice) [![Coverage Status](https://coveralls.io/repos/github/NanoPackage/nano-slice/badge.svg?branch=master)](https://coveralls.io/github/NanoPackage/nano-slice?branch=master) [![npm](https://img.shields.io/npm/v/nano-slice.svg?style=flat-square)](https://www.npmjs.com/package/nano-slice) [![npm](https://img.shields.io/npm/dt/nano-slice.svg?style=flat-square)](https://www.npmjs.com/package/nano-slice) [![npm](https://img.shields.io/npm/l/nano-slice.svg?style=flat-square)](https://www.npmjs.com/package/nano-slice)


# 1. Install

> **npm install nano-slice**


```js
var slice = require('nano-slice');

//or

import slice from 'nano-slice';
```


# 2. Usage

There is only one API named `slice`.

```js
// for array
const arr = slice([1, '2', 3, '4', 5, '6', 7, '8', 9, '0']);

arr['2:5'];  		// [3, '4', 5]
arr[':-2'];  		// [1, '2', 3, '4', 5, '6', 7, '8']
arr['-2:'];  		// [9, '0']
arr['1:5:2'];  		// ['2', '4']
arr['5:1:-2'];  	// ['6', '4']

// for string
const str = slice('1234567890');
str['2:5'];  		// '345'
str[':-2'];  		// '12345678'
str['-2:'];  		// '90'
str['1:5:2'];  		// '24'
str['5:1:-2'];  	// '64'

```


# 3. Test

> npm install
> 
> npm test


# LICENSE

MIT@[hustcc](https://github.com/hustcc).
