# Tooling resources for JavaScript and TypeScript

<p>
  <a href="https://GitHub.com/slikts/tooling/graphs/contributors/" target="_blank"><img src="https://img.shields.io/github/contributors/slikts/tooling.svg" alt="GitHub contributors"></a>
  <a href="https://GitHub.com/slikts/tooling/issues/" target="_blank"><img src="https://img.shields.io/github/issues/slikts/tooling.svg" alt="GitHub issues"></a>
</p>

Developer and build tools exist to avoid predictable problems and to enable efficient workflows, but tooling is a complex field with a lot of churn, and keeping abreast of it can be a full-time job. This list is intended to give a comprehensive and opinionated overview of the available tooling with a focus on JavaScript, TypeScript and React build tools.

It differs from [awesome] lists in that it includes links to both project homepages and GitHub repos, and to [npm trends], and it also lists non-recommended or legacy tools to make it clear that there are better alternatives. It also sets a high bar for tools to be recommended, so that it wouldn't become just a catalogue like is so common with awesome lists.

The intended audience are developers starting or maintaining projects and tool authors. This is a work in progress; criticism or other contributions are welcome.

[awesome]: https://github.com/sindresorhus/awesome
[npm trends]: https://www.npmtrends.com/

## 🔥 Zero-config presets

