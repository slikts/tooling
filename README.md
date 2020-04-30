<h1 align=center>JavaScript and TypeScript tooling overview</h1>

<p align=center aria-hidden=true>
  <a href="https://GitHub.com/slikts/tooling/graphs/contributors/" target="_blank"><img src="https://img.shields.io/github/contributors/slikts/tooling.svg" alt="GitHub contributors"></a>
  <a href="https://GitHub.com/slikts/tooling/issues/" target="_blank"><img src="https://img.shields.io/github/issues/slikts/tooling.svg" alt="GitHub issues"></a>
  <img alt="GitHub" src="https://img.shields.io/github/license/slikts/tooling">
  <a href="https://github.com/slikts/tooling/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/slikts/tooling?style=social"></a>
</p>

A quick and up-to-date overview of existing build and developer tools for JavaScript and TypeScript.

The intended audience is project maintainers and tool authors. The list is selective; [non-recommended][non-rec] tools are listed separately. Existing resources with a similar focus on tooling are [listed][also] at the end; the motivation for this list is filling a gap in them.

The list format includes links to project homepages (if they exist), GitHub pages, and [npm trends] comparisons where applicable. The format differs from the [awesome] template by being slightly more detailed and opinionated.

Criticism, adding omissions and other contributions are [welcome][issues].

[issues]: https://github.com/slikts/tooling/issues
[also]: #🙈-see-also
[awesome]: https://github.com/sindresorhus/awesome
[npm trends]: https://www.npmtrends.com/

## 🔥 Zero-config presets

