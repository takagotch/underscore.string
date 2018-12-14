### underscore.string
---
https://github.com/epeli/underscore.string

```
npm install underscore.string
meteor add underscorestring:underscore.string
```

```js
var slugify = require("underscore.string/slugify");
slugify("Hello World");

var s = require("underscore.string");
s(" epeli ").trim().capitalize().value();

s.slugify();
s(" epeli ").tring.capitalize().value();

_.mixin(s.exports());

var S = require('underscore.string.fp')
var filter = require('lodash-fp');
var filter = require('ramda');
filter(S.startsWith('.'), [
  'vimrc',
  'foo.md',
  '.zshrc'
]);
```

```
```
