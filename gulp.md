


setup
=====


install
-------

```
npm install -g gulp
```


project
-------

* `gulp` has developer dependancies that needs to be setup on a per project basis
* [Linux - No local gulp install found even after installing npm install -g gulp - Stack Overflow](http://stackoverflow.com/questions/23284805/no-local-gulp-install-found-even-after-installing-npm-install-g-gulp)
```
npm install --save-dev gulp
```



concat
======

setup
-----

### install ###

```
npm install -g gulp-concat
```

### project ###

* `gulp-concat` has developer dependancies that needs to be setup on a per project basis

```
npm install --save-dev gulp-concat
```


minimal config
--------------


* [Introduction to Gulp.js with practical examples | Julien Renaux Blog](https://julienrenaux.fr/2014/05/25/introduction-to-gulp-js-with-practical-examples/)

create a file `gulpfile.js`:
```
// plugins
var gulp = require("gulp")
var concat = require("gulp-concat");

// paths to files
const node_modules = [
    "./node_modules/jquery/dist/jquery.min.js",
];

gulp.task('concat', function () {
    gulp.src(node_modules) //
        .pipe(concat('node_modules.js'))  // concat and name it "node_modules.js"
        .pipe(gulp.dest('gulp')); // in the folder 'gulp'
});
```




