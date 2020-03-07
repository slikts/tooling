# 🛠️ Tooling resources for JavaScript and TypeScript

Developer and build tools exist to avoid predictable problems and to enable efficient workflows, but it's a complex field with a lot of churn, and keeping abreast of it can be a full-time job. This list is intended to give a comprehensive and opinionated overview of the available tooling with a focus on JavaScript, TypeScript and React build tools.

It differs from [awesome] lists in that it includes links to both project homepages and GitHub repos, and to [npm trends] comparisons of packages, and it also lists non-recommended or legacy tools to make it clear that there are better alternatives. It also sets a high bar for tools to be recommended, so that it wouldn't become just a catalogue like is so common with awesome lists.

The intended audience is developers starting or maintaining projects and tool authors. This is an early draft and a work in progress; criticism or other contributions are welcome.

[awesome]: https://github.com/sindresorhus/awesome
[*npm trends*]: https://www.npmtrends.com/

## 🚚 Bundlers

> [_npm trends_](https://www.npmtrends.com/parcel-vs-webpack-vs-rollup-vs-fuse-box-vs-poi-vs-microbundle-vs-happypack-vs-fastpack-vs-webpack-jarvis) 📈

- [webpack](https://webpack.js.org/) [:octocat:](https://github.com/webpack/webpack)
- [Rollup](https://rollupjs.org/) [:octocat:](https://github.com/rollup/rollup)
- [Parcel](https://parceljs.org/) [:octocat:](https://github.com/parcel-bundler/parcel)
- [FuseBox](https://fuse-box.org/) [:octocat:](https://github.com/fuse-box/fuse-box)
- microbundle [:octocat:](https://github.com/developit/microbundle)
- [Poi](https://poi.js.org/) [:octocat:](https://github.com/egoist/poi)
  - Zero-config bundler based on webpack

## 0️⃣ Zero-config presets

> [_npm trends_](https://www.npmtrends.com/create-react-app-vs-neutrino-vs-@pika/pack-vs-nwb-vs-tsdx) 📈

Presets, generators or [initializers](https://docs.npmjs.com/cli/init) that don't require configuration to start using them.

- [Create React App](https://create-react-app.dev/) [:octocat:](https://github.com/facebook/create-react-app)
  - The most popular React project initializer; supports TypeScript and many other tools
- [Neutrino](https://neutrinojs.org/) [:octocat:](https://github.com/neutrinojs/neutrino/)
- [Pika](https://pika.dev/) [:octocat:](https://github.com/pikapkg/pack)
- nwb [:octocat:](https://github.com/insin/nwb)
  - Toolkit for quick development with React, Inferno, Preact or vanilla JavaScript
- [React Starter Kit](https://reactstarter.com/) [:octocat:](https://github.com/kriasoft/react-starter-kit)
  - "[Isomorphic](https://medium.com/airbnb-engineering/isomorphic-javascript-the-future-of-web-apps-10882b7a2ebc#.4nyzv6jea)" web app boilerplate
- TSDX [:octocat:](https://github.com/jaredpalmer/tsdx)
- [Next.js](https://nextjs.org/) [:octocat:](https://github.com/zeit/next.js)
  - React framework for server-side rendering (SSR)

## ✍ Compilers

Tools that allow "transcompiling" or "transpiling" JavaScript.

- [Babel](https://babeljs.io/) [:octocat:](https://github.com/babel/babel)
  - [`@babel/preset-env`](https://babeljs.io/docs/en/babel-preset-env)
- [swc](https://swc-project.github.io/) [:octocat:](https://github.com/swc-project/swc)
  - Very fast Babel alternative written in Rust
- [TypeScript](https://www.typescriptlang.org/) [:octocat:](https://github.com/microsoft/TypeScript)

## Other

- [Prepack](https://prepack.io/) [:octocat:](https://github.com/facebook/prepack)
  - Bundle optimizer
- [Snowpack](https://snowpack.dev/) [:octocat:](https://github.com/pikapkg/snowpack)

### 🧫 Code generators

> [_npm trends_](https://www.npmtrends.com/hygen-vs-plop) 📈

- [hygen](http://www.hygen.io/) [:octocat:](https://github.com/jondot/hygen)
  - Ad-hoc generator or project scaffold tool
- [plop](http://plopjs.com/) [:octocat:](https://github.com/plopjs/plop)
  - Boilerplate micro-generator framework

### 💅 Formatters and linters

> [_npm trends_](https://www.npmtrends.com/eslint-vs-prettier-vs-xo-vs-standard-vs-eslint-config-airbnb-vs-tslint-vs-eslint-config-google-vs-jshint-vs-js-beautify) 📈

- ESLint - `eslint-config-airbnb` [:octocat:](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb)
  - [Standard](https://standardjs.com/) [:octocat:](https://github.com/standard/standard)
  - [`typescript-eslint`](https://typescript-eslint.io/) [:octocat:](https://github.com/typescript-eslint/typescript-eslint)
- [Prettier](https://prettier.io/) [:octocat:](https://github.com/prettier/prettier)
  - `eslint-config-prettier` [:octocat:](https://github.com/prettier/eslint-config-prettier)
  - `prettier-eslint` [:octocat:](https://github.com/prettier/prettier-eslint)
  - `pretty-quick` [:octocat:](https://github.com/azz/pretty-quick)
- XO [:octocat:](https://github.com/xojs/xo)
  - Opinionated (zero-config) but configurable ESLint wrapper

### 🐌 Runtimes

- [babel-node](https://babeljs.io/docs/en/next/babel-node.html)
  - Can execute or provide a REPL for, e.g., TypeScript
- [deno](https://deno.land/) [:octocat:](https://github.com/denoland/deno)
  - JavaScript and TypeScript runtime

### 🙈 Test tools

> [_npm trends_](https://www.npmtrends.com/testcafe-vs-cypress-vs-mocha-vs-jasmine-vs-jest-vs-chai-vs-karma-vs-ava) 📈

- [TestCafe](https://devexpress.github.io/testcafe/) [:octocat:](https://github.com/DevExpress/testcafe)
  - A Node.js tool to automate end-to-end web testing
- [Cypress](https://www.cypress.io/)
  - End-to-end test runner - `cypress-testing-library` [:octocat:](https://github.com/testing-library/cypress-testing-library)
  - Custom Cypress commands and utilities that encourage good testing practices
- [Mocha](https://mochajs.org/) [:octocat:](https://github.com/mochajs/mocha)
  - Test framework
- [Jasmine](https://jasmine.github.io/) [:octocat:](https://github.com/jasmine/jasmine)
  - BDD testing framework
- [chai](https://www.chaijs.com/) [:octocat:](https://github.com/chaijs/chai)
  - BDD or TDD assertion library
- [Sinon](https://sinonjs.org/) [:octocat:](https://github.com/sinonjs/sinon)
  - Test spies, stubs and mocks

#### 🏃 Test runners

- [Jest](https://jestjs.io/) [:octocat:](https://github.com/facebook/jest)
  - A popular, well-polished test runner; supports TypeScript via `@babel/preset-typescript` and `babel-jest` - Majestic [:octocat:](https://github.com/Raathigesh/majestic)
  - GUI for Jest - [`jest-stare`](https://dkelosky.github.io/jest-stare/) [:octocat:](https://github.com/dkelosky/jest-stare)
  - Jest HTML reporter - > [_npm trends_](https://www.npmtrends.com/majestic-vs-jest-stare-vs-jest-html-reporter-vs-jest-html-reporters) 📈
- [Karma](https://karma-runner.github.io/) [:octocat:](https://github.com/karma-runner/karma)
  - Test runner for browsers
- AVA [:octocat:](https://github.com/avajs/ava)
- [Wallaby](https://wallabyjs.com/) [:octocat:](https://github.com/wallabyjs/public)
  - Non-free

#### React

- [Enzyme](https://enzymejs.github.io/enzyme/) [:octocat:](https://github.com/enzymejs/enzyme)
  - Assert, manipulate and traverse React components
- [React Testing Library](https://testing-library.com/react) [:octocat:](https://github.com/testing-library/react-testing-library)
  - Focused on avoiding testing implementation details

#### Other

- Benny [:octocat:](https://github.com/caderek/benny)
  - Simple benchmark framework

### 📚 Documentation generators

> [_npm trends_](https://www.npmtrends.com/docz-vs-docusaurus-vs-docsify-vs-docute-vs-jsdoc-vs-esdoc-vs-typedoc) 📈

- [Docz](https://www.docz.site/) [:octocat:](https://github.com/doczjs/docz)
- [Docusaurus](https://docusaurus.io/) [:octocat:](https://github.com/facebook/Docusaurus)
- [docsify](https://docsify.js.org/) [:octocat:](https://github.com/docsifyjs/docsify/)
  - Docs without generating static files
- [TypeDoc](https://typedoc.org/) [:octocat:](https://github.com/TypeStrong/typedoc)
  - `typedoc-plugin-markdown` [:octocat:](https://github.com/tom-grey/typedoc-plugin-markdown)
  - Allows using the generated docs with Docusaurus
- [ESDoc](https://esdoc.org/) [:octocat:](https://github.com/esdoc/esdoc)

### Monorepos

- [awesome-monorepo](https://github.com/korfuri/awesome-monorepo)

#### Monorepo managers

> [_npm trends_](https://www.npmtrends.com/lerna-vs-bolt-vs-mondorepo-vs-oao-vs-@microsoft/rush-vs-create-nx-workspace) 📈

- [Lerna](https://lerna.js.org/) [:octocat:](https://github.com/lerna/lerna)
- [Rush](https://rushjs.io/) [:octocat:](https://github.com/microsoft/rushstack/)
- Yarn [workspaces](https://classic.yarnpkg.com/en/docs/workspaces/)
- [Bolt](http://boltpkg.com/) [:octocat:](https://github.com/boltpkg/bolt)
  - JavaScript project management based on Yarn
- oao [:octocat:](https://github.com/guigrpa/oao)
  - Yarn-based, opinionated

#### Other

- [nx](https://nx.dev/) [:octocat:](https://github.com/nrwl/nx)
  - Automated, extensible dev tool setup for monorepos
- syncpack [:octocat:](https://github.com/JamieMason/syncpack)
  - Manage multiple `package.json` files

### 🚀 Deployment and release tools

> [_npm trends_](https://www.npmtrends.com/semantic-release-vs-standard-version-vs-release-it-vs-shipit-cli-vs-gh-pages-vs-shipjs-vs-publish-please) 📈

- [semantic-release](https://semantic-release.gitbook.io/) [:octocat:](https://github.com/semantic-release/semantic-release)
  - Automated version management and package publishing based on [semver](https://semver.org/)
- Shipit [:octocat:](https://github.com/shipitjs/shipit)
  - Automation engine and a deployment tool; alternative to Capistrano
- release-it [:octocat:](https://github.com/release-it/release-it)
  - Automated versioning and package publishing
- [Ship.js](https://community.algolia.com/shipjs/) [:octocat:](https://github.com/algolia/shipjs)
- [Conventional Commits](https://www.conventionalcommits.org/)
  - A specification for adding human and machine readable meaning to commit messages
- standard-version [:octocat:](https://github.com/conventional-changelog/standard-version)
  - Like semantic-release but without the automatic publishing
- `gh-pages` [:octocat:](https://github.com/tschaub/gh-pages)
  - Publish files to a `gh-pages` branch on GitHub (or any other branch anywhere else)
  - [Tutorial](https://github.com/gitname/react-gh-pages) about using `gh-pages` with CRA
- `publish-please`: [:octocat:](https://github.com/inikulin/publish-please)
  - Replacement for `npm publish`

### 🚩 TypeScript

- [GraphQL Code Generator](https://graphql-code-generator.com/) [:octocat:](https://github.com/dotansimha/graphql-code-generator)
  - Generate TypeScript types from GraphQL schema; invaluable for large projects
- tsd [:octocat:](https://github.com/SamVerschueren/tsd)
  - Check TypeScript type definitions with assertions
- [AssemblyScript](https://docs.assemblyscript.org/) [:octocat:](https://github.com/AssemblyScript/assemblyscript)

#### Rollup plugins

> [_npm trends_](https://www.npmtrends.com/@wessberg/rollup-plugin-ts-vs-rollup-plugin-typescript2) 📈

Useful for generating library type definitions; can be replaced with `tsc` for applications.

- `@wessberg/rollup-plugin-ts` [:octocat:](https://github.com/wessberg/rollup-plugin-ts)
  - A more modern but less mature alternative to `rollup-plugin-typescript2`
- `rollup-plugin-typescript2` [:octocat:](https://github.com/ezolenko/rollup-plugin-typescript2/)

### 📦 Package management

#### Package managers

> [_npm trends_](https://www.npmtrends.com/yarn-vs-pnpm-vs-tink-vs-npm) 📈

- [Yarn](https://yarnpkg.com/) [:octocat:](https://github.com/yarnpkg/yarn)
- tink [:octocat:](https://github.com/npm/tink)
  - Experimental "dependency unwinder"
- [pnpm](https://pnpm.js.org/en/) [:octocat:](https://github.com/pnpm/pnpm)
  - Links dependencies instead of copying

#### Package search, vetting

- [Pika](https://www.pika.dev/search)
- [npms](https://npms.io/)
- > [_npm trends_](https://www.npmtrends.com/)

#### Git hook managers

> [_npm trends_](https://www.npmtrends.com/husky-vs-@arkweid/lefthook-vs-pre-commit) 📈

- Husky [:octocat:](https://github.com/typicode/husky)
- `lint-staged` [:octocat:](https://github.com/okonet/lint-staged)
- Lefthook [:octocat:](https://github.com/Arkweid/lefthook)
  - [Comparison](https://github.com/Arkweid/lefthook/wiki/Comparison-with-other-solutions) with other solutions

#### Desktop packaging

- Electron Packager [:octocat:](https://github.com/electron/electron-packager)
- nexe [:octocat:](https://github.com/nexe/nexe)

#### Executables

- `pkg` [:octocat:](https://github.com/zeit/pkg)

#### Other

- `patch-package` [:octocat:](https://github.com/ds300/patch-package)
- `npm-package-scripts` (`nps`) [:octocat:](https://github.com/sezna/nps)
- `bundlesize` [:octocat:](https://github.com/siddharthkp/bundlesize)
- Size Limit [:octocat:](https://github.com/ai/size-limit)
  - Performance budget tool

### Create React App

> [_npm trends_](https://www.npmtrends.com/react-app-rewired-vs-@craco/craco-vs-customize-cra)

- craco [:octocat:](https://github.com/gsoft-inc/craco)
- react-app-rewired [:octocat:](https://github.com/timarney/react-app-rewired)

### 🎨 Design systems

> [_npm trends_](https://www.npmtrends.com/@storybook/cli-vs-react-styleguidist-vs-@compodoc/compodoc-vs-react-cosmos-vs-playroom) 📈

- [Storybook](https://storybook.js.org/) [:octocat:](https://github.com/storybookjs/storybook)
- [React Styleguidist](https://react-styleguidist.js.org/) [:octocat:](https://github.com/styleguidist/react-styleguidist)
- Playroom[:octocat:](https://github.com/seek-oss/playroom)
- [React Cosmos](https://reactcosmos.org/) [:octocat:](https://github.com/react-cosmos/react-cosmos)

### ❌ Cross-platform

- `cross-env` [:octocat:](https://github.com/kentcdodds/cross-env)
  - Set and use environment variables across platforms
- `shx` [:octocat:](https://github.com/shelljs/shx)
  - Unix-like shell commands

## 💀 Legacy or not recommended

Tools that are deprecated, out of date, have better alternatives or have only niche uses.

### Compilers

- [Bublé](https://buble.surge.sh/) [:octocat:](https://github.com/bublejs/buble)
- [Closure Compiler](https://developers.google.com/closure/compiler) [:octocat:](https://github.com/google/closure-compiler)

### Zero-config presets

- [Yeoman](https://yeoman.io/) [:octocat:](https://github.com/yeoman/yeoman)
  - Generator; Plop or hygen are modern alternatives
- [slush](https://slushjs.github.io/) [:octocat:](https://github.com/slushjs/slush)
  - Scaffolding tool meant to replace Yeoman
- kyt [:octocat:](https://github.com/NYTimes/kyt)
  - Web app configuration toolkit

#### React

- [React Boilerplate](https://www.reactboilerplate.com/) [:octocat:](https://github.com/react-boilerplate/react-boilerplate)
  - [TypeScript fork](https://github.com/react-boilerplate/react-boilerplate-typescript/)
- `create-react-library` [:octocat:](https://github.com/transitive-bullshit/create-react-library)
  - [Slow](https://github.com/transitive-bullshit/create-react-library/issues/171) maintenance and development
- [enclave](http://enclave.js.org/) [:octocat:](https://github.com/eanplatter/enclave)
  - React app compiler

### Bundlers

- [browserify](http://browserify.org/) [:octocat:](https://github.com/browserify/browserify)
- minipack [:octocat:](https://github.com/ronami/minipack)
- [StealJS](https://stealjs.com/) [:octocat:](https://github.com/stealjs/steal)
- HappyPack [:octocat:](https://github.com/amireh/happypack)
- Pundle [:octocat:](https://github.com/steelbrain/pundle)
- [Bili](https://bili.egoist.sh/) [:octocat:](https://github.com/egoist/bili)
  - Rollup-based library bundler
- [Fastpack](https://fastpack.sh/) [:octocat:](https://github.com/fastpack/fastpack)
- Jarvis [:octocat:](https://github.com/zouhir/jarvis)
  - Webpack dashboard, unmaintained
- [Broccoli.js](https://broccoli.build/) [:octocat:](https://github.com/broccolijs/broccoli)
  - Asset pipeline
- [Brunch](https://brunch.io/) [:octocat:](https://github.com/brunch/brunch)

### Doc generators

- dgeni [:octocat:](https://github.com/angular/dgeni)
- [JSDoc](https://jsdoc.app/) [:octocat:](https://github.com/jsdoc/jsdoc)
- [Documentation.js](http://documentation.js.org/) [:octocat:](https://github.com/documentationjs/documentation)
- [Docco](http://ashkenas.com/docco/) [:octocat:](https://github.com/jashkenas/docco)
- [dexy](http://www.dexy.it/) [:octocat:](https://github.com/dexy/dexy)

### Test tools

- [ts-jest](https://kulshekhar.github.io/ts-jest) [:octocat:](https://github.com/kulshekhar/ts-jest)
  - TypeScript preprocessor with sourcemap support for Jest; not recommended due to [obstructive type error](https://github.com/jaredpalmer/tsdx/issues/521) output
- QUnit [:octocat:](https://github.com/qunitjs/qunit)
  - Java-inspired, dated library

#### Coverage

- blanket [:octocat:](https://github.com/alex-seville/blanket)

### Runtimes

- ts-node [:octocat:](https://github.com/TypeStrong/ts-node)
  - `babel-node` should be preferable

### Other

- [Grunt](https://gruntjs.com/) [:octocat:](https://github.com/gruntjs/grunt)
- [Gulp](https://gulpjs.com/) [:octocat:](https://github.com/gulpjs/gulp)
- [TSLint](https://palantir.github.io/tslint/) [:octocat:](https://github.com/palantir/tslint)
  - Deprecated in favor of `typescript-eslint`
- [Bower](http://bower.io/) [:octocat:](https://github.com/bower/bower)
  - Package manager
- JSHint [:octocat:](https://github.com/jshint/jshint)
- [Tern](https://ternjs.net/) [:octocat:](https://github.com/ternjs/tern)
- [JSLint](https://jslint.com/) [:octocat:](https://github.com/douglascrockford/JSLint)
  - Ancient despite still being updated
- Modernizr [:octocat:](https://github.com/Modernizr/Modernizr)
  - Replaced by `@babel/preset-env`
- plato [:octocat:](https://github.com/es-analysis/plato)
- jsinspect [:octocat:](https://github.com/danielstjules/jsinspect)
- React Hot Loader [:octocat:](https://github.com/gaearon/react-hot-loader)
  - Replaced by [React Fast Refresh](https://github.com/facebook/react/issues/16604)
- Retire.js [:octocat:](https://github.com/RetireJS/retire.js)
- JavaScript Stack from Scratch [:octocat:](https://github.com/verekia/js-stack-from-scratch)
  - Years out of date
- next-update [:octocat:](https://github.com/bahmutov/next-update)
- dtslint [:octocat:](https://github.com/microsoft/dtslint)
- js-beautify [:octocat:](https://github.com/beautify-web/js-beautify)
  - Prettier is a modern alternative
- precise-commits [:octocat:](https://github.com/nrwl/precise-commits)
- [NPMCompare.com](https://npmcompare.com/)
- [DocPad](https://docpad.bevry.me/) [:octocat:](https://github.com/docpad/docpad)

## ❓ Uncategorized

- [Metro](https://facebook.github.io/metro/) [:octocat:](https://github.com/facebook/metro)
  - Bundler for React Native
- Bundle Buddy [:octocat:](https://github.com/samccone/bundle-buddy)
  - A tool to identify bundle duplication across splits.
- [terser](https://terser.org/) [:octocat:](https://github.com/terser/terser)
- [Danger.js](https://danger.systems/js/) [:octocat:](https://github.com/danger/danger-js)
  - Automated code review chores
- `npm-run-all` [:octocat:](https://github.com/mysticatea/npm-run-all)
- svgo [:octocat:](https://github.com/svg/svgo)
- Vue Enterprise Boilerplate [:octocat:](https://github.com/chrisvfritz/vue-enterprise-boilerplate)
- [nyc](https://istanbul.js.org/) [:octocat:](https://github.com/istanbuljs/nyc)
- [React PWA](https://www.reactpwa.com/) [:octocat:](https://github.com/Atyantik/react-pwa)
- Electron Packager [:octocat:](https://github.com/electron/electron-packager)
- Angular Webpack Starter [:octocat:](https://github.com/PatrickJS/starter)
- [Capybara](https://teamcapybara.github.io/capybara/) [:octocat:](https://github.com/teamcapybara/capybara)
- `generact` [:octocat:](https://github.com/diegohaz/generact)
  - Generate React components by replicating your own
- react-redux-typescript-guide [:octocat:](https://github.com/piotrwitek/react-redux-typescript-guide)
- react-typescript-cheetsheet [:octocat:](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet)
- `ifdef-loader` [:octocat:](https://github.com/nippur72/ifdef-loader)
- `ncc` [:octocat:](https://github.com/zeit/ncc)
- [BundlePhobia](https://bundlephobia.com/)
- [API Extractor](https://api-extractor.com/) [:octocat:](https://github.com/microsoft/rushstack/blob/master/apps/api-extractor/README.md)

## Unvetted

### TypeScript boilerplate

- `node-typescript-boilerplate` [:octocat:](https://github.com/jsynowiec/node-typescript-boilerplate)

### React

- `react-axe` [:octocat:](https://github.com/dequelabs/react-axe)
  - Accessibility auditing for React apps
- [Loadable Components](https://loadable-components.com/) [:octocat:](https://github.com/gregberge/loadable-components)
- `react-loadable` [:octocat:](https://github.com/jamiebuilds/react-loadable)

## See also

- [awesome-web-dev-resources](https://github.com/mrmartineau/awesome-web-dev-resources)
- [Awesome lists](https://github.com/sindresorhus/awesome)

### Outdated resources

- [frontend-dev-bookmarks Build Tools](https://github.com/dypsilon/frontend-dev-bookmarks/blob/master/workflow/build-tools.md)
- [awesome-javascript](https://github.com/sorrycc/awesome-javascript)
