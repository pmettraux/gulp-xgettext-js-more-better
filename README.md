# [gulp](http://gulpjs.com)-xgettext-js-more-better

> Extract translatable strings using [xgettext-js-more-better](https://www.npmjs.com/package/xgettext-js-more-better)

## Install

Install with [npm](https://npmjs.org/package/gulp-xgettext-js-more-better)

```sh
npm install --save-dev gulp-xgettext-js-more-better
```

## Example

```js
var gulp = require('gulp');
var xgettext = require('gulp-xgettext-js-more-better');

gulp.task('pot', function () {
    return gulp.src(['src/**/*.js'])
        .pipe(xgettext({
            // options to pass to xgettext-js-more-better...
        }))
        .pipe(gulp.dest('po/'));
});
```
