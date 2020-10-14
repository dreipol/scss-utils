# scss-utils

<img src="https://raw.githubusercontent.com/dreipol/scss-utils/master/logo.jpg" width="50%"/>

dreipol scss util @functions and @mixins


[![Build Status][travis-image]][travis-url]
[![NPM version][npm-version-image]][npm-url]
[![NPM downloads][npm-downloads-image]][npm-url]
[![MIT License][license-image]][license-url]

# Installation

```bash
npm i @dreipol/scss-utils -S
```

# Documentation 

These utils are built as sass modules. You can import them in your sass files simply using the `@use` rule for example:

```scss
@use 'node_modules/@dreipol/scss-utils/mixins/has-focus' as *;

a {
    @include has-focus {
        color: red;
    }
} 
```

Notice that you can import all the mixins or functions namespacing them for example:

```scss
// all utils
@use 'node_modules/@dreipol/scss-utils' as utils;
// or also only mixins
@use 'node_modules/@dreipol/scss-utils/mixins' as mixins;

a {
    @include utils.has-focus {
        color: red;
    }
} 

.hidden {
    @include mixins.hide-visually;
} 
```

## API

The of all the exported modules is online available https://www.dreipol.dev/scss-utils/


[travis-image]:https://img.shields.io/travis/dreipol/scss-utils.svg?style=flat-square
[travis-url]:https://travis-ci.org/dreipol/scss-utils

[license-image]:http://img.shields.io/badge/license-MIT-000000.svg?style=flat-square
[license-url]:LICENSE

[npm-version-image]:http://img.shields.io/npm/v/@dreipol/scss-utils.svg?style=flat-square
[npm-downloads-image]:http://img.shields.io/npm/dm/@dreipol/scss-utils.svg?style=flat-square
[npm-url]:https://npmjs.org/package/@dreipol/scss-utils
