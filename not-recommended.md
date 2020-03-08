# 💀 Legacy or not recommended tools

Tools that are deprecated, out of date, have better alternatives or have only niche uses.

## Compilers

- [**Bublé**](https://buble.surge.sh/) ([GitHub](https://github.com/bublejs/buble))
- [**Closure Compiler**](https://developers.google.com/closure/compiler) ([GitHub](https://github.com/google/closure-compiler))

## Zero-config presets

- [**Yeoman**](https://yeoman.io/) ([GitHub](https://github.com/yeoman/yeoman))
  - Generator; Plop or hygen are modern alternatives
- [**slush**](https://slushjs.github.io/) ([GitHub](https://github.com/slushjs/slush))
  - Scaffolding tool meant to replace Yeoman
- **kyt** ([GitHub](https://github.com/NYTimes/kyt))
  - Web app configuration toolkit

### React

- [**React Boilerplate**](https://www.reactboilerplate.com/) ([GitHub](https://github.com/react-boilerplate/react-boilerplate))
  - Once popular, but now out of date
  - Has a [**TypeScript fork**](https://github.com/react-boilerplate/react-boilerplate-typescript/)
- **`create-react-library`** ([GitHub](https://github.com/transitive-bullshit/create-react-library))
  - [**Slow**](https://github.com/transitive-bullshit/create-react-library/issues/171) maintenance and development
- [**enclave**](http://enclave.js.org/) ([GitHub](https://github.com/eanplatter/enclave))
  - React app compiler; supplanted by bundlers and Babel

## Bundlers

- **minipack** ([GitHub](https://github.com/ronami/minipack))
- [**StealJS**](https://stealjs.com/) ([GitHub](https://github.com/stealjs/steal))
- **HappyPack** ([GitHub](https://github.com/amireh/happypack))
- **Pundle** ([GitHub](https://github.com/steelbrain/pundle))
- [**Bili**](https://bili.egoist.sh/) ([GitHub](https://github.com/egoist/bili))
  - Rollup-based library bundler
- [**Fastpack**](https://fastpack.sh/) ([GitHub](https://github.com/fastpack/fastpack))
- **Jarvis** ([GitHub](https://github.com/zouhir/jarvis))
  - Webpack dashboard, unmaintained
- [**Broccoli.js**](https://broccoli.build/) ([GitHub](https://github.com/broccolijs/broccoli))
  - Asset pipeline
- [**Brunch**](https://brunch.io/) ([GitHub](https://github.com/brunch/brunch))

## Doc generators

- **dgeni** ([GitHub](https://github.com/angular/dgeni))
- [**JSDoc**](https://jsdoc.app/) ([GitHub](https://github.com/jsdoc/jsdoc))
- [**Documentation.js**](http://documentation.js.org/) ([GitHub](https://github.com/documentationjs/documentation))
- [**Docco**](http://ashkenas.com/docco/) ([GitHub](https://github.com/jashkenas/docco))
- [**dexy**](http://www.dexy.it/) ([GitHub](https://github.com/dexy/dexy))

## Test tools

- **QUnit** ([GitHub](https://github.com/qunitjs/qunit))
  - Java-inspired, dated library

### Coverage

- **blanket** ([GitHub](https://github.com/alex-seville/blanket))

## Runtimes

- **ts-node** ([GitHub](https://github.com/TypeStrong/ts-node))
  - `babel-node` should be preferable

## Other

- [**Grunt**](https://gruntjs.com/) ([GitHub](https://github.com/gruntjs/grunt))
- [**Gulp**](https://gulpjs.com/) ([GitHub](https://github.com/gulpjs/gulp))
- [**TSLint**](https://palantir.github.io/tslint/) ([GitHub](https://github.com/palantir/tslint))
  - Deprecated in favor of `typescript-eslint`
- [**Bower**](http://bower.io/) ([GitHub](https://github.com/bower/bower))
  - Package manager, popular in the jQuery ecosystem
- **JSHint** ([GitHub](https://github.com/jshint/jshint))
  - A linter developed as a more configurable JSLint but now outclassed by ESLint
- [**Tern**](https://ternjs.net/) ([GitHub](https://github.com/ternjs/tern))
  - Outclassed by TypeScript, since `tsc` can also analyze JavaScript
- [**JSLint**](https://jslint.com/) ([GitHub](https://github.com/douglascrockford/JSLint))
  - Ancient despite still being updated
- **Modernizr** ([GitHub](https://github.com/Modernizr/Modernizr))
  - Replaced by `@babel/preset-env`
- **plato** ([GitHub](https://github.com/es-analysis/plato))
- **jsinspect** ([GitHub](https://github.com/danielstjules/jsinspect))
- **React Hot Loader** ([GitHub](https://github.com/gaearon/react-hot-loader))
  - Replaced by [React Fast Refresh](https://github.com/facebook/react/issues/16604)
- **Retire.js** ([GitHub](https://github.com/RetireJS/retire.js))
- **JavaScript Stack from Scratch** ([GitHub](https://github.com/verekia/js-stack-from-scratch))
  - Resource about tooling; years out of date
- **next-update** ([GitHub](https://github.com/bahmutov/next-update))
- **dtslint** ([GitHub](https://github.com/microsoft/dtslint))
  - `tsd` should be used instead
- **js-beautify** ([GitHub](https://github.com/beautify-web/js-beautify))
  - Prettier is a modern alternative
- **precise-commits** ([GitHub](https://github.com/nrwl/precise-commits))
- [**NPMCompare.com**](https://npmcompare.com/)
- [**DocPad**](https://docpad.bevry.me/) ([GitHub](https://github.com/docpad/docpad))
