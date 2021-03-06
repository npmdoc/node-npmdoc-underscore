# npmdoc-underscore

#### basic api documentation for  [underscore (1.9.1)](http://underscorejs.org)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-underscore.svg)](https://travis-ci.org/npmdoc/node-npmdoc-underscore)

#### JavaScript's functional programming helper library.

[![NPM](https://nodei.co/npm/underscore.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/underscore)

- [https://npmdoc.github.io/node-npmdoc-underscore/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-underscore/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-underscore/build/screenshot.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-underscore/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-underscore/build/screenshot.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-underscore/build/screenshot.npmPackageDependencyTree.svg)



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
        "coveralls": "^2.11.2",
        "docco": "*",
        "eslint": "1.10.x",
        "gzip-size-cli": "^1.0.0",
        "karma": "^0.13.13",
        "karma-qunit": "~2.0.1",
        "nyc": "^2.1.3",
        "pretty-bytes-cli": "^1.0.0",
        "qunit": "^2.6.0",
        "qunit-cli": "~0.2.0",
        "uglify-js": "3.3.21"
    },
    "directories": {},
    "dist": {
        "integrity": "sha512-5/4etnCkd9c8gwgowi5/om/mYO5ajCaOgdzj/oW+0eQV9WxKBDZw5+ycmKmeaTXjInS/W0BzpGLo2xR2aBwZdg==",
        "shasum": "06dce34a0e68a7babc29b365b8e74b8925203961",
        "tarball": "https://registry.npmjs.org/underscore/-/underscore-1.9.1.tgz",
        "fileCount": 6,
        "unpackedSize": 110995,
        "npm-signature": "-----BEGIN PGP SIGNATURE-----\r\nVersion: OpenPGP.js v3.0.4\r\nComment: https://openpgpjs.org\r\n\r\nwsFcBAEBCAAQBQJbEGUHCRA9TVsSAnZWagAAIoIP/jT81dtAcYXnjT8M3neP\nYNCBTRbvovfxCG3xbwnAVq0g0/B6CBaeU+u+Gppz0oJ98vtuiGhstmj93pjy\ncwi+u3DsXMBEJ9E1DsK7ms3cBg7FnCqke+yXWvwv8J+RRoDRW0xcA04taFz4\nDVQtG0nmXOLSGl0eGVX8E7O3g1DrLUcObYHpegxjiKZVGLPoNb16Xlu13GgD\njwajvJ9xfwHOudl1+vVCc5ocyyeaqkK5oz9ri9cIyPhVVXPgtCWBzNwvlUGD\n8t/SM78AkrNVLyHAq2NMLANPPZhg1p0yuBTVu5+I3hhdBYmMBk3zQ6W+lcch\nmS1V5gQaGqjGh9ci+gRnIqY4WZZLDMHPQ9Ba0W6wkjRlCFV0z5MX+ia5V4R1\nWxrqwIwwHbEnEdPZQ/mT86WNLXi8/Izn5gpxp/xcoYvHRlYJST4USRTmkF8p\nrL+dduILMBTGxHSZtjXuFwlOXAiXROCUMSamStDa+02WddL9eUjSL/sjpFyG\nBWhkWaLSc9RrNSWkqlI4cgA9b72AN4tIbmoHeUlVFx4KCUWZwHTbTUkawYmu\n5iTvPevViilYOaGr9gTHo2BYtX+0u4TMtEnQg5rELeiuYp5/VJgqhCh0lUOJ\nqnDRfF7AgE6gQnwJhNi1QB8UFWqSQVZyKgQ9bA7In5J0WWxYwydK/Pml84lV\nqm/l\r\n=gqag\r\n-----END PGP SIGNATURE-----\r\n"
    },
    "files": [
        "underscore.js",
        "underscore-min.js",
        "underscore-min.js.map"
    ],
    "gitHead": "ae037f7c41323807ae6f1533c45512e6d31a1574",
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
        },
        {
            "name": "jridgewell"
        }
    ],
    "name": "underscore",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/jashkenas/underscore.git"
    },
    "scripts": {
        "build": "npm run minify -- --source-map --source-map-url \" \" -o underscore-min.js",
        "coverage": "nyc npm run test-node && nyc report",
        "coveralls": "nyc npm run test-node && nyc report --reporter=text-lcov | coveralls",
        "doc": "docco underscore.js",
        "lint": "eslint underscore.js test/*.js",
        "minify": "uglifyjs underscore.js -c \"evaluate=false\" --comments \"/    .*/\" -m",
        "test": "npm run lint && npm run test-node",
        "test-browser": "npm i karma-phantomjs-launcher && karma start",
        "test-node": "qunit-cli test/*.js",
        "weight": "npm run minify | gzip-size | pretty-bytes"
    },
    "version": "1.9.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
