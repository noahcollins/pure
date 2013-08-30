UI Example 1
====

A simple project that represents an email client. Based primarily on Yahoo's Pure CSS modules.


Notes
--------

* A basic responsive grid.

* Built on Normalize.css to level common cross-browser issues.

* Extremely small production CSS file size: 4.3KB minified + gzipped.

* There are some non-abstracted classes. I use LESS mixins to keep production CSS lean & semantic while retaining source generality. Not used in this example.


Build
-----------------

```shell
$ git clone https://github.com/noahcollins/pure.git
$ cd pure
$ npm install
$ grunt
```

### View the Example

Open `dist/index.html` to view.

### Build Files

Grunt will put the built CSS modules into the `pure/build/` directory. The naming
conventions of the files in the `build/` directory follow these rules:

* `[module]-core.css`: The minimal set of styles, ususally structural, that
  provide the base on which the rest of the module's styles build.

* `[module]-nr.css`: Rollup of `[module]-core.css` + `[module].css` +
  `[module]-[feature].css` from the `src/[module]/` dir. This is the
  non-responsive version of a module.

* `[module].css`: Rollup of `[module]-nr.css` + `[module]-r.css` from the
  `build/` dir. This is the responsive version of a module.

* `pure.css`: A rollup of all `[module].css` files in the `build/` dir. This is
  a responsive roll-up of everything, non-minified.

* `pure-min.css`: Minified version of `pure.css` that should be used in
  production.


Browser Support and Testing
---------------------------

* IE 7+
* Latest Stable: Firefox, Chrome, Safari
* iOS 6.x
* Android 4.x


License
-------

This software is free to use under the Yahoo! Inc. BSD license.
See the [LICENSE file][] for license text and copyright information.


[LICENSE file]: https://github.com/yui/pure/blob/master/LICENSE.md
