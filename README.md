# npmdoc-jpm

#### api documentation for  [jpm (v1.3.1)](https://github.com/mozilla-jetpack/jpm)  [![npm package](https://img.shields.io/npm/v/npmdoc-jpm.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jpm) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jpm.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jpm)

#### Jetpack Mechanic utilities for creating, testing, running and packaging Mozilla Jetpack Addons

[![NPM](https://nodei.co/npm/jpm.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jpm)

- [https://npmdoc.github.io/node-npmdoc-jpm/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jpm/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jpm/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jpm/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jpm/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jpm/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "jpm",
    "version": "1.3.1",
    "description": "Jetpack Mechanic utilities for creating, testing, running and packaging Mozilla Jetpack Addons",
    "main": "index.js",
    "bin": {
        "jpm": "./bin/jpm"
    },
    "engines": {
        "node": ">=0.10",
        "npm": ">=3.0.0"
    },
    "scripts": {
        "addons": "node ./test/run.js addons",
        "functional": "node ./test/run.js functional",
        "addon_runners": "node ./test/run.js addon_runners",
        "unit": "node ./test/run.js unit",
        "documentation": "mocha -t 5000 test/documentation",
        "lint": "eslint bin/jpm lib test",
        "test": "node ./test/run.js",
        "prepush": "npm run lint && npm run documentation",
        "changelog": "conventional-changelog -p angular -u",
        "changelog-lint": "conventional-changelog-lint --from master",
        "get-unbranded-firefox": "get-firefox -ecb unbranded-release"
    },
    "homepage": "https://github.com/mozilla-jetpack/jpm",
    "repository": {
        "type": "git",
        "url": "git://github.com/mozilla-jetpack/jpm.git"
    },
    "bugs": {
        "url": "http://github.com/mozilla-jetpack/jpm/issues"
    },
    "keywords": [
        "firefox",
        "mozilla",
        "jetpack",
        "jpm"
    ],
    "dependencies": {
        "commander": "2.9.0",
        "decompress-zip": "0.3.0",
        "firefox-profile": "0.4.0",
        "fs-extra": "0.30.0",
        "fs-promise": "0.3.1",
        "fx-runner": "1.0.5",
        "jetpack-id": "0.0.4",
        "jetpack-validation": "0.0.7",
        "jpm-core": "0.0.11",
        "jsontoxml": "0.0.11",
        "lodash": "4.11.1",
        "minimatch": "3.0.2",
        "mozilla-toolkit-versioning": "0.0.2",
        "mozilla-version-comparator": "1.0.2",
        "node-watch": "0.3.4",
        "object-assign": "4.1.0",
        "open": "0.0.5",
        "promzard": "0.3.0",
        "read": "1.0.7",
        "semver": "5.1.0",
        "sign-addon": "0.2.0",
        "tmp": "0.0.28",
        "when": "3.7.2",
        "xml2js": "0.4.16",
        "zip-dir": "1.0.2",
        "jszip": "2.4.0"
    },
    "devDependencies": {
        "async": "1.5.0",
        "chai": "3.4.1",
        "conventional-changelog-cli": "1.2.0",
        "conventional-changelog-lint": "1.0.0",
        "dive": "0.4.0",
        "eslint": "3.5.0",
        "eslint-plugin-dependencies": "1.3.0",
        "get-firefox": "1.5.0",
        "glob": "5.0.3",
        "husky": "^0.10.1",
        "mocha": "2.5.3",
        "release-it": "2.3.1",
        "rimraf": "2.3.2",
        "teacher": "0.0.1",
        "xmldom": "0.1.19"
    },
    "author": "Jordan Santell",
    "license": "MPL-2.0",
    "locales": {
        "es": {
            "description": "Utilidades Mecánico Jetpack para crear, probar, ejecutar y empacar Mozilla Jetpack Addons"
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
