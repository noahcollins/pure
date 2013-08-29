UI Example 1
====

This is a simple email client UI. Based primarily on Yahoo's Pure CSS modules.


Outline
--------

* A basic responsive grid.

* Built on Normalize.css to level most cross-browser issues.

* Consistently styled buttons that work with `<a>` and `<button>` elements.

* Responsive by default, with a non-responsive option.

* Extremely small production CSS file size: 4.3KB minified + gzipped.


Build
-----------------

```shell
$ git clone https://github.com/noahcollins/pure.git
$ cd pure
$ npm install
$ grunt
```

### Build Files

Grunt will put everything into the `pure/build/` directory. The naming
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
