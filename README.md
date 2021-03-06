# cache-it [![Build Status](https://travis-ci.org/reinaldo13/cache-it.svg?branch=master)](https://travis-ci.org/reinaldo13/cache-it)
Because caching should be simple! A Javascript cache helper object. Supports in-memory and local storage caching as well as cache expiration.

## Installation
```shell
npm install cache-it --save
```

## Constructor Parameters:
- type: 'MEMORY' for memory cache or 'LOCAL' for html5 local storage (compatible with I8+)
- name: namespace for the cache's instance
- expiry: amount of seconds that the cache will be valid for

## Usage
```javascript
var CacheIt = require('cache-it');
var cache = new CacheIt('MEMORY', 'usersStore', 180);
cache.put('myKey', 'myValue');
var value = cache.get('myKey');
console.log(value);
```

## Tests
```shell
npm test
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style.
Add unit tests for any new or changed functionality. Lint and test your code.

## Release History
* 1.0.0 Initial release
