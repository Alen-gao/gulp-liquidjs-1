Gulp Liquid
===========
Liquid plugin for gulp

Installation
------------

```git
npm install --save-dev gulp-liquidjs
```

Usage
-----
gulpfile.js:
```js
const gulp = require('gulp');
const liquid = require('gulp-liquidjs');

gulp.src("./src/*.liquid")
    .pipe(liquid())
    .pipe(gulp.dest("./dist"));
```

API
---
#### liquid(options)

* **options.data** - ***{Object}*** - The locals object is passed as template variables to the liquid templating engine.
* **options.tags** - ***{Object}*** - Custom tags. See [registration-of-new-tags](https://www.npmjs.com/package/liquid-node#registration-of-new-tags)
* **options.filters** - ***{Object}*** - Custom filters. See [registration-of-new-filters](https://www.npmjs.com/package/liquid-node#registration-of-new-filters)

