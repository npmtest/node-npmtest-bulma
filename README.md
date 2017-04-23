# npmtest-bulma

#### basic test coverage for  [bulma (v0.4.0)](http://bulma.io)  [![npm package](https://img.shields.io/npm/v/npmtest-bulma.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-bulma) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-bulma.svg)](https://travis-ci.org/npmtest/node-npmtest-bulma)

#### Modern CSS framework based on Flexbox

[![NPM](https://nodei.co/npm/bulma.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/bulma)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-bulma/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-bulma/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-bulma/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-bulma/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-bulma/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-bulma/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-bulma/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-bulma/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-bulma/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-bulma/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-bulma/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-bulma/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-bulma/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-bulma/build/test-report.html](https://npmtest.github.io/node-npmtest-bulma/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-bulma/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-bulma/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-bulma/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-bulma/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bulma/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bulma/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-bulma/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-bulma/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "bulma",
    "version": "0.4.0",
    "homepage": "http://bulma.io",
    "author": "Jeremy Thomas <bbxdesign@gmail.com> (http://jgthms.com)",
    "description": "Modern CSS framework based on Flexbox",
    "main": "bulma.sass",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jgthms/bulma.git"
    },
    "license": "MIT",
    "keywords": [
        "css",
        "sass",
        "flexbox",
        "responsive",
        "framework"
    ],
    "bugs": {
        "url": "https://github.com/jgthms/bulma/issues"
    },
    "devDependencies": {
        "autoprefixer": "^6.3.3",
        "captain-git-hook": "~1.0.5",
        "node-sass": "^3.4.2",
        "postcss-cli": "^2.5.1"
    },
    "scripts": {
        "build": "npm run build-clean && npm run build-sass && npm run build-autoprefix",
        "build-autoprefix": "postcss --use autoprefixer --output css/bulma.css css/bulma.css",
        "build-clean": "rm -rf css",
        "build-sass": "node-sass --output-style expanded --source-map true bulma.sass css/bulma.css",
        "deploy": "npm run build && npm run docs",
        "docs": "npm run docs-sass && npm run docs-autoprefix",
        "docs-autoprefix": "postcss --use autoprefixer --output docs/css/bulma-docs.css docs/css/bulma-docs.css",
        "docs-sass": "node-sass --output-style expanded docs/bulma-docs.sass docs/css/bulma-docs.css",
        "start": "npm run build-sass -- --watch",
        "start-docs": "npm run docs-sass -- --watch",
        "start-test": "npm run test-sass -- --watch",
        "test-sass": "node-sass --output-style expanded docs/bulma-test.sass docs/css/bulma-test.css"
    },
    "files": [
        "css",
        "sass",
        "bulma.sass",
        "LICENSE",
        "README.md"
    ],
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
