# @friends-of-js/javascript-kit

[![Build Status](https://travis-ci.org/friends-of-js/javascript-kit.svg?branch=master)](https://travis-ci.org/friends-of-js/javascript-kit)
[![Maintainability](https://api.codeclimate.com/v1/badges/9b27632d1b43755d11a5/maintainability)](https://codeclimate.com/github/friends-of-js/javascript-kit/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/9b27632d1b43755d11a5/test_coverage)](https://codeclimate.com/github/friends-of-js/javascript-kit/test_coverage)
[![codecov](https://codecov.io/gh/friends-of-js/javascript-kit/branch/master/graph/badge.svg)](https://codecov.io/gh/friends-of-js/javascript-kit)
[![license](https://img.shields.io/github/license/friends-of-js/javascript-kit.svg)](LICENSE)

![Preview](https://s31vla.storage.yandex.net/rdisk/5afb860bd756882655be84f4e0c8f06a5b46d7b13dd33de46772e4fc0303c0df/5ad22ffc/WQE6_438HcyEeCp6WXRb_V8Rcrt0ki1iNnFvpE_PFrz-YALI3mbhXKgBIFFUMyykmrXdVnFjo6ScW1Btm2vzZw==?uid=0&filename=javascript-kit.gif&disposition=inline&hash=&limit=0&content_type=image%2Fgif&fsize=1741216&hid=33fb02433cfb68468a0fafae16524857&media_type=image&tknv=v2&etag=614a4432598c659c7004c9a55216f473&rtoken=QIK7qZFqk9n3&force_default=no&ycrid=na-4b371e84e3c0afe96487b91a83d9cea5-downloader3h&ts=569d1b4aef700&s=bc439ed37d6bb5c0bd01023e63f86fba88f2c77f49b9f3ae1a21c42ef7ff0c81&pb=U2FsdGVkX1-h5x2O0TBw6oySe0GSKBjJ-Lin4qTxy7zPLZQeWcDc5fukrNGzf_MaJ3gENqYxG7aSAE4HViQ0qYcgG9qvbbd9xyCsqQrI2Ys)

## Install

```sh
yarn add global @friends-of-js/javascript-kit
# or
npm install -g @friends-of-js/javascript-kit
```

## Usage

```bash
javascript-kit [directory]
```
 
## Features

- [x] Support JavaScript and TypeScript languages
- [x] Fully customizable
- [x] TSlint and ESlint out of the box
- [x] Modules for both Node.js and browser
- [x] Browser modules with webpack
- [x] Generate both CommonJS and ESNext modules for Node.js
- [x] Autogenerated TypeScript defenitions
- [x] Node.js tests with Mocha and Chai
- [x] Browser tests with Karma, Mocha and Chai
- [x] Code coverage for both TypeScript and JavaScript through Istanbul and nyc
- [x] Sending code coverage to Codecov, Codeclimate, and Codacy
- [x] TravisCI out of the box
- [x] Autogenerated docs
- [x] Publishing to github and npm after succesfull build
- [x] Publishing release to github with generated changelog
- [x] Git hooks for linting and testing before publishing

## Commands

For a complete list of the commands available for your module, see the section "scripts" in generated package.json

| Yarn               | Npm                   | Make               | Description                                       |
| ------------------ | --------------------- | ------------------ | ------------------------------------------------- |
| yarn build         | npm run build         | make build         | Build CommonJS, ESNext modules and Browser bundle |
| yarn lint          | npm run lint          | make lint          | Lint your code with TSLint or ESLint              |
| yarn fix           | npm run fix           | make fix           | Fix errors found by linter                        |
| yarn test          | npm run test          | make test          | Run tests                                         |
| yarn coverage      | npm run coverage      | make coverage      | Run tests and generate code coverage reports      |
| yarn docs          | npm run docs          | make docs          | Generate documentation                            |
| yarn release.major | npm run release.major | make release.major | Create and publish new major release              |
| yarn release.minor | npm run release.minor | make release.minor | Create and publish new minor release              |
| yarn release.patch | npm run release.patch | make release.patch | Create and publish new patch release              |
| yarn commit        | npm run commit        | make commit        | Interactively create conventional commit message  |


## Project structure

| Name                | Description                                                      |
| ------------------- | ---------------------------------------------------------------- |
| src                 | Your source files placed here                                    |
| spec                | Contains your tests files                                        |
| node_modules        | Contains all your npm dependencies                               |
| build               | Scripts that responsible for building package                    |
| build/browser       | Scripts for building browser package                             |
| build/module        | Typescript configs for building CommonJS and ESNext modules      |
| build/declarations  | Typescript definitions and config for building eclarations files |
| lib                 | Generated package                                                |
| lib/module          | Node module packages                                             |
| lib/module/commonjs | Commonjs node module using es5 features                          |
| lib/module/esnext   | Node module using es7 and esnext features                        |
| lib/browser         | Browser package generated by webpack                             |
| coverage            | Code coverage report files                                       |
| docs                | Generated documentation                                          |

## License

@friends-of-js/javascript-kit © [Dmitriy Romanov](https://github.com/friends-of-js), released under the MIT License.
Authored and maintained with help from contributors ([list](https://github.com/friends-of-js/javascript-kit/contributors)).