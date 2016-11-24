# tiny.pictures-sdk-js  [![Build Status](https://travis-ci.org/erkstruwe/tiny.pictures-sdk-js.svg?branch=master)](https://travis-ci.org/erkstruwe/tiny.pictures-sdk-js) [![Coverage Status](https://coveralls.io/repos/github/erkstruwe/tiny.pictures-sdk-js/badge.svg?branch=master)](https://coveralls.io/github/erkstruwe/tiny.pictures-sdk-js?branch=master)
JavaScript SDK for [tiny.pictures](https://tiny.pictures/)

## Functions and demo
* Automatic srcset calculation for responsive images
* Lazy loading

Visit https://tiny.pictures/js-sdk for demos and details.

## Browser
### Installation
Use our CDN for a fast-loading and always up-to-date library.
```
  ...
  <script src="https://tiny.pictures/tiny.pictures.min.js">
</body>
</html>
```
### Usage
All functions are available in the global `tiny.pictures` object.
#### Example
```
tiny.pictures.url('http://your.domain/path/to/image.jpg', {width: 200})
// 'https://tiny.pictures/api/path/to/image.jpg?protocol=http&hostname=your.domain&width=200'
```

## NodeJS
### Installation
```
npm install tiny.pictures-sdk-js
```
### Usage
Just `require` the package.
#### Example
```
var tinyPictures = require('tiny.pictures-sdk-js')
tinyPictures.url('http://your.domain/path/to/image.jpg', {width: 200})
// 'https://tiny.pictures/api/path/to/image.jpg?protocol=http&hostname=your.domain&width=200'
```