> [_npm trends_](https://www.npmtrends.com/create-react-app-vs-neutrino-vs-@pika/pack-vs-nwb-vs-tsdx) 📈

Presets, generators or [initializers](https://docs.npmjs.com/cli/init) that don't require configuration to start using them.

- [**Pika**](https://pika.dev/) ([GitHub](https://github.com/pikapkg/pack))
  - Build `npm` packages using composable plugins
- **nwb** ([GitHub](https://github.com/insin/nwb))
  - Toolkit for quick development with React, Inferno, Preact or vanilla JavaScript
- [**Next.js**](https://nextjs.org/) ([GitHub](https://github.com/zeit/next.js))
  - React framework for server-side rendering
- [**Neutrino**](https://neutrinojs.org/) ([GitHub](https://github.com/neutrinojs/neutrino/))
  - Zero-configuration presets for React, Preact, Vue, web, Node.js projects and libraries
- **TSDX** ([GitHub](https://github.com/jaredpalmer/tsdx))
  - Library-oriented preset for TypeScript

### React presets

- [**Create React App**](https://create-react-app.dev/) ([GitHub](https://github.com/facebook/create-react-app))
  - The most popular React project initializer; supports TypeScript and many other tools, and is a safe choice for starting a React app
- [**React Starter Kit**](https://reactstarter.com/) ([GitHub](https://github.com/kriasoft/react-starter-kit))
  - "[Isomorphic](https://medium.com/airbnb-engineering/isomorphic-javascript-the-future-of-web-apps-10882b7a2ebc#.4nyzv6jea)" web app boilerplate

## 🚚 Bundlers

> [_npm trends_](https://www.npmtrends.com/parcel-vs-webpack-vs-rollup-vs-fuse-box-vs-poi-vs-microbundle-vs-happypack-vs-fastpack-vs-webpack-jarvis) 📈

- [**webpack**](https://webpack.js.org/) ([GitHub](https://github.com/webpack/webpack))
  - The most popular bundler with a wide ecosystem of plugins; used by popular tools like Create React App
- [**Rollup**](https://rollupjs.org/) ([GitHub](https://github.com/rollup/rollup))
  - A bundler often used specifically for bundling libraries; requires plugins for TypeScript support (see TypeScript section below)
- [**Parcel**](https://parceljs.org/) ([GitHub](https://github.com/parcel-bundler/parcel))
  - A fast, zero-configuration bundler; builtin TypeScript support
- [**FuseBox**](https://fuse-box.org/) ([GitHub](https://github.com/fuse-box/fuse-box))
  - Fast bundler with many features and builtin publishing and TypeScript support
- **microbundle** ([GitHub](https://github.com/developit/microbundle))
  - Fast, zero-configuration bundler that aims to reduce bundle size; supports TypeScript out of the box
- [**Poi**](https://poi.js.org/) ([GitHub](https://github.com/egoist/poi))
  - Zero-config bundler based on webpack

### Other

- [**Prepack**](https://prepack.io/) ([GitHub](https://github.com/facebook/prepack))
  - Bundle optimizer
- [**Snowpack**](https://snowpack.dev/) ([GitHub](https://github.com/pikapkg/snowpack))
  - Used by Pika

## ✍ Compilers

Tools that allow "transcompiling" or "transpiling" JavaScript.

- [**Babel**](https://babeljs.io/) ([GitHub](https://github.com/babel/babel))
  - A tool to "downlevel compile" modern JavaScript to support older browsers; also used to add features like JSX to the language
  - [**`@babel/preset-env`**](https://babeljs.io/docs/en/babel-preset-env)
    - Tune Babel output for the minimum required level of browser support
- [**swc**](https://swc-project.github.io/) ([GitHub](https://github.com/swc-project/swc))
  - Very fast Babel alternative written in Rust
- [**TypeScript**](https://www.typescriptlang.org/) ([GitHub](https://github.com/microsoft/TypeScript))
  - JavaScript with gradual typing; particularly useful for library authors and larger projects

## 🧫 Code generators

> [_npm trends_](https://www.npmtrends.com/hygen-vs-plop) 📈

- [**hygen**](http://www.hygen.io/) ([GitHub](https://github.com/jondot/hygen))
  - Ad-hoc generator or project scaffold tool
- [**plop**](http://plopjs.com/) ([GitHub](https://github.com/plopjs/plop))
  - Boilerplate micro-generator framework

## 💅 Formatters and linters

> [_npm trends_](https://www.npmtrends.com/eslint-vs-prettier-vs-xo-vs-standard-vs-eslint-config-airbnb-vs-tslint-vs-eslint-config-google-vs-jshint-vs-js-beautify) 📈

- [**ESLint**](https://eslint.org/) ([GitHub](https://github.com/eslint/eslint))
  - The defacto standard linter for JavaScript (and TypeScript since `typescript-eslint`)
  - `eslint-config-airbnb` ([GitHub](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb))
    - The most popular ruleset for ESLint; relatively conservative
  - [**Standard**](https://standardjs.com/) ([GitHub](https://github.com/standard/standard))
    - A popular ruleset, but the "standard" title is more tongue in cheek
  - [**`typescript-eslint`**](https://typescript-eslint.io/) ([GitHub](https://github.com/typescript-eslint/typescript-eslint))
    - A replacement for the now-deprecated TSLint
- [**Prettier**](https://prettier.io/) ([GitHub](https://github.com/prettier/prettier))
  - Opinionated formatter for JavaScript and TypeScript; useful for automatically enforcing consistent formatting and hence, for example, simplifying code reviews
  - `prettier-eslint` ([GitHub](https://github.com/prettier/prettier-eslint))
    - Allows using Prettier as an ESLint plugin
  - `eslint-config-prettier` ([GitHub](https://github.com/prettier/eslint-config-prettier))
    - Prevents ESLint conflicts with Prettier
  - `pretty-quick` ([GitHub](https://github.com/azz/pretty-quick))
    - Skips running Prettier on unchanged files
- **XO** ([GitHub](https://github.com/xojs/xo))
  - Opinionated (zero-config), configurable ESLint wrapper

## 🐌 Runtimes

- [**babel-node**](https://babeljs.io/docs/en/next/babel-node.html)
  - Can execute or provide a REPL for, e.g., TypeScript
- [**deno**](https://deno.land/) ([GitHub](https://github.com/denoland/deno))
  - JavaScript and TypeScript runtime

## 🏃 Testing

Tools for end-to-end, integration and unit testing.

### Test libraries and frameworks

> [_npm trends_](https://www.npmtrends.com/mocha-vs-chai-vs-jest-vs-jasmine-vs-expect.js-vs-should-vs-sinon) 📈

- [**Mocha**](https://mochajs.org/) ([GitHub](https://github.com/mochajs/mocha))
  - Test framework
- [**Jasmine**](https://jasmine.github.io/) ([GitHub](https://github.com/jasmine/jasmine))
  - BDD testing framework
- [**chai**](https://www.chaijs.com/) ([GitHub](https://github.com/chaijs/chai))
  - BDD or TDD assertion library
- [**Sinon**](https://sinonjs.org/) ([GitHub](https://github.com/sinonjs/sinon))
  - Test spies, stubs and mocks

### Test runners

> [_npm trends_](https://www.npmtrends.com/testcafe-vs-cypress-vs-jest-vs-karma-vs-ava-vs-nightwatch-vs-puppeteer) 📈

- [**Jest**](https://jestjs.io/) ([GitHub](https://github.com/facebook/jest))
  - A popular, well-polished test runner; supports TypeScript via `@babel/preset-typescript` and `babel-jest`; includes tools for spies, stubs, mocks and assertions
  - **Majestic** ([GitHub](https://github.com/Raathigesh/majestic))
    - GUI for Jest
  - [**`jest-stare`**](https://dkelosky.github.io/jest-stare/) ([GitHub](https://github.com/dkelosky/jest-stare))
    - Jest HTML reporter
- [**Karma**](https://karma-runner.github.io/) ([GitHub](https://github.com/karma-runner/karma))
  - Test runner for browsers
- **AVA** ([GitHub](https://github.com/avajs/ava))
- [**Wallaby**](https://wallabyjs.com/) ([GitHub](https://github.com/wallabyjs/public))
  - Non-free; integrates test output in the editor

#### End-to-end testing focused frameworks

- [**TestCafe**](https://devexpress.github.io/testcafe/) ([GitHub](https://github.com/DevExpress/testcafe))
  - A Node.js tool to automate end-to-end web testing
- [**Cypress**](https://www.cypress.io/)
  - End-to-end test runner
  - **`cypress-testing-library`** ([GitHub](https://github.com/testing-library/cypress-testing-library))
    - Custom Cypress commands and utilities to avoid testing implementation details
- [**Nightwatch**](https://nightwatchjs.org/) ([GitHub](https://github.com/nightwatchjs/nightwatch))
- [**Puppeteer**](https://pptr.dev/) ([GitHub](https://github.com/puppeteer/puppeteer))
  - A library for controlling headless Chrome or Chromium instances

### React testing

- [**Enzyme**](https://enzymejs.github.io/enzyme/) ([GitHub](https://github.com/enzymejs/enzyme))
  - Assert, manipulate and traverse React components
- [**React Testing Library**](https://testing-library.com/react) ([GitHub](https://github.com/testing-library/react-testing-library))
  - Focused on avoiding testing implementation details

## 🐇 Benchmarking

- **Benny** ([GitHub](https://github.com/caderek/benny))
  - Simple benchmark framework

## 📚 Documentation generators

> [_npm trends_](https://www.npmtrends.com/docz-vs-docusaurus-vs-docsify-vs-docute-vs-jsdoc-vs-esdoc-vs-typedoc) 📈

- [**Docz**](https://www.docz.site/) ([GitHub](https://github.com/doczjs/docz))
  - Creates live-reloading, seo-friendly, production-ready documentation sites with MDX; based on Gatsby
- [**Docusaurus**](https://docusaurus.io/) ([GitHub](https://github.com/facebook/Docusaurus))
  - A popular, full-featured documentation generator
- [**docsify**](https://docsify.js.org/) ([GitHub](https://github.com/docsifyjs/docsify/))
  - Simple docs with an option to skip generating static files
- [**TypeDoc**](https://typedoc.org/) ([GitHub](https://github.com/TypeStrong/typedoc))
  - Generates API documentation from TypeScript
  - `typedoc-plugin-markdown` ([GitHub](https://github.com/tom-grey/typedoc-plugin-markdown))
    - Allows using the generated docs with Docusaurus
- [**ESDoc**](https://esdoc.org/) ([GitHub](https://github.com/esdoc/esdoc))
  - JavaScript API documentation generator

## 👨‍💻 Monorepos

- [**awesome-monorepo**](https://github.com/korfuri/awesome-monorepo)
  - List of monorepo resources

### Monorepo managers

> [_npm trends_](https://www.npmtrends.com/lerna-vs-bolt-vs-mondorepo-vs-oao-vs-@microsoft/rush-vs-create-nx-workspace) 📈

- [**Lerna**](https://lerna.js.org/) ([GitHub](https://github.com/lerna/lerna))
  - The most popular solution for managing monorepos
- [**Rush**](https://rushjs.io/) ([GitHub](https://github.com/microsoft/rushstack/))
  - Part of the Rush stack by Microsoft
- **Yarn** [**workspaces**](https://classic.yarnpkg.com/en/docs/workspaces/)
  - Can be used alone or in conjunction with Lerna
- [**Bolt**](http://boltpkg.com/) ([GitHub](https://github.com/boltpkg/bolt))
  - JavaScript project management based on Yarn
- **oao** ([GitHub](https://github.com/guigrpa/oao))
  - Yarn-based, opinionated

### Other

- [**nx**](https://nx.dev/) ([GitHub](https://github.com/nrwl/nx))
  - Automated (zero-config), extensible dev tool setup for monorepos
- **syncpack** ([GitHub](https://github.com/JamieMason/syncpack))
  - Manage multiple `package.json` files

## 🚀 Deployment and release tools

> [_npm trends_](https://www.npmtrends.com/semantic-release-vs-standard-version-vs-release-it-vs-shipit-cli-vs-gh-pages-vs-shipjs-vs-publish-please) 📈

- [**semantic-release**](https://semantic-release.gitbook.io/) ([GitHub](https://github.com/semantic-release/semantic-release))
  - Automated version management and package publishing based on [semver](https://semver.org/)
- **Shipit** ([GitHub](https://github.com/shipitjs/shipit))
  - Automation engine and a deployment tool; alternative to Capistrano
- **`release-it`** ([GitHub](https://github.com/release-it/release-it))
  - Automated versioning and package publishing
- [**Ship.js**](https://community.algolia.com/shipjs/) ([GitHub](https://github.com/algolia/shipjs))
- [**Conventional Commits**](https://www.conventionalcommits.org/)
  - A specification for adding human and machine readable meaning to commit messages
- **Standard Version** ([GitHub](https://github.com/conventional-changelog/standard-version))
  - Like **semantic-release** but without the automatic publishing
- **`gh-pages`** ([GitHub](https://github.com/tschaub/gh-pages))
  - Publish files to a `gh-pages` branch on GitHub (or any other branch)
  - [**Tutorial**](https://github.com/gitname/react-gh-pages) about using `gh-pages` with CRA
- **`publish-please`** ([GitHub](https://github.com/inikulin/publish-please))
  - Replacement for `npm publish`

## 🚩 TypeScript

- [**GraphQL Code Generator**](https://graphql-code-generator.com/) ([GitHub](https://github.com/dotansimha/graphql-code-generator))
  - Generate TypeScript types from GraphQL schema; invaluable for large projects
- **tsd** ([GitHub](https://github.com/SamVerschueren/tsd))
  - Check TypeScript type definitions with assertions
- [**AssemblyScript**](https://docs.assemblyscript.org/) ([GitHub](https://github.com/AssemblyScript/assemblyscript))
  - Compile TypeScript to WASM

### Rollup plugins

> [_npm trends_](https://www.npmtrends.com/@wessberg/rollup-plugin-ts-vs-rollup-plugin-typescript2) 📈

Useful for generating library type definitions; can be replaced with `tsc` for applications.

- **`@wessberg/rollup-plugin-ts`** ([GitHub](https://github.com/wessberg/rollup-plugin-ts))
  - A more modern but slightly less mature alternative to `rollup-plugin-typescript2`
- **`rollup-plugin-typescript2`** ([GitHub](https://github.com/ezolenko/rollup-plugin-typescript2/))

## 📦 Package management

### Package managers

> [_npm trends_](https://www.npmtrends.com/yarn-vs-pnpm-vs-tink-vs-npm) 📈

- [**Yarn**](https://yarnpkg.com/) ([GitHub](https://github.com/yarnpkg/yarn))
  - A replacement for `npm`
- **tink** ([GitHub](https://github.com/npm/tink))
  - Experimental "dependency unwinder"
- [**pnpm**](https://pnpm.js.org/en/) ([GitHub](https://github.com/pnpm/pnpm))
  - Links dependencies instead of copying to save space

### Package search, vetting

- [**Pika**](https://www.pika.dev/search)
- [**npm trends**](https://www.npmtrends.com/)
- [**npms**](https://npms.io/)

### Git hook managers

> [_npm trends_](https://www.npmtrends.com/husky-vs-@arkweid/lefthook-vs-pre-commit) 📈

- **Husky** ([GitHub](https://github.com/typicode/husky))
- **`lint-staged`** ([GitHub](https://github.com/okonet/lint-staged))
- **Lefthook** ([GitHub](https://github.com/Arkweid/lefthook))
  - [**Comparison**](https://github.com/Arkweid/lefthook/wiki/Comparison-with-other-solutions) with other solutions

### Desktop packaging

- **Electron Packager** ([GitHub](https://github.com/electron/electron-packager))
- **nexe** ([GitHub](https://github.com/nexe/nexe))

### Executables

- **`pkg`** ([GitHub](https://github.com/zeit/pkg))

### Other

- **`patch-package`** ([GitHub](https://github.com/ds300/patch-package))
  - A tool to fix issues with packages without having to fork them or wait for an official patch
- **`npm-package-scripts`** (`nps`) ([GitHub](https://github.com/sezna/nps))
  - A specialized tool for having complex `npm` scripts
- **`bundlesize`** ([GitHub](https://github.com/siddharthkp/bundlesize))
  - A configurable tool to set bundle size limits
- **Size Limit** ([GitHub](https://github.com/ai/size-limit))
  - Performance budget tool

## 💡 Create React App

> [_npm trends_](https://www.npmtrends.com/react-app-rewired-vs-@craco/craco-vs-customize-cra))

Create React App purposely limits its configurability to be able to give developer guarantees, but there are advanced use cases that require configuration while still avoiding "ejecting" from Create React App.

- **craco** ([GitHub](https://github.com/gsoft-inc/craco))
- **react-app-rewired** ([GitHub](https://github.com/timarney/react-app-rewired))

## 🎨 Design systems

> [_npm trends_](https://www.npmtrends.com/@storybook/cli-vs-react-styleguidist-vs-@compodoc/compodoc-vs-react-cosmos-vs-playroom) 📈

Tools for developing and testing components and for creating style guides and reusable collections of components.

- [**Storybook**](https://storybook.js.org/) ([GitHub](https://github.com/storybookjs/storybook))
  - The most popular solution for developing and testing component libraries
- [**React Styleguidist**](https://react-styleguidist.js.org/) ([GitHub](https://github.com/styleguidist/react-styleguidist))
  - Isolated React component development environment with a living style guide
- **Playroom** ([GitHub](https://github.com/seek-oss/playroom))
  - Design for different screen sizes and themes at the same time using React
- [**React Cosmos**](https://reactcosmos.org/) ([GitHub](https://github.com/react-cosmos/react-cosmos))
  - A development environment for scalable, high-quality UIs and visual TDD

## ❌ Cross-platform

- **`cross-env`** ([GitHub](https://github.com/kentcdodds/cross-env))
  - Set and use environment variables across platforms
- **`shx`** ([GitHub](https://github.com/shelljs/shx))
  - Unix-like shell commands

## ❓ Uncategorized

- [**Metro**](https://facebook.github.io/metro/) ([GitHub](https://github.com/facebook/metro))
  - Bundler for React Native
- **Bundle Buddy** ([GitHub](https://github.com/samccone/bundle-buddy))
  - A tool to identify bundle duplication across splits.
- [**terser**](https://terser.org/) ([GitHub](https://github.com/terser/terser))
  - A more modern alternative to UglifyJS for "minifying" and obfuscating code
- [**Danger.js**](https://danger.systems/js/) ([GitHub](https://github.com/danger/danger-js))
  - Automated code review chores
- **`npm-run-all`** ([GitHub](https://github.com/mysticatea/npm-run-all))
- **svgo** ([GitHub](https://github.com/svg/svgo))
  - SVG file optimizer
- **Vue Enterprise Boilerplate** ([GitHub](https://github.com/chrisvfritz/vue-enterprise-boilerplate))
- [**nyc**](https://istanbul.js.org/) ([GitHub](https://github.com/istanbuljs/nyc))
- [**React PWA**](https://www.reactpwa.com/) ([GitHub](https://github.com/Atyantik/react-pwa))
- **Electron Packager** ([GitHub](https://github.com/electron/electron-packager))
- **Angular Webpack Starter** ([GitHub](https://github.com/PatrickJS/starter))
- [**Capybara**](https://teamcapybara.github.io/capybara/) ([GitHub](https://github.com/teamcapybara/capybara))
- **`generact`** ([GitHub](https://github.com/diegohaz/generact))
  - Generate React components by replicating your own
- **react-redux-typescript-guide** ([GitHub](https://github.com/piotrwitek/react-redux-typescript-guide))
- **react-typescript-cheetsheet** ([GitHub](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet))
- **`ifdef-loader`** ([GitHub](https://github.com/nippur72/ifdef-loader))
- **`ncc`** ([GitHub](https://github.com/zeit/ncc))
- [**BundlePhobia**](https://bundlephobia.com/)
- [**API Extractor**](https://api-extractor.com/) ([GitHub](https://github.com/microsoft/rushstack/blob/master/apps/api-extractor/README.md))

## 🚧 Unvetted

### TypeScript boilerplate

- **`node-typescript-boilerplate`** ([GitHub](https://github.com/jsynowiec/node-typescript-boilerplate))

### React

- **`react-axe`** ([GitHub](https://github.com/dequelabs/react-axe))
  - Accessibility auditing for React apps
- [**Loadable Components**](https://loadable-components.com/) ([GitHub](https://github.com/gregberge/loadable-components))
- **`react-loadable`** ([GitHub](https://github.com/jamiebuilds/react-loadable))

## 💀 Legacy or not recommended tools

[List hosted separately](https://github.com/slikts/tooling/blob/master/not-recommended.md) to avoid confusion.

## 🙈 See also

- [**awesome-web-dev-resources**](https://github.com/mrmartineau/awesome-web-dev-resources)
- [**Awesome lists**](https://github.com/sindresorhus/awesome)

### _Outdated_ resources

- [**frontend-dev-bookmarks Build Tools**](https://github.com/dypsilon/frontend-dev-bookmarks/blob/master/workflow/build-tools.md)
- [**awesome-javascript**](https://github.com/sorrycc/awesome-javascript)
