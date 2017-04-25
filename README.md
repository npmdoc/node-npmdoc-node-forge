# npmdoc-node-forge

#### basic api documentation for  [node-forge (v0.7.1)](https://github.com/digitalbazaar/forge)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-forge.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-forge) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-forge.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-forge)

#### JavaScript implementations of network transports, cryptography, ciphers, PKI, message digests, and various utilities.

[![NPM](https://nodei.co/npm/node-forge.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-forge)

- [https://npmdoc.github.io/node-npmdoc-node-forge/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-forge/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-forge/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-forge/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-forge/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-forge/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Digital Bazaar, Inc.",
        "url": "http://digitalbazaar.com/"
    },
    "browser": {
        "buffer": false,
        "crypto": false,
        "process": false
    },
    "bugs": {
        "url": "https://github.com/digitalbazaar/forge/issues"
    },
    "contributors": [
        {
            "name": "Dave Longley"
        },
        {
            "name": "David I. Lehn"
        },
        {
            "name": "Stefan Siegl"
        },
        {
            "name": "Christoph Dorn"
        }
    ],
    "dependencies": {},
    "description": "JavaScript implementations of network transports, cryptography, ciphers, PKI, message digests, and various utilities.",
    "devDependencies": {
        "browserify": "^13.1.1",
        "commander": "^2.9.0",
        "express": "^4.14.1",
        "istanbul": "^0.4.5",
        "jscs": "^3.0.7",
        "jshint": "^2.9.4",
        "karma": "^1.4.1",
        "karma-browserify": "^5.1.1",
        "karma-chrome-launcher": "^2.0.0",
        "karma-edge-launcher": "^0.2.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-ie-launcher": "^1.0.0",
        "karma-mocha": "^1.3.0",
        "karma-mocha-reporter": "^2.2.2",
        "karma-phantomjs-launcher": "^1.0.2",
        "karma-safari-launcher": "^1.0.0",
        "karma-sauce-launcher": "^1.1.0",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-tap-reporter": "0.0.6",
        "karma-webpack": "^2.0.2",
        "mocha": "^3.2.0",
        "mocha-lcov-reporter": "^1.2.0",
        "nodejs-websocket": "^1.7.1",
        "opts": "^1.2.2",
        "webpack": "^2.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "9da611ea08982f4b94206b3beb4cc9665f20c300",
        "tarball": "https://registry.npmjs.org/node-forge/-/node-forge-0.7.1.tgz"
    },
    "engines": {
        "node": "*"
    },
    "files": [
        "lib/*.js",
        "flash/swf/*.swf",
        "dist/*.min.js",
        "dist/*.min.js.map"
    ],
    "gitHead": "11e0cdccf190ff74e2b38d7fff06afebda29f5f5",
    "homepage": "https://github.com/digitalbazaar/forge",
    "jspm": {
        "format": "amd"
    },
    "keywords": [
        "aes",
        "asn",
        "asn.1",
        "cbc",
        "crypto",
        "cryptography",
        "csr",
        "des",
        "gcm",
        "hmac",
        "http",
        "https",
        "md5",
        "network",
        "pkcs",
        "pki",
        "prng",
        "rc2",
        "rsa",
        "sha1",
        "sha256",
        "sha384",
        "sha512",
        "ssh",
        "tls",
        "x.509",
        "x509"
    ],
    "license": "(BSD-3-Clause OR GPL-2.0)",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "davidlehn"
        },
        {
            "name": "dlongley"
        },
        {
            "name": "msporny"
        }
    ],
    "name": "node-forge",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/digitalbazaar/forge.git"
    },
    "scripts": {
        "_jscs": "jscs *.js lib/*.js tests/*.js tests/unit/*.js tests/legacy/*.js tests/issues/*.js tests/websockets/*.js",
        "_jshint": "jshint *.js lib/*.js tests/*.js tests/unit/*.js tests/legacy/*.js tests/issues/*.js tests/websockets/*.js",
        "build": "webpack",
        "coverage": "rm -rf coverage && ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha -- -u exports -t 30000 -R spec tests/unit/index.js",
        "coverage-lcov": "rm -rf coverage && ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha --report lcovonly -- -u exports -t 30000 -R spec tests/unit/index.js",
        "coverage-report": "istanbul report",
        "jscs": "jscs *.js lib/*.js tests/*.js tests/unit/*.js tests/legacy/*.js tests/issues/*.js tests/websockets/*.js",
        "jshint": "jshint *.js lib/*.js tests/unit/*.js tests/legacy/*.js tests/issues/*.js tests/websockets/*.js",
        "prepublish": "npm run build",
        "test": "mocha -t 30000 -R spec tests/unit/index.js",
        "test-build": "webpack --config webpack-tests.config.js",
        "test-karma": "karma start",
        "test-karma-sauce": "karma start karma-sauce.conf",
        "test-server": "node tests/server.js",
        "test-server-webid": "node tests/websockets/server-webid.js",
        "test-server-ws": "node tests/websockets/server-ws.js"
    },
    "version": "0.7.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
