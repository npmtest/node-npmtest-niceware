# npmtest-niceware

#### basic test coverage for  [niceware (v1.0.4)](http://www.github.com/diracdeltas/niceware)  [![npm package](https://img.shields.io/npm/v/npmtest-niceware.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-niceware) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-niceware.svg)](https://travis-ci.org/npmtest/node-npmtest-niceware)

#### Utility for generating memorable passwords and converting random bytes into human-readable phrases

[![NPM](https://nodei.co/npm/niceware.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/niceware)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-niceware/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-niceware/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-niceware/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-niceware/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-niceware/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-niceware/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-niceware/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-niceware/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-niceware/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-niceware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-niceware/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-niceware/build/test-report.html](https://npmtest.github.io/node-npmtest-niceware/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-niceware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-niceware/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-niceware/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-niceware/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-niceware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-niceware/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-niceware/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-niceware/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "niceware",
    "version": "1.0.4",
    "description": "Utility for generating memorable passwords and converting random bytes into human-readable phrases",
    "keywords": [
        "diceware",
        "passphrase",
        "password",
        "generator",
        "password generator",
        "dictionary",
        "crypto",
        "cryptography",
        "random",
        "entropy",
        "encryption"
    ],
    "homepage": "http://www.github.com/diracdeltas/niceware",
    "main": "lib/main.js",
    "devDependencies": {
        "browserify": "^13.1.1",
        "coveralls": "^2.11.15",
        "flow-bin": "^0.35.0",
        "istanbul": "^0.4.5",
        "jsdoc-to-markdown": "^2.0.1",
        "nsp": "^2.6.2",
        "standard": "^8.1.0",
        "tape": "^4.6.3"
    },
    "scripts": {
        "browsertest": "browserify test/*.js > testbundle.js && python -m SimpleHTTPServer",
        "build": "browserify lib/main.js -o browser/niceware.js",
        "check": "nsp check",
        "coverage": "istanbul cover tape test/**/*.js --report lcovonly -- -R spec",
        "lint": "standard",
        "jsdoc": "jsdoc2md lib/main.js > docs/api.md",
        "flow": "flow; test $? -eq 0 -o $? -eq 2",
        "test": "tape test/**/*.js"
    },
    "standard": {
        "ignore": [
            "lib/wordlist.js",
            "browser/niceware.js"
        ]
    },
    "author": "yan <yan@mit.edu>",
    "repository": {
        "type": "git",
        "url": "git://github.com/diracdeltas/niceware.git"
    },
    "license": "MIT",
    "dependencies": {
        "binary-search": "^1.3.2",
        "randombytes": "^2.0.3"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