> [_npm trends_](https://www.npmtrends.com/create-react-app-vs-neutrino-vs-@pika/pack-vs-nwb-vs-tsdx) 📈

Presets, generators or [initializers](https://docs.npmjs.com/cli/init) that don't require configuration to start using them. Presets are recommended when starting out and to save the time and effort of building and maintaing a custom stack, but can be limited in certain aspects.

- [**@pika/pack**](https://www.pika.dev/blog/introducing-pika-pack/) ([GitHub](https://github.com/pikapkg/pack))
  - Build `npm` packages using composable plugins
- **nwb** ([GitHub](https://github.com/insin/nwb))
  - Toolkit for quick development with React, Inferno, Preact or vanilla JavaScript
- **TSDX** ([GitHub](https://github.com/jaredpalmer/tsdx))
  - Library-oriented preset for TypeScript
- [**Neutrino**](https://neutrinojs.org/) ([GitHub](https://github.com/neutrinojs/neutrino/))
  - Zero-configuration presets for React, Preact, Vue, web and Node.js projects and libraries; lacks TypeScript support

### React presets and frameworks

- [**Create React App**](https://create-react-app.dev/) ([GitHub](https://github.com/facebook/create-react-app))
  - The most popular React project initializer; supports TypeScript and many other tools, and is a safe choice for starting a React app
- [**Next.js**](https://nextjs.org/) ([GitHub](https://github.com/zeit/next.js))
  - React framework for server-side rendering
- [**Gatsby**](https://www.gatsbyjs.org/) ([GitHub](https://github.com/gatsbyjs/gatsby))
  - PWA and static site generator
- [**React Starter Kit**](https://reactstarter.com/) ([GitHub](https://github.com/kriasoft/react-starter-kit))
  - "[Isomorphic](https://medium.com/airbnb-engineering/isomorphic-javascript-the-future-of-web-apps-10882b7a2ebc#.4nyzv6jea)" (universal) web app boilerplate

### Toolchains

- [**Rome**](https://romejs.dev/) ([GitHub](https://github.com/facebookexperimental/rome))
  - Rome is an experimental JavaScript toolchain from Facebook which includes a compiler, linter, formatter, bundler, testing framework and more

## 🚚 Bundlers

> [_npm trends_](https://www.npmtrends.com/parcel-vs-webpack-vs-rollup-vs-fuse-box-vs-poi-vs-microbundle-vs-happypack-vs-fastpack-vs-webpack-jarvis-vs-browserify) 📈

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
- [**browserify**](http://browserify.org/) ([GitHub](https://github.com/browserify/browserify))
  - The first JavaScript bundler around

### Other

- [**Prepack**](https://prepack.io/) ([GitHub](https://github.com/facebook/prepack))
  - Bundle optimizer
- [**Snowpack**](https://snowpack.dev/) ([GitHub](https://github.com/pikapkg/snowpack))
  - Used by Pika

## 👨‍💻 Compilers

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

> [_npm trends_](https://www.npmtrends.com/eslint-vs-prettier-vs-xo-vs-standard-vs-eslint-config-airbnb-vs-tslint-vs-eslint-config-google-vs-jshint-vs-js-beautify-vs-zoe) 📈

- [**ESLint**](https://eslint.org/) ([GitHub](https://github.com/eslint/eslint))
  - The defacto standard linter for JavaScript (and TypeScript since `typescript-eslint`)
  - `eslint-config-airbnb` ([GitHub](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb))
    - The most popular ruleset for ESLint; relatively conservative
  - [**Standard**](https://standardjs.com/) ([GitHub](https://github.com/standard/standard))
    - A popular ruleset, although the "standard" name is more tongue in cheek
  - [**`typescript-eslint`**](https://typescript-eslint.io/) ([GitHub](https://github.com/typescript-eslint/typescript-eslint))
    - Replacement for the now-deprecated TSLint
  - **`eslint-config-es`** ([GitHub](https://github.com/thenativeweb/eslint-config-es))
    - ESLint configuration with a focus on strictness; supports TypeScript, React
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
- **Zoe** ([GitHub](https://github.com/jorgegonzalez/zoe))
  - Zero-config ESLint toolchain; includes Prettier and supports Jest and React

## 🐌 Runtimes

- [**Node.js**](https://nodejs.org/) ([GitHub](https://github.com/nodejs/node))
  - The de facto standard runtime for JavaScript; includes the `npm` and `npx` tools
- [**`babel-node`**](https://babeljs.io/docs/en/next/babel-node.html)
  - Can execute or provide a REPL for, e.g., TypeScript
- [**Deno**](https://deno.land/) ([GitHub](https://github.com/denoland/deno))
  - JavaScript and TypeScript runtime with an alternative module design
- **ts-node** ([GitHub](https://github.com/TypeStrong/ts-node))

### Version managers

- **`nvm`** ([GitHub](https://github.com/nvm-sh/nvm))
  - A commonly used version manager for Node.js
- **`fnm`** ([GitHub](https://github.com/Schniz/fnm))
  - Fast Node Manager; built in native ReasonML
- [**Volta**](https://volta.sh/) ([GitHub](https://github.com/volta-cli/volta))
  - Fast, reliable and universal version manager for the whole Node.js toolchain; written in Rust

## 🏃 Testing

Tools for end-to-end, integration and unit testing.

### Test libraries and frameworks

> [_npm trends_](https://www.npmtrends.com/mocha-vs-chai-vs-jest-vs-jasmine-vs-expect.js-vs-should-vs-sinon-vs-testdouble) 📈

- [**Mocha**](https://mochajs.org/) ([GitHub](https://github.com/mochajs/mocha))
  - Test framework
- [**Jasmine**](https://jasmine.github.io/) ([GitHub](https://github.com/jasmine/jasmine))
  - BDD testing framework
- [**Chai**](https://www.chaijs.com/) ([GitHub](https://github.com/chaijs/chai))
  - BDD or TDD assertion library for Node.js and browsers
- [**Sinon**](https://sinonjs.org/) ([GitHub](https://github.com/sinonjs/sinon))
  - Test spies, stubs and mocks
- **testdouble.js** ([GitHub](https://github.com/testdouble/testdouble.js))
  - A minimal test double library for TDD

#### "Over the wire" test doubles

> [_npm trends_](https://www.npmtrends.com/nock-vs-supertest-vs-mountebank-vs-chai-http) 📈

- **Nock** ([GitHub](https://github.com/nock/nock#readme))
  - HTTP server mocking and expectations library for Node.js
- **SuperTest** ([GitHub](https://github.com/visionmedia/supertest))
  - HTTP assertions using [superagent](http://github.com/visionmedia/superagent)
- [**Mountebank**](http://www.mbtest.org/) ([GitHub](https://github.com/bbyars/mountebank))
  - Service virtualization tool with support for mock verification, stubbing with advanced predicates, JavaScript injection, and record-playback through proxying; supports HTTP, TCP and SMTP and can support custom protocols
- [**Chai HTTP**](http://chaijs.com/plugins/chai-http) ([GitHub](https://github.com/chaijs/chai-http))
  - HTTP integration testing addon for Chai

### Test runners

> [_npm trends_](https://www.npmtrends.com/testcafe-vs-cypress-vs-jest-vs-karma-vs-ava-vs-nightwatch-vs-puppeteer) 📈

- [**Jest**](https://jestjs.io/) ([GitHub](https://github.com/facebook/jest))
  - Popular, well-polished test runner; supports TypeScript via `@babel/preset-typescript` and `babel-jest`; includes tools for spies, stubs, mocks and assertions
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
  - Automate end-to-end web testing
- [**Cypress**](https://www.cypress.io/)
  - End-to-end test runner
  - **`cypress-testing-library`** ([GitHub](https://github.com/testing-library/cypress-testing-library))
    - Custom Cypress commands and utilities to avoid testing implementation details
- [**Nightwatch**](https://nightwatchjs.org/) ([GitHub](https://github.com/nightwatchjs/nightwatch))
- [**Puppeteer**](https://pptr.dev/) ([GitHub](https://github.com/puppeteer/puppeteer))
  - Library for controlling headless Chrome or Chromium instances
- **Playwright** ([GitHub](https://github.com/microsoft/playwright))
  - Node library to automate the Chromium, WebKit and Firefox browsers with a single API; made by Microsoft

### React testing

- [**Enzyme**](https://enzymejs.github.io/enzyme/) ([GitHub](https://github.com/enzymejs/enzyme))
  - Assert, manipulate and traverse React components
- [**React Testing Library**](https://testing-library.com/react) ([GitHub](https://github.com/testing-library/react-testing-library))
  - Focused on avoiding testing implementation details

## 🐇 Performance

### Benchmarking and profiling

- **Benny** ([GitHub](https://github.com/caderek/benny))
  - Simple benchmark framework
- [**Clinic.js**](https://clinicjs.org) ([GitHub](https://github.com/nearform/node-clinic))
  - Node.js performance profiling suite

### Performance monitoring

- [**Falco**](https://getfal.co) ([GitHub](https://github.com/theodo/falco))
  - Automatically audit performance with [WebPageTest](https://www.webpagetest.org/)

### React performance

- [**`storybook-addon-performance`**](https://storybook-addon-performance.netlify.com) ([GitHub](https://github.com/atlassian-labs/storybook-addon-performance))
  - Storybook addon for debugging React component performance

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

## ☂️ Monorepos

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
  - **graphql-let** ([GitHub](https://github.com/piglovesyou/graphql-let))
- **tsd** ([GitHub](https://github.com/SamVerschueren/tsd))
  - Check TypeScript type definitions with assertions
  - A recent alternative is [`@ts-expect-error`](https://github.com/microsoft/TypeScript/pull/36014)
- [**AssemblyScript**](https://docs.assemblyscript.org/) ([GitHub](https://github.com/AssemblyScript/assemblyscript))
  - Compile TypeScript to WASM
- [**ts-jest**](https://kulshekhar.github.io/ts-jest) ([GitHub](https://github.com/kulshekhar/ts-jest))
  - TypeScript preprocessor with sourcemap support for Jest
- **`gts`** ([GitHub](https://github.com/google/gts))
  - Google TypeScript Style; zero-configuration formatting, linting and code fixing
- **`tsc-watch`** ([GitHub](https://github.com/gilamran/tsc-watch))
  - `nodemon` for TypeScript
- [**Tsearch**](https://tsearch.io) ([GitHub](https://github.com/tsearch-io/tsearch))
  - Search functions in different packages by their type signature
- **`dts-bundle-generator`** ([GitHub](https://github.com/timocov/dts-bundle-generator))
  - Tool to generate a single bundle of dts

### Documentation

- [**TSDoc**](https://microsoft.github.io/tsdoc/) ([GitHub](https://github.com/microsoft/tsdoc))
  - A documentation comment standard
- [**API Extractor**](https://api-extractor.com/) ([GitHub](https://github.com/microsoft/rushstack/blob/master/apps/api-extractor/README.md))
  - Analysis tool that can extract API reports for an API review workflow, bundle multiple declaration files into one, and extract a documentation model and generate an API reference website from it
- See also: [**TypeDoc**](#📚-documentation-generators)

### Rollup plugins

> [_npm trends_](https://www.npmtrends.com/@wessberg/rollup-plugin-ts-vs-rollup-plugin-typescript2) 📈

Useful for generating library type definitions; can be replaced with `tsc` for applications.

- **`@wessberg/rollup-plugin-ts`** ([GitHub](https://github.com/wessberg/rollup-plugin-ts))
  - A more modern but slightly less mature alternative to `rollup-plugin-typescript2`
- **`rollup-plugin-typescript2`** ([GitHub](https://github.com/ezolenko/rollup-plugin-typescript2/))

## 📦 Package management

### Package managers

> [_npm trends_](https://www.npmtrends.com/yarn-vs-pnpm-vs-tink-vs-npm) 📈

- **npm** ([GitHub](https://github.com/npm/cli))
  - The package manager included with Node.js
- [**Yarn**](https://yarnpkg.com/) ([GitHub](https://github.com/yarnpkg/yarn))
  - Replacement for `npm`
  - Recently released [Yarn 2](https://dev.to/arcanis/introducing-yarn-2-4eh1)
- **tink** ([GitHub](https://github.com/npm/tink))
  - Experimental "dependency unwinder"
- [**pnpm**](https://pnpm.js.org/en/) ([GitHub](https://github.com/pnpm/pnpm))
  - Links dependencies instead of copying to save space
- [**entropic**](https://discourse.entropic.dev/) ([GitHub](https://github.com/entropic-dev/entropic))
  - Federated package registry aiming to [replace npm](https://youtu.be/MO8hZlgK5zc)

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
  - Fix issues with packages without having to fork them or waiting
- **`npm-package-scripts`** (`nps`) ([GitHub](https://github.com/sezna/nps))
  - A specialized tool for having complex `npm` scripts
- **`bundlesize`** ([GitHub](https://github.com/siddharthkp/bundlesize))
  - Set configurable bundle size limits
- **Size Limit** ([GitHub](https://github.com/ai/size-limit))
  - Performance budget tool
- **Depcheck** ([GitHub](https://github.com/depcheck/depcheck))
  - Check `npm` packages for unused dependencies
- **`why-npm-i-so-long`** ([GitHub](https://github.com/antonk52/why-npm-i-so-long))
- [**Package Phobia**](https://packagephobia.now.sh/) ([GitHub](https://github.com/styfle/packagephobia))
- **`nrm`** ([GitHub](https://github.com/Pana/nrm))
  - `npm` registry manager; fast switch between different registries
- [**Open-Registry**](https://open-registry.dev/)
  - Community-funded mirror of the `npm` registry
- [**Dependency cruiser**](https://npmjs.com/dependency-cruiser) ([GitHub](https://github.com/sverweij/dependency-cruiser))
  - Validate and visualize dependencies

## 💡 Create React App

> [_npm trends_](https://www.npmtrends.com/react-app-rewired-vs-@craco/craco-vs-customize-cra) 📈

Create React App purposely limits its configurability to be able to give developer guarantees, but there are advanced use cases that require configuration while still avoiding "ejecting" from Create React App.

- **craco** ([GitHub](https://github.com/gsoft-inc/craco))
- **react-app-rewired** ([GitHub](https://github.com/timarney/react-app-rewired))

## 🎨 Design systems and prototyping

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
- [**Diez**](https://diez.org/) ([GitHub](https://github.com/diez/diez))
  - Developer toolkit for building [design tokens](https://diez.org/glossary/#tokens)
- [**React Figma**](https://react-figma.now.sh/) ([GitHub](https://github.com/react-figma/react-figma))
  - Render React components to [Figma](https://www.figma.com/)

## ❌ Cross-platform

- **`cross-env`** ([GitHub](https://github.com/kentcdodds/cross-env))
  - Set and use environment variables across platforms
- **`shx`** ([GitHub](https://github.com/shelljs/shx))
  - Unix-like shell commands

## 🗿 GraphQL

- **`eslint-plugin-graphql`** ([GitHub](https://github.com/apollographql/eslint-plugin-graphql))
  - ESLint plugin to validate GraphQL query strings against a schema

## 🚧 Unvetted or uncategorized

### TypeScript

- **`node-typescript-boilerplate`** ([GitHub](https://github.com/jsynowiec/node-typescript-boilerplate))
- **`ttypescript`** ([GitHub](https://github.com/cevek/ttypescript))
  - Wraps `tsc` to enable transforming the compiled code
- **TypeScript Node Starter** ([GitHub](https://github.com/microsoft/TypeScript-Node-Starter))
  - Microsoft's end-to-end project setup for Node.js using TypeScript

#### webpack plugins

- **`ts-loader`** ([GitHub](https://github.com/TypeStrong/ts-loader))
  - TypeScript loader for webpack
- [**Fork TS Checker Webpack Plugin**](https://blog.johnnyreilly.com/2019/07/typescript-and-eslint-meet-fork-ts-checker-webpack-plugin.html) ([GitHub](https://github.com/TypeStrong/fork-ts-checker-webpack-plugin))
  - Runs TypeScript type checker in a separate process from webpack

### React

- **`react-axe`** ([GitHub](https://github.com/dequelabs/react-axe))
  - Accessibility auditing for React apps
- [**Loadable Components**](https://loadable-components.com/) ([GitHub](https://github.com/gregberge/loadable-components))
- **`react-loadable`** ([GitHub](https://github.com/jamiebuilds/react-loadable))

### Package management

- **`reg`** ([GitHub](https://github.com/mikeal/reg))
  - Experimental package manager for native ES modules
- **Yarn deduplicate** ([GitHub](https://github.com/atlassian/yarn-deduplicate))
  - Deduplication tool for `yarn.lock` files

### GraphQL

- [**`babel-blade`**](https://babel-blade.netlify.com/) ([GitHub](https://github.com/babel-blade/babel-blade))
  - Babel plugin/macro that generates GraphQL query strings inline to solve the [double declaration problem](https://babel-blade.netlify.com/docs/declarationdeclaration.html)

### React

- **`jest-react-profiler`** ([GitHub](https://github.com/bvaughn/jest-react-profiler))
  - Jest helpers for working with the React Profiler API

### Linting

- **`eslint-plugin-filenames`** ([GitHub](https://github.com/selaux/eslint-plugin-filenames))
- **`ls-lint`** ([GitHub](https://github.com/loeffel-io/ls-lint))

### WebExtensions

- **web-extension-starter** ([GitHub](https://github.com/abhijithvijayan/web-extension-starter))
- **Chrome Extension CLI** ([GitHub](https://github.com/dutiyesh/chrome-extension-cli))
- **Chrome Extension Boilerplate** ([GitHub](https://github.com/duo-labs/chrome-extension-boilerplate))
- **Web Store Upload CLI** ([GitHub](https://github.com/DrewML/chrome-webstore-upload-cli))

#### Extension testing

- **`sinon-chrome`** ([GitHub](https://github.com/acvetkov/sinon-chrome))

### Other

- [**Metro**](https://facebook.github.io/metro/) ([GitHub](https://github.com/facebook/metro))
  - Bundler for React Native
- **Bundle Buddy** ([GitHub](https://github.com/samccone/bundle-buddy))
  - Identify bundle duplication across splits
- [**terser**](https://terser.org/) ([GitHub](https://github.com/terser/terser))
  - A more modern alternative to UglifyJS for "minifying" and obfuscating code
- [**Danger.js**](https://danger.systems/js/) ([GitHub](https://github.com/danger/danger-js))
  - Automated code review chores
- **`npm-run-all`** ([GitHub](https://github.com/mysticatea/npm-run-all))
- **`svgo`** ([GitHub](https://github.com/svg/svgo))
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
- [**Neutralino**](https://neutralino.js.org/) ([GitHub](https://github.com/neutralinojs/neutralinojs))
  - Portable and lightweight cross platform application development framework
- [**Phenomic**](https://phenomic.io/) ([GitHub](https://github.com/phenomic/phenomic))
  - Static site generator
- **tomo** ([GitHub](https://github.com/jhwohlgemuth/tomo-cli))
  - Zero-config React app generator
- **Mrm** ([GitHub](https://github.com/sapegin/mrm))
  - Sync configuration files between projects
- **`try`** ([GitHub](https://github.com/BrunnerLivio/try))
  - Quickly try out `npm` packages in a container
- **`webpack-nano`** ([GitHub](https://github.com/shellscape/webpack-nano))
  - Lightweight, configurable alternative to `webpack-cli`
- [**`npkill`**](https://voidcosmos.github.io/npkill/) ([GitHub](https://github.com/voidcosmos/npkill))
  - List and clean up all `node_modules` directories
- [**TypL**](https://TypL.dev) ([GitHub](https://github.com/getify/TypL))
  - JavaScript Type Linter; alternative to TypeScript
- **`format-graphql`** ([GitHub](https://github.com/gajus/format-graphql))
  - Alphabetically sorts definitions, fields and arguments in GraphQL schema definition language (SDL)
- [**Universal PWA Builder**](https://pwa.cafe) ([GitHub](https://github.com/lukeed/pwa))
  - Zero-configuration PWA presets for Preact, React, Vue and Svelte
- **StackTracey** ([GitHub](https://github.com/xpl/stacktracey))
  - Parses, cleans, filters and logs stack traces with source maps
- [**Codecrumbs**](https://codecrumbs.io) ([GitHub](https://github.com/Bogdan-Lyashenko/codecrumbs))
  - Visualize codebases
- [**Static Site Boilerplate**](http://staticsiteboilerplate.com) ([GitHub](https://github.com/ericalli/static-site-boilerplate))
- [**nodemon**](http://nodemon.io/) ([GitHub](https://github.com/remy/nodemon/))
  - Development tool for restarting a process on source changes
- [**PM2**](https://pm2.io) ([GitHub](https://github.com/Unitech/pm2))
  - Node.js production process manager with a built-in load balancer
- [**NPMCompare.com**](https://npmcompare.com/)
- [**ts-engine**](https://ts-engine.dev) ([GitHub](https://github.com/ts-engine/ts-engine))

## 💀 Legacy or not recommended tools

[Listed separately][non-rec] to avoid confusion.

[non-rec]: https://github.com/slikts/tooling/blob/master/not-recommended.md

## 🙈 See also

- [**JSter**](http://jster.net/blog)
  - Popular blog about libraries and tools
- [**StackShare**](https://stackshare.io/)
  - Social network centered around finding and vetting developer tools
- [**Free for developers**](https://free-for.dev/)
  - List of SaaS, PaaS and IaaS offerings that have free tiers of interest to devops and infradev
- [**awesome-web-dev-resources**](https://github.com/mrmartineau/awesome-web-dev-resources)
- [**Awesome lists**](https://github.com/sindresorhus/awesome)

### Outdated resources

- **JavaScript Stack from Scratch** ([GitHub](https://github.com/verekia/js-stack-from-scratch))
- [**frontend-dev-bookmarks Build Tools**](https://github.com/dypsilon/frontend-dev-bookmarks/blob/master/workflow/build-tools.md)
- [**awesome-javascript**](https://github.com/sorrycc/awesome-javascript)
