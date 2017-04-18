# npmdoc-underscore

#### api documentation for  [underscore (v1.8.3)](http://underscorejs.org)  [![npm package](https://img.shields.io/npm/v/npmdoc-underscore.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-underscore) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-underscore.svg)](https://travis-ci.org/npmdoc/node-npmdoc-underscore)

#### JavaScript's functional programming helper library.

[![NPM](https://nodei.co/npm/underscore.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/underscore)

- [https://npmdoc.github.io/node-npmdoc-underscore/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-underscore/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-underscore/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-underscore/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-underscore/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-underscore/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jeremy Ashkenas"
    },
    "bugs": {
        "url": "https://github.com/jashkenas/underscore/issues"
    },
    "dependencies": {},
    "description": "JavaScript's functional programming helper library.",
    "devDependencies": {
        "docco": "*",
        "eslint": "0.6.x",
        "karma": "~0.12.31",
        "karma-qunit": "~0.1.4",
        "qunit-cli": "~0.2.0",
        "uglify-js": "2.4.x"
    },
    "directories": {},
    "dist": {
        "shasum": "4f3fb53b106e6097fcf9cb4109f2a5e9bdfa5022",
        "tarball": "https://registry.npmjs.org/underscore/-/underscore-1.8.3.tgz"
    },
    "files": [
        "underscore.js",
        "underscore-min.js",
        "underscore-min.map",
        "LICENSE"
    ],
    "gitHead": "e4743ab712b8ab42ad4ccb48b155034d02394e4d",
    "homepage": "http://underscorejs.org",
    "keywords": [
        "util",
        "functional",
        "server",
        "client",
        "browser"
    ],
    "license": "MIT",
    "main": "underscore.js",
    "maintainers": [
        {
            "name": "jashkenas"
        }
    ],
    "name": "underscore",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/jashkenas/underscore.git"
    },
    "scripts": {
        "build": "uglifyjs underscore.js -c \"evaluate=false\" --comments \"/    .*/\" -m --source-map underscore-min.map -o underscore-min.js",
        "doc": "docco underscore.js",
        "lint": "eslint underscore.js test/*.js",
        "test": "npm run test-node && npm run lint",
        "test-browser": "npm i karma-phantomjs-launcher && ./node_modules/karma/bin/karma start",
        "test-node": "qunit-cli test/*.js"
    },
    "version": "1.8.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
