# npmtest-vuex

#### basic test coverage for  [vuex (v2.3.1)](https://github.com/vuejs/vuex#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-vuex.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-vuex) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-vuex.svg)](https://travis-ci.org/npmtest/node-npmtest-vuex)

#### state management for Vue.js

[![NPM](https://nodei.co/npm/vuex.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/vuex)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-vuex/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-vuex/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-vuex/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-vuex/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-vuex/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-vuex/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-vuex/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-vuex/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-vuex/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-vuex/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-vuex/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-vuex/build/test-report.html](https://npmtest.github.io/node-npmtest-vuex/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-vuex/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-vuex/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-vuex/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-vuex/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vuex/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vuex/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-vuex/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-vuex/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Evan You"
    },
    "bugs": {
        "url": "https://github.com/vuejs/vuex/issues"
    },
    "dependencies": {},
    "description": "state management for Vue.js",
    "devDependencies": {
        "babel-core": "^6.22.1",
        "babel-eslint": "^7.1.1",
        "babel-loader": "^6.2.10",
        "babel-plugin-transform-runtime": "^6.22.0",
        "babel-polyfill": "^6.22.0",
        "babel-preset-es2015": "^6.22.0",
        "babel-preset-es2015-rollup": "^3.0.0",
        "babel-preset-stage-2": "^6.22.0",
        "babel-runtime": "^6.22.0",
        "chromedriver": "^2.27.2",
        "cross-spawn": "^5.0.1",
        "css-loader": "^0.26.1",
        "eslint": "^3.15.0",
        "eslint-config-vue": "^2.0.2",
        "eslint-plugin-vue": "^2.0.1",
        "express": "^4.14.1",
        "jasmine": "2.5.3",
        "jasmine-core": "2.5.2",
        "nightwatch": "^0.9.12",
        "nightwatch-helpers": "^1.2.0",
        "phantomjs-prebuilt": "^2.1.14",
        "rollup": "^0.41.4",
        "rollup-plugin-buble": "^0.15.0",
        "rollup-plugin-replace": "^1.1.1",
        "rollup-watch": "^3.2.2",
        "selenium-server": "^2.53.1",
        "todomvc-app-css": "^2.0.6",
        "typescript": "^2.1.5",
        "uglify-js": "^2.7.5",
        "vue": "^2.1.10",
        "vue-loader": "^11.0.0",
        "vue-template-compiler": "^2.1.10",
        "webpack": "^2.2.1",
        "webpack-dev-middleware": "^1.10.0",
        "webpack-hot-middleware": "^2.16.1"
    },
    "directories": {},
    "dist": {
        "shasum": "cde8e997c1f9957719bc7dea154f9aa691d981a6",
        "tarball": "https://registry.npmjs.org/vuex/-/vuex-2.3.1.tgz"
    },
    "files": [
        "dist",
        "src",
        "types/index.d.ts",
        "types/helpers.d.ts",
        "types/vue.d.ts"
    ],
    "gitHead": "03b386ea4e964ecd2cf816cb4141acf34b2ef81c",
    "homepage": "https://github.com/vuejs/vuex#readme",
    "license": "MIT",
    "main": "dist/vuex.js",
    "maintainers": [
        {
            "name": "yyx990803"
        }
    ],
    "module": "dist/vuex.esm.js",
    "name": "vuex",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/vuejs/vuex.git"
    },
    "scripts": {
        "build": "npm run build:main && npm run build:esm && npm run build:logger",
        "build:esm": "rollup -c build/rollup.config.js --environment ESM",
        "build:logger": "rollup -c build/rollup.logger.config.js",
        "build:main": "rollup -c build/rollup.config.js && uglifyjs dist/vuex.js -cm --comments -o dist/vuex.min.js",
        "dev": "node examples/server.js",
        "dev:dist": "rollup -wm -c build/rollup.config.js",
        "docs": "cd docs && gitbook serve",
        "docs:deploy": "cd docs && ./deploy.sh",
        "lint": "eslint src test",
        "release": "bash build/release.sh",
        "test": "npm run lint && npm run test:types && npm run test:unit && npm run test:e2e",
        "test:e2e": "node test/e2e/runner.js",
        "test:types": "tsc -p types/test",
        "test:unit": "rollup -c build/rollup.config.js && jasmine JASMINE_CONFIG_PATH=test/unit/jasmine.json"
    },
    "typings": "types/index.d.ts",
    "unpkg": "dist/vuex.js",
    "version": "2.3.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
