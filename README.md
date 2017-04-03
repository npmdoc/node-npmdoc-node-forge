# api documentation for  [node-forge (v0.7.1)](https://github.com/digitalbazaar/forge)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-forge.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-forge) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-forge.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-forge)
#### JavaScript implementations of network transports, cryptography, ciphers, PKI, message digests, and various utilities.

[![NPM](https://nodei.co/npm/node-forge.png?downloads=true)](https://www.npmjs.com/package/node-forge)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-forge/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-forge_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-forge/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-forge/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-forge/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Digital Bazaar, Inc.",
        "email": "support@digitalbazaar.com",
        "url": "http://digitalbazaar.com/"
    },
    "browser": {
        "buffer": false,
        "crypto": false,
        "process": false
    },
    "bugs": {
        "url": "https://github.com/digitalbazaar/forge/issues",
        "email": "support@digitalbazaar.com"
    },
    "contributors": [
        {
            "name": "Dave Longley",
            "email": "dlongley@digitalbazaar.com"
        },
        {
            "name": "David I. Lehn",
            "email": "dlehn@digitalbazaar.com"
        },
        {
            "name": "Stefan Siegl",
            "email": "stesie@brokenpipe.de"
        },
        {
            "name": "Christoph Dorn",
            "email": "christoph@christophdorn.com"
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
            "name": "davidlehn",
            "email": "dil@lehn.org"
        },
        {
            "name": "dlongley",
            "email": "dlongley@digitalbazaar.com"
        },
        {
            "name": "msporny",
            "email": "msporny@digitalbazaar.com"
        }
    ],
    "name": "node-forge",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "0.7.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-forge](#apidoc.module.node-forge)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>aes.Algorithm (name, mode)](#apidoc.element.node-forge.aes.Algorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>cipher.BlockCipher (options)](#apidoc.element.node-forge.cipher.BlockCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>des.Algorithm (name, mode)](#apidoc.element.node-forge.des.Algorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>jsbn.BigInteger (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>pbkdf2 ( p, s, c, dkLen, md, callback)](#apidoc.element.node-forge.pbkdf2)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>util.ByteBuffer (b)](#apidoc.element.node-forge.util.ByteBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.</span>util.DataBuffer (b, options)](#apidoc.element.node-forge.util.DataBuffer)
1.  object <span class="apidocSignatureSpan">node-forge.</span>aes
1.  object <span class="apidocSignatureSpan">node-forge.</span>aes.Algorithm.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>asn1
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.BlockCipher.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.algorithms
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes.cbc.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes.cfb.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes.ctr.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes.ecb.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes.gcm.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>cipher.modes.ofb.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>debug
1.  object <span class="apidocSignatureSpan">node-forge.</span>des
1.  object <span class="apidocSignatureSpan">node-forge.</span>des.Algorithm.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>form
1.  object <span class="apidocSignatureSpan">node-forge.</span>hmac
1.  object <span class="apidocSignatureSpan">node-forge.</span>http
1.  object <span class="apidocSignatureSpan">node-forge.</span>jsbn
1.  object <span class="apidocSignatureSpan">node-forge.</span>jsbn.BigInteger.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>kem
1.  object <span class="apidocSignatureSpan">node-forge.</span>kem.rsa
1.  object <span class="apidocSignatureSpan">node-forge.</span>log
1.  object <span class="apidocSignatureSpan">node-forge.</span>log.consoleLogger
1.  object <span class="apidocSignatureSpan">node-forge.</span>md
1.  object <span class="apidocSignatureSpan">node-forge.</span>md5
1.  object <span class="apidocSignatureSpan">node-forge.</span>mgf
1.  object <span class="apidocSignatureSpan">node-forge.</span>mgf1
1.  object <span class="apidocSignatureSpan">node-forge.</span>net
1.  object <span class="apidocSignatureSpan">node-forge.</span>oids
1.  object <span class="apidocSignatureSpan">node-forge.</span>options
1.  object <span class="apidocSignatureSpan">node-forge.</span>pbe
1.  object <span class="apidocSignatureSpan">node-forge.</span>pem
1.  object <span class="apidocSignatureSpan">node-forge.</span>pkcs1
1.  object <span class="apidocSignatureSpan">node-forge.</span>pkcs12
1.  object <span class="apidocSignatureSpan">node-forge.</span>pkcs5
1.  object <span class="apidocSignatureSpan">node-forge.</span>pkcs7
1.  object <span class="apidocSignatureSpan">node-forge.</span>pkcs7asn1
1.  object <span class="apidocSignatureSpan">node-forge.</span>pki
1.  object <span class="apidocSignatureSpan">node-forge.</span>prime
1.  object <span class="apidocSignatureSpan">node-forge.</span>prng
1.  object <span class="apidocSignatureSpan">node-forge.</span>pss
1.  object <span class="apidocSignatureSpan">node-forge.</span>random
1.  object <span class="apidocSignatureSpan">node-forge.</span>random.plugin
1.  object <span class="apidocSignatureSpan">node-forge.</span>rc2
1.  object <span class="apidocSignatureSpan">node-forge.</span>rsa
1.  object <span class="apidocSignatureSpan">node-forge.</span>sha1
1.  object <span class="apidocSignatureSpan">node-forge.</span>sha256
1.  object <span class="apidocSignatureSpan">node-forge.</span>sha384
1.  object <span class="apidocSignatureSpan">node-forge.</span>sha512
1.  object <span class="apidocSignatureSpan">node-forge.</span>sha512.sha224
1.  object <span class="apidocSignatureSpan">node-forge.</span>sha512.sha256
1.  object <span class="apidocSignatureSpan">node-forge.</span>ssh
1.  object <span class="apidocSignatureSpan">node-forge.</span>task
1.  object <span class="apidocSignatureSpan">node-forge.</span>tls
1.  object <span class="apidocSignatureSpan">node-forge.</span>util
1.  object <span class="apidocSignatureSpan">node-forge.</span>util.ByteBuffer.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>util.DataBuffer.prototype
1.  object <span class="apidocSignatureSpan">node-forge.</span>xhr

#### [module node-forge.aes](#apidoc.module.node-forge.aes)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>Algorithm (name, mode)](#apidoc.element.node-forge.aes.Algorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>_expandKey (key, decrypt)](#apidoc.element.node-forge.aes._expandKey)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>_updateBlock (w, input, output, decrypt)](#apidoc.element.node-forge.aes._updateBlock)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>createDecryptionCipher (key, mode)](#apidoc.element.node-forge.aes.createDecryptionCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>createEncryptionCipher (key, mode)](#apidoc.element.node-forge.aes.createEncryptionCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>startDecrypting (key, iv, output, mode)](#apidoc.element.node-forge.aes.startDecrypting)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>startEncrypting (key, iv, output, mode)](#apidoc.element.node-forge.aes.startEncrypting)

#### [module node-forge.aes.Algorithm](#apidoc.module.node-forge.aes.Algorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.</span>Algorithm (name, mode)](#apidoc.element.node-forge.aes.Algorithm.Algorithm)

#### [module node-forge.aes.Algorithm.prototype](#apidoc.module.node-forge.aes.Algorithm.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.aes.Algorithm.prototype.</span>initialize (options)](#apidoc.element.node-forge.aes.Algorithm.prototype.initialize)

#### [module node-forge.asn1](#apidoc.module.node-forge.asn1)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>copy (obj, options)](#apidoc.element.node-forge.asn1.copy)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>create (tagClass, type, constructed, value, options)](#apidoc.element.node-forge.asn1.create)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>dateToGeneralizedTime (date)](#apidoc.element.node-forge.asn1.dateToGeneralizedTime)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>dateToUtcTime (date)](#apidoc.element.node-forge.asn1.dateToUtcTime)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>derToInteger (bytes)](#apidoc.element.node-forge.asn1.derToInteger)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>derToOid (bytes)](#apidoc.element.node-forge.asn1.derToOid)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>equals (obj1, obj2, options)](#apidoc.element.node-forge.asn1.equals)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>fromDer (bytes, options)](#apidoc.element.node-forge.asn1.fromDer)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>generalizedTimeToDate (gentime)](#apidoc.element.node-forge.asn1.generalizedTimeToDate)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>getBerValueLength (b)](#apidoc.element.node-forge.asn1.getBerValueLength)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>integerToDer (x)](#apidoc.element.node-forge.asn1.integerToDer)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>oidToDer (oid)](#apidoc.element.node-forge.asn1.oidToDer)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>prettyPrint (obj, level, indentation)](#apidoc.element.node-forge.asn1.prettyPrint)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>toDer (obj)](#apidoc.element.node-forge.asn1.toDer)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>utcTimeToDate (utc)](#apidoc.element.node-forge.asn1.utcTimeToDate)
1.  [function <span class="apidocSignatureSpan">node-forge.asn1.</span>validate (obj, v, capture, errors)](#apidoc.element.node-forge.asn1.validate)
1.  object <span class="apidocSignatureSpan">node-forge.asn1.</span>Class
1.  object <span class="apidocSignatureSpan">node-forge.asn1.</span>Type

#### [module node-forge.cipher](#apidoc.module.node-forge.cipher)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.</span>BlockCipher (options)](#apidoc.element.node-forge.cipher.BlockCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.</span>createCipher (algorithm, key)](#apidoc.element.node-forge.cipher.createCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.</span>createDecipher (algorithm, key)](#apidoc.element.node-forge.cipher.createDecipher)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.</span>getAlgorithm (name)](#apidoc.element.node-forge.cipher.getAlgorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.</span>registerAlgorithm (name, algorithm)](#apidoc.element.node-forge.cipher.registerAlgorithm)
1.  object <span class="apidocSignatureSpan">node-forge.cipher.</span>algorithms
1.  object <span class="apidocSignatureSpan">node-forge.cipher.</span>modes

#### [module node-forge.cipher.BlockCipher](#apidoc.module.node-forge.cipher.BlockCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.</span>BlockCipher (options)](#apidoc.element.node-forge.cipher.BlockCipher.BlockCipher)

#### [module node-forge.cipher.BlockCipher.prototype](#apidoc.module.node-forge.cipher.BlockCipher.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.BlockCipher.prototype.</span>finish (pad)](#apidoc.element.node-forge.cipher.BlockCipher.prototype.finish)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.BlockCipher.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.BlockCipher.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.BlockCipher.prototype.</span>update (input)](#apidoc.element.node-forge.cipher.BlockCipher.prototype.update)

#### [module node-forge.cipher.algorithms](#apidoc.module.node-forge.cipher.algorithms)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-CBC ()](#apidoc.element.node-forge.cipher.algorithms.3DES-CBC)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-CFB ()](#apidoc.element.node-forge.cipher.algorithms.3DES-CFB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-CTR ()](#apidoc.element.node-forge.cipher.algorithms.3DES-CTR)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-ECB ()](#apidoc.element.node-forge.cipher.algorithms.3DES-ECB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-OFB ()](#apidoc.element.node-forge.cipher.algorithms.3DES-OFB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-CBC ()](#apidoc.element.node-forge.cipher.algorithms.AES-CBC)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-CFB ()](#apidoc.element.node-forge.cipher.algorithms.AES-CFB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-CTR ()](#apidoc.element.node-forge.cipher.algorithms.AES-CTR)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-ECB ()](#apidoc.element.node-forge.cipher.algorithms.AES-ECB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-GCM ()](#apidoc.element.node-forge.cipher.algorithms.AES-GCM)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-OFB ()](#apidoc.element.node-forge.cipher.algorithms.AES-OFB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-CBC ()](#apidoc.element.node-forge.cipher.algorithms.DES-CBC)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-CFB ()](#apidoc.element.node-forge.cipher.algorithms.DES-CFB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-CTR ()](#apidoc.element.node-forge.cipher.algorithms.DES-CTR)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-ECB ()](#apidoc.element.node-forge.cipher.algorithms.DES-ECB)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-OFB ()](#apidoc.element.node-forge.cipher.algorithms.DES-OFB)

#### [module node-forge.cipher.modes](#apidoc.module.node-forge.cipher.modes)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>cbc (options)](#apidoc.element.node-forge.cipher.modes.cbc)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>cfb (options)](#apidoc.element.node-forge.cipher.modes.cfb)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>ctr (options)](#apidoc.element.node-forge.cipher.modes.ctr)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>ecb (options)](#apidoc.element.node-forge.cipher.modes.ecb)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>gcm (options)](#apidoc.element.node-forge.cipher.modes.gcm)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>ofb (options)](#apidoc.element.node-forge.cipher.modes.ofb)

#### [module node-forge.cipher.modes.cbc.prototype](#apidoc.module.node-forge.cipher.modes.cbc.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>pad (input, options)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.pad)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>unpad (output, options)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.unpad)

#### [module node-forge.cipher.modes.cfb.prototype](#apidoc.module.node-forge.cipher.modes.cfb.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cfb.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cfb.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cfb.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cfb.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.cfb.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.cfb.prototype.start)

#### [module node-forge.cipher.modes.ctr.prototype](#apidoc.module.node-forge.cipher.modes.ctr.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ctr.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ctr.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ctr.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ctr.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ctr.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.ctr.prototype.start)

#### [module node-forge.cipher.modes.ecb.prototype](#apidoc.module.node-forge.cipher.modes.ecb.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>pad (input, options)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.pad)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>unpad (output, options)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.unpad)

#### [module node-forge.cipher.modes.gcm.prototype](#apidoc.module.node-forge.cipher.modes.gcm.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>afterFinish (output, options)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.afterFinish)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>generateHashTable (h, bits)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.generateHashTable)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>generateSubHashTable (mid, bits)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.generateSubHashTable)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>ghash (h, y, x)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.ghash)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>multiply (x, y)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>pow (x, out)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.pow)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>tableMultiply (x)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.tableMultiply)

#### [module node-forge.cipher.modes.ofb.prototype](#apidoc.module.node-forge.cipher.modes.ofb.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ofb.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ofb.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ofb.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ofb.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.cipher.modes.ofb.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.ofb.prototype.start)

#### [module node-forge.debug](#apidoc.module.node-forge.debug)
1.  [function <span class="apidocSignatureSpan">node-forge.debug.</span>clear (cat, name)](#apidoc.element.node-forge.debug.clear)
1.  [function <span class="apidocSignatureSpan">node-forge.debug.</span>get (cat, name)](#apidoc.element.node-forge.debug.get)
1.  [function <span class="apidocSignatureSpan">node-forge.debug.</span>set (cat, name, data)](#apidoc.element.node-forge.debug.set)
1.  object <span class="apidocSignatureSpan">node-forge.debug.</span>storage

#### [module node-forge.des](#apidoc.module.node-forge.des)
1.  [function <span class="apidocSignatureSpan">node-forge.des.</span>Algorithm (name, mode)](#apidoc.element.node-forge.des.Algorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.des.</span>createDecryptionCipher (key, mode)](#apidoc.element.node-forge.des.createDecryptionCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.des.</span>createEncryptionCipher (key, mode)](#apidoc.element.node-forge.des.createEncryptionCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.des.</span>startDecrypting (key, iv, output, mode)](#apidoc.element.node-forge.des.startDecrypting)
1.  [function <span class="apidocSignatureSpan">node-forge.des.</span>startEncrypting (key, iv, output, mode)](#apidoc.element.node-forge.des.startEncrypting)

#### [module node-forge.des.Algorithm](#apidoc.module.node-forge.des.Algorithm)
1.  [function <span class="apidocSignatureSpan">node-forge.des.</span>Algorithm (name, mode)](#apidoc.element.node-forge.des.Algorithm.Algorithm)

#### [module node-forge.des.Algorithm.prototype](#apidoc.module.node-forge.des.Algorithm.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.des.Algorithm.prototype.</span>initialize (options)](#apidoc.element.node-forge.des.Algorithm.prototype.initialize)

#### [module node-forge.hmac](#apidoc.module.node-forge.hmac)
1.  [function <span class="apidocSignatureSpan">node-forge.hmac.</span>create ()](#apidoc.element.node-forge.hmac.create)

#### [module node-forge.http](#apidoc.module.node-forge.http)
1.  [function <span class="apidocSignatureSpan">node-forge.http.</span>createClient (options)](#apidoc.element.node-forge.http.createClient)
1.  [function <span class="apidocSignatureSpan">node-forge.http.</span>createRequest (options)](#apidoc.element.node-forge.http.createRequest)
1.  [function <span class="apidocSignatureSpan">node-forge.http.</span>createResponse ()](#apidoc.element.node-forge.http.createResponse)
1.  [function <span class="apidocSignatureSpan">node-forge.http.</span>parseUrl (str)](#apidoc.element.node-forge.http.parseUrl)
1.  [function <span class="apidocSignatureSpan">node-forge.http.</span>withinCookieDomain (url, cookie)](#apidoc.element.node-forge.http.withinCookieDomain)

#### [module node-forge.jsbn](#apidoc.module.node-forge.jsbn)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.</span>BigInteger (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger)

#### [module node-forge.jsbn.BigInteger](#apidoc.module.node-forge.jsbn.BigInteger)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.</span>BigInteger (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger.BigInteger)
1.  object <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.</span>ONE
1.  object <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.</span>ZERO

#### [module node-forge.jsbn.BigInteger.prototype](#apidoc.module.node-forge.jsbn.BigInteger.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>abs ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.abs)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>add (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.add)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>addTo (a, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.addTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>am (i, x, w, j, c, n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.am)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>and (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.and)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>andNot (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.andNot)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>bitCount ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.bitCount)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>bitLength ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.bitLength)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>bitwiseTo (a, op, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.bitwiseTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>byteValue ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.byteValue)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>changeBit (n, op)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.changeBit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>chunkSize (r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.chunkSize)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>clamp ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.clamp)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>clearBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.clearBit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>clone ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.clone)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>compareTo (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.compareTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>copyTo (r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.copyTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>dAddOffset (n, w)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.dAddOffset)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>dMultiply (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.dMultiply)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>divRemTo (m, q, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.divRemTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>divide (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.divide)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>divideAndRemainder (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.divideAndRemainder)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>dlShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.dlShiftTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>drShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.drShiftTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>equals (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.equals)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>exp (e, z)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.exp)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>flipBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.flipBit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromInt (x)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromInt)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromNumber (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromNumber)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromRadix (s, b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromRadix)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromString (s, b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromString)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>gcd (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.gcd)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>getLowestSetBit ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.getLowestSetBit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>intValue ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.intValue)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>invDigit ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.invDigit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>isEven ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.isEven)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>isProbablePrime (t)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.isProbablePrime)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>lShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.lShiftTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>max (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.max)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>millerRabin (t)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.millerRabin)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>min (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.min)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>mod (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.mod)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modInt (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modInt)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modInverse (m)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modInverse)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modPow (e, m)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modPow)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modPowInt (e, m)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modPowInt)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiply (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiplyLowerTo (a, n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyLowerTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiplyTo (a, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiplyUpperTo (a, n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyUpperTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>negate ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.negate)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>not ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.not)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>or (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.or)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>pow (e)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.pow)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>rShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.rShiftTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>remainder (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.remainder)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>setBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.setBit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>shiftLeft (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.shiftLeft)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>shiftRight (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.shiftRight)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>shortValue ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.shortValue)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>signum ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.signum)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>squareTo (r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.squareTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>subTo (a, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.subTo)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>subtract (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>testBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.testBit)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>toByteArray ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.toByteArray)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>toRadix (b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.toRadix)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>toString (b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.toString)
1.  [function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>xor (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.xor)
1.  number <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>DB
1.  number <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>DM
1.  number <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>DV
1.  number <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>F1
1.  number <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>F2
1.  number <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>FV

#### [module node-forge.kem](#apidoc.module.node-forge.kem)
1.  [function <span class="apidocSignatureSpan">node-forge.kem.</span>kdf1 (md, digestLength)](#apidoc.element.node-forge.kem.kdf1)
1.  [function <span class="apidocSignatureSpan">node-forge.kem.</span>kdf2 (md, digestLength)](#apidoc.element.node-forge.kem.kdf2)
1.  object <span class="apidocSignatureSpan">node-forge.kem.</span>rsa

#### [module node-forge.kem.rsa](#apidoc.module.node-forge.kem.rsa)
1.  [function <span class="apidocSignatureSpan">node-forge.kem.rsa.</span>create (kdf, options)](#apidoc.element.node-forge.kem.rsa.create)

#### [module node-forge.log](#apidoc.module.node-forge.log)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>addLogger (logger)](#apidoc.element.node-forge.log.addLogger)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>debug (category, message)](#apidoc.element.node-forge.log.debug)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>error (category, message)](#apidoc.element.node-forge.log.error)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>info (category, message)](#apidoc.element.node-forge.log.info)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>lock (logger, lock)](#apidoc.element.node-forge.log.lock)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>logMessage (message)](#apidoc.element.node-forge.log.logMessage)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>makeLogger (logFunction)](#apidoc.element.node-forge.log.makeLogger)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>prepareFull (message)](#apidoc.element.node-forge.log.prepareFull)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>prepareStandard (message)](#apidoc.element.node-forge.log.prepareStandard)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>prepareStandardFull (message)](#apidoc.element.node-forge.log.prepareStandardFull)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>setLevel (logger, level)](#apidoc.element.node-forge.log.setLevel)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>verbose (category, message)](#apidoc.element.node-forge.log.verbose)
1.  [function <span class="apidocSignatureSpan">node-forge.log.</span>warning (category, message)](#apidoc.element.node-forge.log.warning)
1.  number <span class="apidocSignatureSpan">node-forge.log.</span>INTERPOLATE
1.  number <span class="apidocSignatureSpan">node-forge.log.</span>LEVEL_LOCKED
1.  number <span class="apidocSignatureSpan">node-forge.log.</span>NO_LEVEL_CHECK
1.  object <span class="apidocSignatureSpan">node-forge.log.</span>consoleLogger
1.  object <span class="apidocSignatureSpan">node-forge.log.</span>levels

#### [module node-forge.log.consoleLogger](#apidoc.module.node-forge.log.consoleLogger)
1.  [function <span class="apidocSignatureSpan">node-forge.log.consoleLogger.</span>f (logger, message)](#apidoc.element.node-forge.log.consoleLogger.f)
1.  number <span class="apidocSignatureSpan">node-forge.log.consoleLogger.</span>flags
1.  string <span class="apidocSignatureSpan">node-forge.log.consoleLogger.</span>level

#### [module node-forge.md5](#apidoc.module.node-forge.md5)
1.  [function <span class="apidocSignatureSpan">node-forge.md5.</span>create ()](#apidoc.element.node-forge.md5.create)

#### [module node-forge.mgf1](#apidoc.module.node-forge.mgf1)
1.  [function <span class="apidocSignatureSpan">node-forge.mgf1.</span>create (md)](#apidoc.element.node-forge.mgf1.create)

#### [module node-forge.net](#apidoc.module.node-forge.net)
1.  [function <span class="apidocSignatureSpan">node-forge.net.</span>createSocket (options)](#apidoc.element.node-forge.net.createSocket)
1.  [function <span class="apidocSignatureSpan">node-forge.net.</span>createSocketPool (options)](#apidoc.element.node-forge.net.createSocketPool)
1.  [function <span class="apidocSignatureSpan">node-forge.net.</span>destroySocketPool (options)](#apidoc.element.node-forge.net.destroySocketPool)
1.  object <span class="apidocSignatureSpan">node-forge.net.</span>socketPools

#### [module node-forge.pbe](#apidoc.module.node-forge.pbe)
1.  [function <span class="apidocSignatureSpan">node-forge.pbe.</span>generatePkcs12Key (password, salt, id, iter, n, md)](#apidoc.element.node-forge.pbe.generatePkcs12Key)
1.  [function <span class="apidocSignatureSpan">node-forge.pbe.</span>getCipher (oid, params, password)](#apidoc.element.node-forge.pbe.getCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.pbe.</span>getCipherForPBES2 (oid, params, password)](#apidoc.element.node-forge.pbe.getCipherForPBES2)
1.  [function <span class="apidocSignatureSpan">node-forge.pbe.</span>getCipherForPKCS12PBE (oid, params, password)](#apidoc.element.node-forge.pbe.getCipherForPKCS12PBE)
1.  [function <span class="apidocSignatureSpan">node-forge.pbe.</span>opensslDeriveBytes (password, salt, dkLen, md)](#apidoc.element.node-forge.pbe.opensslDeriveBytes)

#### [module node-forge.pem](#apidoc.module.node-forge.pem)
1.  [function <span class="apidocSignatureSpan">node-forge.pem.</span>decode (str)](#apidoc.element.node-forge.pem.decode)
1.  [function <span class="apidocSignatureSpan">node-forge.pem.</span>encode (msg, options)](#apidoc.element.node-forge.pem.encode)

#### [module node-forge.pkcs1](#apidoc.module.node-forge.pkcs1)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs1.</span>decode_rsa_oaep (key, em, options)](#apidoc.element.node-forge.pkcs1.decode_rsa_oaep)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs1.</span>encode_rsa_oaep (key, message, options)](#apidoc.element.node-forge.pkcs1.encode_rsa_oaep)

#### [module node-forge.pkcs12](#apidoc.module.node-forge.pkcs12)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs12.</span>generateKey (password, salt, id, iter, n, md)](#apidoc.element.node-forge.pkcs12.generateKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs12.</span>pkcs12FromAsn1 (obj, strict, password)](#apidoc.element.node-forge.pkcs12.pkcs12FromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs12.</span>toPkcs12Asn1 (key, cert, password, options)](#apidoc.element.node-forge.pkcs12.toPkcs12Asn1)

#### [module node-forge.pkcs5](#apidoc.module.node-forge.pkcs5)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs5.</span>pbkdf2 ( p, s, c, dkLen, md, callback)](#apidoc.element.node-forge.pkcs5.pbkdf2)

#### [module node-forge.pkcs7](#apidoc.module.node-forge.pkcs7)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>createEncryptedData ()](#apidoc.element.node-forge.pkcs7.createEncryptedData)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>createEnvelopedData ()](#apidoc.element.node-forge.pkcs7.createEnvelopedData)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>createSignedData ()](#apidoc.element.node-forge.pkcs7.createSignedData)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>messageFromAsn1 (obj)](#apidoc.element.node-forge.pkcs7.messageFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>messageFromPem (pem)](#apidoc.element.node-forge.pkcs7.messageFromPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>messageToPem (msg, maxline)](#apidoc.element.node-forge.pkcs7.messageToPem)
1.  object <span class="apidocSignatureSpan">node-forge.pkcs7.</span>asn1

#### [module node-forge.pki](#apidoc.module.node-forge.pki)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>CRIAttributesAsArray (attributes)](#apidoc.element.node-forge.pki.CRIAttributesAsArray)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>RDNAttributesAsArray (rdn, md)](#apidoc.element.node-forge.pki.RDNAttributesAsArray)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionFromAsn1 (ext)](#apidoc.element.node-forge.pki.certificateExtensionFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionToAsn1 (ext)](#apidoc.element.node-forge.pki.certificateExtensionToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionsFromAsn1 (exts)](#apidoc.element.node-forge.pki.certificateExtensionsFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionsToAsn1 (exts)](#apidoc.element.node-forge.pki.certificateExtensionsToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateFromAsn1 (obj, computeHash)](#apidoc.element.node-forge.pki.certificateFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateFromPem (pem, computeHash, strict)](#apidoc.element.node-forge.pki.certificateFromPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateToAsn1 (cert)](#apidoc.element.node-forge.pki.certificateToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateToPem (cert, maxline)](#apidoc.element.node-forge.pki.certificateToPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestFromAsn1 (obj, computeHash)](#apidoc.element.node-forge.pki.certificationRequestFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestFromPem (pem, computeHash, strict)](#apidoc.element.node-forge.pki.certificationRequestFromPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestToAsn1 (csr)](#apidoc.element.node-forge.pki.certificationRequestToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestToPem (csr, maxline)](#apidoc.element.node-forge.pki.certificationRequestToPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>createCaStore (certs)](#apidoc.element.node-forge.pki.createCaStore)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>createCertificate ()](#apidoc.element.node-forge.pki.createCertificate)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>createCertificationRequest ()](#apidoc.element.node-forge.pki.createCertificationRequest)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>decryptPrivateKeyInfo (obj, password)](#apidoc.element.node-forge.pki.decryptPrivateKeyInfo)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>decryptRsaPrivateKey (pem, password)](#apidoc.element.node-forge.pki.decryptRsaPrivateKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>distinguishedNameToAsn1 (dn)](#apidoc.element.node-forge.pki.distinguishedNameToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptPrivateKeyInfo (obj, password, options)](#apidoc.element.node-forge.pki.encryptPrivateKeyInfo)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptRsaPrivateKey (rsaKey, password, options)](#apidoc.element.node-forge.pki.encryptRsaPrivateKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptedPrivateKeyFromPem (pem)](#apidoc.element.node-forge.pki.encryptedPrivateKeyFromPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptedPrivateKeyToPem (epki, maxline)](#apidoc.element.node-forge.pki.encryptedPrivateKeyToPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>getCertificationRequestInfo (csr)](#apidoc.element.node-forge.pki.getCertificationRequestInfo)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>getPublicKeyFingerprint (key, options)](#apidoc.element.node-forge.pki.getPublicKeyFingerprint)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>getTBSCertificate (cert)](#apidoc.element.node-forge.pki.getTBSCertificate)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>pemToDer (pem)](#apidoc.element.node-forge.pki.pemToDer)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyFromAsn1 (obj)](#apidoc.element.node-forge.pki.privateKeyFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyFromPem (pem)](#apidoc.element.node-forge.pki.privateKeyFromPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyInfoToPem (pki, maxline)](#apidoc.element.node-forge.pki.privateKeyInfoToPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyToAsn1 (key)](#apidoc.element.node-forge.pki.privateKeyToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyToPem (key, maxline)](#apidoc.element.node-forge.pki.privateKeyToPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyToRSAPrivateKey (key)](#apidoc.element.node-forge.pki.privateKeyToRSAPrivateKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyFromAsn1 (obj)](#apidoc.element.node-forge.pki.publicKeyFromAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyFromPem (pem)](#apidoc.element.node-forge.pki.publicKeyFromPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToAsn1 (key)](#apidoc.element.node-forge.pki.publicKeyToAsn1)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToPem (key, maxline)](#apidoc.element.node-forge.pki.publicKeyToPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToRSAPublicKey (key)](#apidoc.element.node-forge.pki.publicKeyToRSAPublicKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToRSAPublicKeyPem (key, maxline)](#apidoc.element.node-forge.pki.publicKeyToRSAPublicKeyPem)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToSubjectPublicKeyInfo (key)](#apidoc.element.node-forge.pki.publicKeyToSubjectPublicKeyInfo)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>setRsaPrivateKey ( n, e, d, p, q, dP, dQ, qInv)](#apidoc.element.node-forge.pki.setRsaPrivateKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>setRsaPublicKey (n, e)](#apidoc.element.node-forge.pki.setRsaPublicKey)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>verifyCertificateChain (caStore, chain, verify)](#apidoc.element.node-forge.pki.verifyCertificateChain)
1.  [function <span class="apidocSignatureSpan">node-forge.pki.</span>wrapRsaPrivateKey (rsaKey)](#apidoc.element.node-forge.pki.wrapRsaPrivateKey)
1.  object <span class="apidocSignatureSpan">node-forge.pki.</span>certificateError
1.  object <span class="apidocSignatureSpan">node-forge.pki.</span>oids
1.  object <span class="apidocSignatureSpan">node-forge.pki.</span>pbe
1.  object <span class="apidocSignatureSpan">node-forge.pki.</span>rsa

#### [module node-forge.prime](#apidoc.module.node-forge.prime)
1.  [function <span class="apidocSignatureSpan">node-forge.prime.</span>generateProbablePrime (bits, options, callback)](#apidoc.element.node-forge.prime.generateProbablePrime)

#### [module node-forge.prng](#apidoc.module.node-forge.prng)
1.  [function <span class="apidocSignatureSpan">node-forge.prng.</span>create (plugin)](#apidoc.element.node-forge.prng.create)

#### [module node-forge.pss](#apidoc.module.node-forge.pss)
1.  [function <span class="apidocSignatureSpan">node-forge.pss.</span>create (options)](#apidoc.element.node-forge.pss.create)

#### [module node-forge.random](#apidoc.module.node-forge.random)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>collect (bytes)](#apidoc.element.node-forge.random.collect)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>collectInt (i, n)](#apidoc.element.node-forge.random.collectInt)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>createInstance ()](#apidoc.element.node-forge.random.createInstance)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>generate (count, callback)](#apidoc.element.node-forge.random.generate)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>generateSync (count)](#apidoc.element.node-forge.random.generateSync)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>getBytes (count, callback)](#apidoc.element.node-forge.random.getBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>getBytesSync (count)](#apidoc.element.node-forge.random.getBytesSync)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>registerWorker (worker)](#apidoc.element.node-forge.random.registerWorker)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>seedFile (needed, callback)](#apidoc.element.node-forge.random.seedFile)
1.  [function <span class="apidocSignatureSpan">node-forge.random.</span>seedFileSync (needed)](#apidoc.element.node-forge.random.seedFileSync)
1.  number <span class="apidocSignatureSpan">node-forge.random.</span>generated
1.  number <span class="apidocSignatureSpan">node-forge.random.</span>pool
1.  number <span class="apidocSignatureSpan">node-forge.random.</span>reseeds
1.  object <span class="apidocSignatureSpan">node-forge.random.</span>key
1.  object <span class="apidocSignatureSpan">node-forge.random.</span>plugin
1.  object <span class="apidocSignatureSpan">node-forge.random.</span>pools
1.  object <span class="apidocSignatureSpan">node-forge.random.</span>seed
1.  object <span class="apidocSignatureSpan">node-forge.random.</span>time

#### [module node-forge.random.plugin](#apidoc.module.node-forge.random.plugin)
1.  [function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>cipher (key, seed)](#apidoc.element.node-forge.random.plugin.cipher)
1.  [function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>formatKey (key)](#apidoc.element.node-forge.random.plugin.formatKey)
1.  [function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>formatSeed (seed)](#apidoc.element.node-forge.random.plugin.formatSeed)
1.  [function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>increment (seed)](#apidoc.element.node-forge.random.plugin.increment)
1.  object <span class="apidocSignatureSpan">node-forge.random.plugin.</span>md

#### [module node-forge.rc2](#apidoc.module.node-forge.rc2)
1.  [function <span class="apidocSignatureSpan">node-forge.rc2.</span>createDecryptionCipher (key, bits)](#apidoc.element.node-forge.rc2.createDecryptionCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.rc2.</span>createEncryptionCipher (key, bits)](#apidoc.element.node-forge.rc2.createEncryptionCipher)
1.  [function <span class="apidocSignatureSpan">node-forge.rc2.</span>expandKey (key, effKeyBits)](#apidoc.element.node-forge.rc2.expandKey)
1.  [function <span class="apidocSignatureSpan">node-forge.rc2.</span>startDecrypting (key, iv, output)](#apidoc.element.node-forge.rc2.startDecrypting)
1.  [function <span class="apidocSignatureSpan">node-forge.rc2.</span>startEncrypting (key, iv, output)](#apidoc.element.node-forge.rc2.startEncrypting)

#### [module node-forge.rsa](#apidoc.module.node-forge.rsa)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>createKeyPairGenerationState (bits, e, options)](#apidoc.element.node-forge.rsa.createKeyPairGenerationState)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>decrypt (ed, key, pub, ml)](#apidoc.element.node-forge.rsa.decrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>encrypt (m, key, bt)](#apidoc.element.node-forge.rsa.encrypt)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>generateKeyPair (bits, e, options, callback)](#apidoc.element.node-forge.rsa.generateKeyPair)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>setPrivateKey ( n, e, d, p, q, dP, dQ, qInv)](#apidoc.element.node-forge.rsa.setPrivateKey)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>setPublicKey (n, e)](#apidoc.element.node-forge.rsa.setPublicKey)
1.  [function <span class="apidocSignatureSpan">node-forge.rsa.</span>stepKeyPairGenerationState (state, n)](#apidoc.element.node-forge.rsa.stepKeyPairGenerationState)
1.  object <span class="apidocSignatureSpan">node-forge.rsa.</span>publicKeyValidator

#### [module node-forge.sha1](#apidoc.module.node-forge.sha1)
1.  [function <span class="apidocSignatureSpan">node-forge.sha1.</span>create ()](#apidoc.element.node-forge.sha1.create)

#### [module node-forge.sha256](#apidoc.module.node-forge.sha256)
1.  [function <span class="apidocSignatureSpan">node-forge.sha256.</span>create ()](#apidoc.element.node-forge.sha256.create)

#### [module node-forge.sha384](#apidoc.module.node-forge.sha384)
1.  [function <span class="apidocSignatureSpan">node-forge.sha384.</span>create ()](#apidoc.element.node-forge.sha384.create)

#### [module node-forge.sha512](#apidoc.module.node-forge.sha512)
1.  [function <span class="apidocSignatureSpan">node-forge.sha512.</span>create (algorithm)](#apidoc.element.node-forge.sha512.create)
1.  object <span class="apidocSignatureSpan">node-forge.sha512.</span>sha224
1.  object <span class="apidocSignatureSpan">node-forge.sha512.</span>sha256
1.  object <span class="apidocSignatureSpan">node-forge.sha512.</span>sha384

#### [module node-forge.sha512.sha224](#apidoc.module.node-forge.sha512.sha224)
1.  [function <span class="apidocSignatureSpan">node-forge.sha512.sha224.</span>create ()](#apidoc.element.node-forge.sha512.sha224.create)

#### [module node-forge.sha512.sha256](#apidoc.module.node-forge.sha512.sha256)
1.  [function <span class="apidocSignatureSpan">node-forge.sha512.sha256.</span>create ()](#apidoc.element.node-forge.sha512.sha256.create)

#### [module node-forge.ssh](#apidoc.module.node-forge.ssh)
1.  [function <span class="apidocSignatureSpan">node-forge.ssh.</span>getPublicKeyFingerprint (key, options)](#apidoc.element.node-forge.ssh.getPublicKeyFingerprint)
1.  [function <span class="apidocSignatureSpan">node-forge.ssh.</span>privateKeyToOpenSSH (privateKey, passphrase)](#apidoc.element.node-forge.ssh.privateKeyToOpenSSH)
1.  [function <span class="apidocSignatureSpan">node-forge.ssh.</span>privateKeyToPutty (privateKey, passphrase, comment)](#apidoc.element.node-forge.ssh.privateKeyToPutty)
1.  [function <span class="apidocSignatureSpan">node-forge.ssh.</span>publicKeyToOpenSSH (key, comment)](#apidoc.element.node-forge.ssh.publicKeyToOpenSSH)

#### [module node-forge.task](#apidoc.module.node-forge.task)
1.  [function <span class="apidocSignatureSpan">node-forge.task.</span>cancel (type)](#apidoc.element.node-forge.task.cancel)
1.  [function <span class="apidocSignatureSpan">node-forge.task.</span>createCondition ()](#apidoc.element.node-forge.task.createCondition)
1.  [function <span class="apidocSignatureSpan">node-forge.task.</span>start (options)](#apidoc.element.node-forge.task.start)

#### [module node-forge.tls](#apidoc.module.node-forge.tls)
1.  [function <span class="apidocSignatureSpan">node-forge.tls.</span>createConnection (options)](#apidoc.element.node-forge.tls.createConnection)
1.  [function <span class="apidocSignatureSpan">node-forge.tls.</span>createSessionCache (cache, capacity)](#apidoc.element.node-forge.tls.createSessionCache)
1.  [function <span class="apidocSignatureSpan">node-forge.tls.</span>hmac_sha1 (key, seqNum, record)](#apidoc.element.node-forge.tls.hmac_sha1)
1.  [function <span class="apidocSignatureSpan">node-forge.tls.</span>prf_tls1 (secret, label, seed, length)](#apidoc.element.node-forge.tls.prf_tls1)
1.  [function <span class="apidocSignatureSpan">node-forge.tls.</span>wrapSocket (options)](#apidoc.element.node-forge.tls.wrapSocket)
1.  number <span class="apidocSignatureSpan">node-forge.tls.</span>MaxFragment
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>Alert
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>BulkCipherAlgorithm
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>CipherSuites
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>CipherType
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>CompressionMethod
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>ConnectionEnd
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>ContentType
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>HandshakeType
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>HeartbeatMessageType
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>MACAlgorithm
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>PRFAlgorithm
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>SupportedVersions
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>Version
1.  object <span class="apidocSignatureSpan">node-forge.tls.</span>Versions

#### [module node-forge.util](#apidoc.module.node-forge.util)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>ByteBuffer (b)](#apidoc.element.node-forge.util.ByteBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>ByteStringBuffer (b)](#apidoc.element.node-forge.util.ByteStringBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>DataBuffer (b, options)](#apidoc.element.node-forge.util.DataBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesFromIP (ip)](#apidoc.element.node-forge.util.bytesFromIP)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesFromIPv4 (ip)](#apidoc.element.node-forge.util.bytesFromIPv4)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesFromIPv6 (ip)](#apidoc.element.node-forge.util.bytesFromIPv6)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToHex (bytes)](#apidoc.element.node-forge.util.bytesToHex)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToIP (bytes)](#apidoc.element.node-forge.util.bytesToIP)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToIPv4 (bytes)](#apidoc.element.node-forge.util.bytesToIPv4)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToIPv6 (bytes)](#apidoc.element.node-forge.util.bytesToIPv6)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>clearItems (api, id, location)](#apidoc.element.node-forge.util.clearItems)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>createBuffer (input, encoding)](#apidoc.element.node-forge.util.createBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>decode64 (input)](#apidoc.element.node-forge.util.decode64)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>decodeUtf8 (str)](#apidoc.element.node-forge.util.decodeUtf8)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>deflate (api, bytes, raw)](#apidoc.element.node-forge.util.deflate)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>deletePath (object, keys)](#apidoc.element.node-forge.util.deletePath)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>encode64 (input, maxline)](#apidoc.element.node-forge.util.encode64)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>encodeUtf8 (str)](#apidoc.element.node-forge.util.encodeUtf8)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>estimateCores (options, callback)](#apidoc.element.node-forge.util.estimateCores)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>fillString (c, n)](#apidoc.element.node-forge.util.fillString)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>format (format)](#apidoc.element.node-forge.util.format)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>formatNumber (number, decimals, dec_point, thousands_sep)](#apidoc.element.node-forge.util.formatNumber)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>formatSize (size)](#apidoc.element.node-forge.util.formatSize)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>getItem (api, id, key, location)](#apidoc.element.node-forge.util.getItem)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>getPath (object, keys, _default)](#apidoc.element.node-forge.util.getPath)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>getQueryVariables (query)](#apidoc.element.node-forge.util.getQueryVariables)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>hexToBytes (hex)](#apidoc.element.node-forge.util.hexToBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>inflate (api, bytes, raw)](#apidoc.element.node-forge.util.inflate)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>int32ToBytes (i)](#apidoc.element.node-forge.util.int32ToBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>isArray ()](#apidoc.element.node-forge.util.isArray)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>isArrayBuffer (x)](#apidoc.element.node-forge.util.isArrayBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>isArrayBufferView (x)](#apidoc.element.node-forge.util.isArrayBufferView)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>isEmpty (obj)](#apidoc.element.node-forge.util.isEmpty)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>makeLink (path, query, fragment)](#apidoc.element.node-forge.util.makeLink)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>makeRequest (reqString)](#apidoc.element.node-forge.util.makeRequest)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>nextTick (callback)](#apidoc.element.node-forge.util.nextTick)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>parseFragment (fragment)](#apidoc.element.node-forge.util.parseFragment)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>parseUrl (str)](#apidoc.element.node-forge.util.parseUrl)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>removeItem (api, id, key, location)](#apidoc.element.node-forge.util.removeItem)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>setImmediate (callback, arg1, arg2, arg3)](#apidoc.element.node-forge.util.setImmediate)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>setItem (api, id, key, data, location)](#apidoc.element.node-forge.util.setItem)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>setPath (object, keys, value)](#apidoc.element.node-forge.util.setPath)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>xorBytes (s1, s2, n)](#apidoc.element.node-forge.util.xorBytes)
1.  object <span class="apidocSignatureSpan">node-forge.util.</span>binary
1.  object <span class="apidocSignatureSpan">node-forge.util.</span>text
1.  string <span class="apidocSignatureSpan">node-forge.util.</span>isNodejs

#### [module node-forge.util.ByteBuffer](#apidoc.module.node-forge.util.ByteBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>ByteBuffer (b)](#apidoc.element.node-forge.util.ByteBuffer.ByteBuffer)

#### [module node-forge.util.ByteBuffer.prototype](#apidoc.module.node-forge.util.ByteBuffer.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>_optimizeConstructedString (x)](#apidoc.element.node-forge.util.ByteBuffer.prototype._optimizeConstructedString)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>at (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.at)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>bytes (count)](#apidoc.element.node-forge.util.ByteBuffer.prototype.bytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>clear ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.clear)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>compact ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.compact)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>copy ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.copy)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>fillWithByte (b, n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.fillWithByte)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getByte ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getByte)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getBytes (count)](#apidoc.element.node-forge.util.ByteBuffer.prototype.getBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt (n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt16 ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt16)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt16Le ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt16Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt24 ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt24)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt24Le ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt24Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt32 ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt32)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt32Le ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt32Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getSignedInt (n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.getSignedInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>isEmpty ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>last ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.last)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>length ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.length)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putBuffer (buffer)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putByte (b)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putByte)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putBytes (bytes)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt (i, n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt16 (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt16)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt16Le (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt16Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt24 (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt24)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt24Le (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt24Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt32 (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt32)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt32Le (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt32Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putSignedInt (i, n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putSignedInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putString (str)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putString)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>setAt (i, b)](#apidoc.element.node-forge.util.ByteBuffer.prototype.setAt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>toHex ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.toHex)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>toString ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>truncate (count)](#apidoc.element.node-forge.util.ByteBuffer.prototype.truncate)

#### [module node-forge.util.DataBuffer](#apidoc.module.node-forge.util.DataBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.</span>DataBuffer (b, options)](#apidoc.element.node-forge.util.DataBuffer.DataBuffer)

#### [module node-forge.util.DataBuffer.prototype](#apidoc.module.node-forge.util.DataBuffer.prototype)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>accommodate (amount, growSize)](#apidoc.element.node-forge.util.DataBuffer.prototype.accommodate)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>at (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.at)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>bytes (count)](#apidoc.element.node-forge.util.DataBuffer.prototype.bytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>clear ()](#apidoc.element.node-forge.util.DataBuffer.prototype.clear)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>compact ()](#apidoc.element.node-forge.util.DataBuffer.prototype.compact)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>copy ()](#apidoc.element.node-forge.util.DataBuffer.prototype.copy)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>fillWithByte (b, n)](#apidoc.element.node-forge.util.DataBuffer.prototype.fillWithByte)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getByte ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getByte)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getBytes (count)](#apidoc.element.node-forge.util.DataBuffer.prototype.getBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt (n)](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt16 ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt16)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt16Le ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt16Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt24 ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt24)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt24Le ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt24Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt32 ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt32)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt32Le ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt32Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getSignedInt (n)](#apidoc.element.node-forge.util.DataBuffer.prototype.getSignedInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>isEmpty ()](#apidoc.element.node-forge.util.DataBuffer.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>last ()](#apidoc.element.node-forge.util.DataBuffer.prototype.last)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>length ()](#apidoc.element.node-forge.util.DataBuffer.prototype.length)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putBuffer (buffer)](#apidoc.element.node-forge.util.DataBuffer.prototype.putBuffer)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putByte (b)](#apidoc.element.node-forge.util.DataBuffer.prototype.putByte)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putBytes (bytes, encoding)](#apidoc.element.node-forge.util.DataBuffer.prototype.putBytes)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt (i, n)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt16 (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt16)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt16Le (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt16Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt24 (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt24)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt24Le (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt24Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt32 (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt32)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt32Le (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt32Le)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putSignedInt (i, n)](#apidoc.element.node-forge.util.DataBuffer.prototype.putSignedInt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putString (str)](#apidoc.element.node-forge.util.DataBuffer.prototype.putString)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>setAt (i, b)](#apidoc.element.node-forge.util.DataBuffer.prototype.setAt)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>toHex ()](#apidoc.element.node-forge.util.DataBuffer.prototype.toHex)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>toString (encoding)](#apidoc.element.node-forge.util.DataBuffer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>truncate (count)](#apidoc.element.node-forge.util.DataBuffer.prototype.truncate)



# <a name="apidoc.module.node-forge"></a>[module node-forge](#apidoc.module.node-forge)

#### <a name="apidoc.element.node-forge.aes.Algorithm"></a>[function <span class="apidocSignatureSpan">node-forge.</span>aes.Algorithm (name, mode)](#apidoc.element.node-forge.aes.Algorithm)
- description and source-code
```javascript
aes.Algorithm = function (name, mode) {
  if(!init) {
    initialize();
  }
  var self = this;
  self.name = name;
  self.mode = new mode({
    blockSize: 16,
    cipher: {
      encrypt: function(inBlock, outBlock) {
        return _updateBlock(self._w, inBlock, outBlock, false);
      },
      decrypt: function(inBlock, outBlock) {
        return _updateBlock(self._w, inBlock, outBlock, true);
      }
    }
  });
  self._init = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.BlockCipher"></a>[function <span class="apidocSignatureSpan">node-forge.</span>cipher.BlockCipher (options)](#apidoc.element.node-forge.cipher.BlockCipher)
- description and source-code
```javascript
cipher.BlockCipher = function (options) {
  this.algorithm = options.algorithm;
  this.mode = this.algorithm.mode;
  this.blockSize = this.mode.blockSize;
  this._finish = false;
  this._input = null;
  this.output = null;
  this._op = options.decrypt ? this.mode.decrypt : this.mode.encrypt;
  this._decrypt = options.decrypt;
  this.algorithm.initialize(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.des.Algorithm"></a>[function <span class="apidocSignatureSpan">node-forge.</span>des.Algorithm (name, mode)](#apidoc.element.node-forge.des.Algorithm)
- description and source-code
```javascript
des.Algorithm = function (name, mode) {
  var self = this;
  self.name = name;
  self.mode = new mode({
    blockSize: 8,
    cipher: {
      encrypt: function(inBlock, outBlock) {
        return _updateBlock(self._keys, inBlock, outBlock, false);
      },
      decrypt: function(inBlock, outBlock) {
        return _updateBlock(self._keys, inBlock, outBlock, true);
      }
    }
  });
  self._init = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger"></a>[function <span class="apidocSignatureSpan">node-forge.</span>jsbn.BigInteger (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger)
- description and source-code
```javascript
function BigInteger(a, b, c) {
  this.data = [];
  if(a != null)
    if("number" == typeof a) this.fromNumber(a,b,c);
    else if(b == null && "string" != typeof a) this.fromString(a,256);
    else this.fromString(a,b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pbkdf2"></a>[function <span class="apidocSignatureSpan">node-forge.</span>pbkdf2 ( p, s, c, dkLen, md, callback)](#apidoc.element.node-forge.pbkdf2)
- description and source-code
```javascript
pbkdf2 = function ( p, s, c, dkLen, md, callback) {
  if(typeof md === 'function') {
    callback = md;
    md = null;
  }

  // use native implementation if possible and not disabled, note that
  // some node versions only support SHA-1, others allow digest to be changed
  if(forge.util.isNodejs && !forge.options.usePureJavaScript &&
    crypto.pbkdf2 && (md === null || typeof md !== 'object') &&
    (crypto.pbkdf2Sync.length > 4 || (!md || md === 'sha1'))) {
    if(typeof md !== 'string') {
      // default prf to SHA-1
      md = 'sha1';
    }
    p = new Buffer(p, 'binary');
    s = new Buffer(s, 'binary');
    if(!callback) {
      if(crypto.pbkdf2Sync.length === 4) {
        return crypto.pbkdf2Sync(p, s, c, dkLen).toString('binary');
      }
      return crypto.pbkdf2Sync(p, s, c, dkLen, md).toString('binary');
    }
    if(crypto.pbkdf2Sync.length === 4) {
      return crypto.pbkdf2(p, s, c, dkLen, function(err, key) {
        if(err) {
          return callback(err);
        }
        callback(null, key.toString('binary'));
      });
    }
    return crypto.pbkdf2(p, s, c, dkLen, md, function(err, key) {
      if(err) {
        return callback(err);
      }
      callback(null, key.toString('binary'));
    });
  }

  if(typeof md === 'undefined' || md === null) {
    // default prf to SHA-1
    md = 'sha1';
  }
  if(typeof md === 'string') {
    if(!(md in forge.md.algorithms)) {
      throw new Error('Unknown hash algorithm: ' + md);
    }
    md = forge.md[md].create();
  }

  var hLen = md.digestLength;

<span class="apidocCodeCommentSpan">  /* 1. If dkLen > (2^32 - 1) * hLen, output "derived key too long" and
    stop. */
</span>  if(dkLen > (0xFFFFFFFF * hLen)) {
    var err = new Error('Derived key is too long.');
    if(callback) {
      return callback(err);
    }
    throw err;
  }

  /* 2. Let len be the number of hLen-octet blocks in the derived key,
    rounding up, and let r be the number of octets in the last
    block:

    len = CEIL(dkLen / hLen),
    r = dkLen - (len - 1) * hLen. */
  var len = Math.ceil(dkLen / hLen);
  var r = dkLen - (len - 1) * hLen;

  /* 3. For each block of the derived key apply the function F defined
    below to the password P, the salt S, the iteration count c, and
    the block index to compute the block:

    T_1 = F(P, S, c, 1),
    T_2 = F(P, S, c, 2),
    ...
    T_len = F(P, S, c, len),

    where the function F is defined as the exclusive-or sum of the
    first c iterates of the underlying pseudorandom function PRF
    applied to the password P and the concatenation of the salt S
    and the block index i:

    F(P, S, c, i) = u_1 XOR u_2 XOR ... XOR u_c

    where

    u_1 = PRF(P, S || INT(i)),
    u_2 = PRF(P, u_1),
    ...
    u_c = PRF(P, u_{c-1}).

    Here, INT(i) is a four-octet encoding of the integer i, most
    significant octet first. */
  var prf = forge.hmac.create();
  prf.start(md, p);
  var dk = '';
  var xor, u_c, u_c1;

  // sync version
  if(!callback) {
    for(var i = 1; i <= len; ++i) {
      // PRF(P, S || INT(i)) (first iteration)
      prf.start(null, null);
      prf.update(s);
      prf.update(forge.util.int32ToBytes(i));
      xor = u_c1 = prf.digest().getBytes();

      // PRF(P, u_{c-1}) (other iterations)
      for(var j = 2; j <= c; ++j) {
        prf.start(null, null);
        prf.update(u_c1);
        u_c = prf.digest().getBytes();
        // F(p, s, c, i)
        xor = forge.util.xorBytes(xor, u_c, hLen);
        u_c1 = u_c;
      }

      /* 4. Concatenate the blocks and extract the first dkLen octets to
        produce a derived key DK:

        DK = T_1 || T_2 ||  ...  || T_len<0..r-1> */
      dk += (i < len) ? xor : xor.substr(0, r);
    }
    /* 5. Output the derived key DK. */
    return dk;
  }

  // async version
  var i = 1, j;
  function outer() {
    if(i > len) {
      // done
      return callback(null, dk);
    }

    // PRF(P, S || INT(i)) (first iteration)
    prf.start(null, null);
    prf.update(s);
    prf.update(forge.util.int32ToBytes(i));
    xor = u_c1 = prf.digest().getBytes();

    // PRF(P, u_{c-1}) (other iterations)
    j = 2;
    inner();
  } ...
```
- example usage
```shell
...
// generate a random key and IV
// Note: a key size of 16 bytes will use AES-128, 24 => AES-192, 32 => AES-256
var key = forge.random.getBytesSync(16);
var iv = forge.random.getBytesSync(16);

/* alternatively, generate a password-based 16-byte key
var salt = forge.random.getBytesSync(128);
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.</span>util.ByteBuffer (b)](#apidoc.element.node-forge.util.ByteBuffer)
- description and source-code
```javascript
function ByteStringBuffer(b) {
  // TODO: update to match DataBuffer API

  // the data in this buffer
  this.data = '';
  // the pointer for reading from this buffer
  this.read = 0;

  if(typeof b === 'string') {
    this.data = b;
  } else if(util.isArrayBuffer(b) || util.isArrayBufferView(b)) {
    // convert native buffer to forge buffer
    // FIXME: support native buffers internally instead
    var arr = new Uint8Array(b);
    try {
      this.data = String.fromCharCode.apply(null, arr);
    } catch(e) {
      for(var i = 0; i < arr.length; ++i) {
        this.putByte(arr[i]);
      }
    }
  } else if(b instanceof ByteStringBuffer ||
    (typeof b === 'object' && typeof b.data === 'string' &&
    typeof b.read === 'number')) {
    // copy existing buffer
    this.data = b.data;
    this.read = b.read;
  }

  // used for v8 optimization
  this._constructedStringLength = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.</span>util.DataBuffer (b, options)](#apidoc.element.node-forge.util.DataBuffer)
- description and source-code
```javascript
function DataBuffer(b, options) {
  // default options
  options = options || {};

  // pointers for read from/write to buffer
  this.read = options.readOffset || 0;
  this.growSize = options.growSize || 1024;

  var isArrayBuffer = util.isArrayBuffer(b);
  var isArrayBufferView = util.isArrayBufferView(b);
  if(isArrayBuffer || isArrayBufferView) {
    // use ArrayBuffer directly
    if(isArrayBuffer) {
      this.data = new DataView(b);
    } else {
      // TODO: adjust read/write offset based on the type of view
      // or specify that this must be done in the options ... that the
      // offsets are byte-based
      this.data = new DataView(b.buffer, b.byteOffset, b.byteLength);
    }
    this.write = ('writeOffset' in options ?
      options.writeOffset : this.data.byteLength);
    return;
  }

  // initialize to empty array buffer and add any given bytes using putBytes
  this.data = new DataView(new ArrayBuffer(0));
  this.write = 0;

  if(b !== null && b !== undefined) {
    this.putBytes(b);
  }

  if('writeOffset' in options) {
    this.write = options.writeOffset;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.aes"></a>[module node-forge.aes](#apidoc.module.node-forge.aes)

#### <a name="apidoc.element.node-forge.aes.Algorithm"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>Algorithm (name, mode)](#apidoc.element.node-forge.aes.Algorithm)
- description and source-code
```javascript
Algorithm = function (name, mode) {
  if(!init) {
    initialize();
  }
  var self = this;
  self.name = name;
  self.mode = new mode({
    blockSize: 16,
    cipher: {
      encrypt: function(inBlock, outBlock) {
        return _updateBlock(self._w, inBlock, outBlock, false);
      },
      decrypt: function(inBlock, outBlock) {
        return _updateBlock(self._w, inBlock, outBlock, true);
      }
    }
  });
  self._init = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.aes._expandKey"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>_expandKey (key, decrypt)](#apidoc.element.node-forge.aes._expandKey)
- description and source-code
```javascript
_expandKey = function (key, decrypt) {
  if(!init) {
    initialize();
  }
  return _expandKey(key, decrypt);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.aes._updateBlock"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>_updateBlock (w, input, output, decrypt)](#apidoc.element.node-forge.aes._updateBlock)
- description and source-code
```javascript
function _updateBlock(w, input, output, decrypt) {
<span class="apidocCodeCommentSpan">  /*
  Cipher(byte in[4*Nb], byte out[4*Nb], word w[Nb*(Nr+1)])
  begin
    byte state[4,Nb]
    state = in
    AddRoundKey(state, w[0, Nb-1])
    for round = 1 step 1 to Nr–1
      SubBytes(state)
      ShiftRows(state)
      MixColumns(state)
      AddRoundKey(state, w[round*Nb, (round+1)*Nb-1])
    end for
    SubBytes(state)
    ShiftRows(state)
    AddRoundKey(state, w[Nr*Nb, (Nr+1)*Nb-1])
    out = state
  end

  InvCipher(byte in[4*Nb], byte out[4*Nb], word w[Nb*(Nr+1)])
  begin
    byte state[4,Nb]
    state = in
    AddRoundKey(state, w[Nr*Nb, (Nr+1)*Nb-1])
    for round = Nr-1 step -1 downto 1
      InvShiftRows(state)
      InvSubBytes(state)
      AddRoundKey(state, w[round*Nb, (round+1)*Nb-1])
      InvMixColumns(state)
    end for
    InvShiftRows(state)
    InvSubBytes(state)
    AddRoundKey(state, w[0, Nb-1])
    out = state
  end
  */
</span>
  // Encrypt: AddRoundKey(state, w[0, Nb-1])
  // Decrypt: AddRoundKey(state, w[Nr*Nb, (Nr+1)*Nb-1])
  var Nr = w.length / 4 - 1;
  var m0, m1, m2, m3, sub;
  if(decrypt) {
    m0 = imix[0];
    m1 = imix[1];
    m2 = imix[2];
    m3 = imix[3];
    sub = isbox;
  } else {
    m0 = mix[0];
    m1 = mix[1];
    m2 = mix[2];
    m3 = mix[3];
    sub = sbox;
  }
  var a, b, c, d, a2, b2, c2;
  a = input[0] ^ w[0];
  b = input[decrypt ? 3 : 1] ^ w[1];
  c = input[2] ^ w[2];
  d = input[decrypt ? 1 : 3] ^ w[3];
  var i = 3;

  /* In order to share code we follow the encryption algorithm when both
    encrypting and decrypting. To account for the changes required in the
    decryption algorithm, we use different lookup tables when decrypting
    and use a modified key schedule to account for the difference in the
    order of transformations applied when performing rounds. We also get
    key rounds in reverse order (relative to encryption). */
  for(var round = 1; round < Nr; ++round) {
    /* As described above, we'll be using table lookups to perform the
      column mixing. Each column is stored as a word in the state (the
      array 'input' has one column as a word at each index). In order to
      mix a column, we perform these transformations on each row in c,
      which is 1 byte in each word. The new column for c0 is c'0:

               m0      m1      m2      m3
      r0,c'0 = 2*r0,c0 + 3*r1,c0 + 1*r2,c0 + 1*r3,c0
      r1,c'0 = 1*r0,c0 + 2*r1,c0 + 3*r2,c0 + 1*r3,c0
      r2,c'0 = 1*r0,c0 + 1*r1,c0 + 2*r2,c0 + 3*r3,c0
      r3,c'0 = 3*r0,c0 + 1*r1,c0 + 1*r2,c0 + 2*r3,c0

      So using mix tables where c0 is a word with r0 being its upper
      8 bits and r3 being its lower 8 bits:

      m0[c0 >> 24] will yield this word: [2*r0,1*r0,1*r0,3*r0]
      ...
      m3[c0 & 255] will yield this word: [1*r3,1*r3,3*r3,2*r3]

      Therefore to mix the columns in each word in the state we
      do the following (& 255 omitted for brevity):
      c'0,r0 = m0[c0 >> 24] ^ m1[c1 >> 16] ^ m2[c2 >> 8] ^ m3[c3]
      c'0,r1 = m0[c0 >> 24] ^ m1[c1 >> 16] ^ m2[c2 >> 8] ^ m3[c3]
      c'0,r2 = m0[c0 >> 24] ^ m1[c1 >> 16] ^ m2[c2 >> 8] ^ m3[c3]
      c'0,r3 = m0[c0 >> 24] ^ m1[c1 >> 16] ^ m2[c2 >> 8] ^ m3[c3]

      However, before mixing, the algorithm requires us to perform
      ShiftRows(). The ShiftRows() transformation cyclically shifts the
      last 3 rows of the state over different offsets. The first row
      (r = 0) is not shifted.

      s'_r,c = s_r,(c + shift(r, Nb) mod Nb
      for 0 < r < 4 and 0 <= c < Nb and
      shift(1, 4) = 1
      shift(2, 4) = 2
      shift(3, 4) = 3.

      This causes the first byte in r = 1 to be moved to the end of
      the row, the first 2 bytes in r = 2 to be moved to the end of
      the row, the first 3 bytes in r = 3 to be moved to the end of
      the row:

      r1: [c0 c1 c2 c3] => [c1 c2 c3 c0]
      r2: [c0 c1 c2 c3]    [c2 c3 c0 c1]
      r3: [c0 c1 c2 c3]    [c3 c0 c1 c2]

      We can make these substitutions inline with our column mixing to
      generate an updated set of equations to produce each word in the
      state (note the columns have changed positions):

      c0 c1 ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.aes.createDecryptionCipher"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>createDecryptionCipher (key, mode)](#apidoc.element.node-forge.aes.createDecryptionCipher)
- description and source-code
```javascript
createDecryptionCipher = function (key, mode) {
  return _createCipher({
    key: key,
    output: null,
    decrypt: true,
    mode: mode
  });
}
```
- example usage
```shell
...
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes
var cipher = forge.rc2.createDecryptionCipher(key);
cipher.start(iv);
cipher.update(encrypted);
cipher.finish();
// outputs decrypted hex
console.log(cipher.output.toHex());
'''
...
```

#### <a name="apidoc.element.node-forge.aes.createEncryptionCipher"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>createEncryptionCipher (key, mode)](#apidoc.element.node-forge.aes.createEncryptionCipher)
- description and source-code
```javascript
createEncryptionCipher = function (key, mode) {
  return _createCipher({
    key: key,
    output: null,
    decrypt: false,
    mode: mode
  });
}
```
- example usage
```shell
...

'''js
// generate a random key and IV
var key = forge.random.getBytesSync(16);
var iv = forge.random.getBytesSync(8);

// encrypt some bytes
var cipher = forge.rc2.createEncryptionCipher(key);
cipher.start(iv);
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());
...
```

#### <a name="apidoc.element.node-forge.aes.startDecrypting"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>startDecrypting (key, iv, output, mode)](#apidoc.element.node-forge.aes.startDecrypting)
- description and source-code
```javascript
startDecrypting = function (key, iv, output, mode) {
  var cipher = _createCipher({
    key: key,
    output: output,
    decrypt: true,
    mode: mode
  });
  cipher.start(iv);
  return cipher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.aes.startEncrypting"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>startEncrypting (key, iv, output, mode)](#apidoc.element.node-forge.aes.startEncrypting)
- description and source-code
```javascript
startEncrypting = function (key, iv, output, mode) {
  var cipher = _createCipher({
    key: key,
    output: output,
    decrypt: false,
    mode: mode
  });
  cipher.start(iv);
  return cipher;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.aes.Algorithm"></a>[module node-forge.aes.Algorithm](#apidoc.module.node-forge.aes.Algorithm)

#### <a name="apidoc.element.node-forge.aes.Algorithm.Algorithm"></a>[function <span class="apidocSignatureSpan">node-forge.aes.</span>Algorithm (name, mode)](#apidoc.element.node-forge.aes.Algorithm.Algorithm)
- description and source-code
```javascript
Algorithm = function (name, mode) {
  if(!init) {
    initialize();
  }
  var self = this;
  self.name = name;
  self.mode = new mode({
    blockSize: 16,
    cipher: {
      encrypt: function(inBlock, outBlock) {
        return _updateBlock(self._w, inBlock, outBlock, false);
      },
      decrypt: function(inBlock, outBlock) {
        return _updateBlock(self._w, inBlock, outBlock, true);
      }
    }
  });
  self._init = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.aes.Algorithm.prototype"></a>[module node-forge.aes.Algorithm.prototype](#apidoc.module.node-forge.aes.Algorithm.prototype)

#### <a name="apidoc.element.node-forge.aes.Algorithm.prototype.initialize"></a>[function <span class="apidocSignatureSpan">node-forge.aes.Algorithm.prototype.</span>initialize (options)](#apidoc.element.node-forge.aes.Algorithm.prototype.initialize)
- description and source-code
```javascript
initialize = function (options) {
  if(this._init) {
    return;
  }

  var key = options.key;
  var tmp;

<span class="apidocCodeCommentSpan">  /* Note: The key may be a string of bytes, an array of bytes, a byte
    buffer, or an array of 32-bit integers. If the key is in bytes, then
    it must be 16, 24, or 32 bytes in length. If it is in 32-bit
    integers, it must be 4, 6, or 8 integers long. */
</span>
  if(typeof key === 'string' &&
    (key.length === 16 || key.length === 24 || key.length === 32)) {
    // convert key string into byte buffer
    key = forge.util.createBuffer(key);
  } else if(forge.util.isArray(key) &&
    (key.length === 16 || key.length === 24 || key.length === 32)) {
    // convert key integer array into byte buffer
    tmp = key;
    key = forge.util.createBuffer();
    for(var i = 0; i < tmp.length; ++i) {
      key.putByte(tmp[i]);
    }
  }

  // convert key byte buffer into 32-bit integer array
  if(!forge.util.isArray(key)) {
    tmp = key;
    key = [];

    // key lengths of 16, 24, 32 bytes allowed
    var len = tmp.length();
    if(len === 16 || len === 24 || len === 32) {
      len = len >>> 2;
      for(var i = 0; i < len; ++i) {
        key.push(tmp.getInt32());
      }
    }
  }

  // key must be an array of 32-bit integers by now
  if(!forge.util.isArray(key) ||
    !(key.length === 4 || key.length === 6 || key.length === 8)) {
    throw new Error('Invalid key parameter.');
  }

  // encryption operation is always used for these modes
  var mode = this.mode.name;
  var encryptOp = (['CFB', 'OFB', 'CTR', 'GCM'].indexOf(mode) !== -1);

  // do key expansion
  this._w = _expandKey(key, options.decrypt && !encryptOp);
  this._init = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.asn1"></a>[module node-forge.asn1](#apidoc.module.node-forge.asn1)

#### <a name="apidoc.element.node-forge.asn1.copy"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>copy (obj, options)](#apidoc.element.node-forge.asn1.copy)
- description and source-code
```javascript
copy = function (obj, options) {
  var copy;

  if(forge.util.isArray(obj)) {
    copy = [];
    for(var i = 0; i < obj.length; ++i) {
      copy.push(asn1.copy(obj[i], options));
    }
    return copy;
  }

  if(typeof obj === 'string') {
    // TODO: copy byte buffer if it's a buffer not a string
    return obj;
  }

  copy = {
    tagClass: obj.tagClass,
    type: obj.type,
    constructed: obj.constructed,
    composed: obj.composed,
    value: asn1.copy(obj.value, options)
  };
  if(options && !options.excludeBitStringContents) {
    // TODO: copy byte buffer if it's a buffer not a string
    copy.bitStringContents = obj.bitStringContents;
  }
  return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.create"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>create (tagClass, type, constructed, value, options)](#apidoc.element.node-forge.asn1.create)
- description and source-code
```javascript
create = function (tagClass, type, constructed, value, options) {
<span class="apidocCodeCommentSpan">  /* An asn1 object has a tagClass, a type, a constructed flag, and a
    value. The value's type depends on the constructed flag. If
    constructed, it will contain a list of other asn1 objects. If not,
    it will contain the ASN.1 value as an array of bytes formatted
    according to the ASN.1 data type. */
</span>
  // remove undefined values
  if(forge.util.isArray(value)) {
    var tmp = [];
    for(var i = 0; i < value.length; ++i) {
      if(value[i] !== undefined) {
        tmp.push(value[i]);
      }
    }
    value = tmp;
  }

  var obj = {
    tagClass: tagClass,
    type: type,
    constructed: constructed,
    composed: constructed || forge.util.isArray(value),
    value: value
  };
  if(options && 'bitStringContents' in options) {
    // TODO: copy byte buffer if it's a buffer not a string
    obj.bitStringContents = options.bitStringContents;
    // TODO: add readonly flag to avoid this overhead
    // save copy to detect changes
    obj.original = asn1.copy(obj);
  }
  return obj;
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```

#### <a name="apidoc.element.node-forge.asn1.dateToGeneralizedTime"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>dateToGeneralizedTime (date)](#apidoc.element.node-forge.asn1.dateToGeneralizedTime)
- description and source-code
```javascript
dateToGeneralizedTime = function (date) {
  // TODO: validate; currently assumes proper format
  if(typeof date === 'string') {
    return date;
  }

  var rval = '';

  // create format YYYYMMDDHHMMSSZ
  var format = [];
  format.push('' + date.getUTCFullYear());
  format.push('' + (date.getUTCMonth() + 1));
  format.push('' + date.getUTCDate());
  format.push('' + date.getUTCHours());
  format.push('' + date.getUTCMinutes());
  format.push('' + date.getUTCSeconds());

  // ensure 2 digits are used for each format entry
  for(var i = 0; i < format.length; ++i) {
    if(format[i].length < 2) {
      rval += '0';
    }
    rval += format[i];
  }
  rval += 'Z';

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.dateToUtcTime"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>dateToUtcTime (date)](#apidoc.element.node-forge.asn1.dateToUtcTime)
- description and source-code
```javascript
dateToUtcTime = function (date) {
  // TODO: validate; currently assumes proper format
  if(typeof date === 'string') {
    return date;
  }

  var rval = '';

  // create format YYMMDDhhmmssZ
  var format = [];
  format.push(('' + date.getUTCFullYear()).substr(2));
  format.push('' + (date.getUTCMonth() + 1));
  format.push('' + date.getUTCDate());
  format.push('' + date.getUTCHours());
  format.push('' + date.getUTCMinutes());
  format.push('' + date.getUTCSeconds());

  // ensure 2 digits are used for each format entry
  for(var i = 0; i < format.length; ++i) {
    if(format[i].length < 2) {
      rval += '0';
    }
    rval += format[i];
  }
  rval += 'Z';

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.derToInteger"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>derToInteger (bytes)](#apidoc.element.node-forge.asn1.derToInteger)
- description and source-code
```javascript
derToInteger = function (bytes) {
  // wrap in buffer if needed
  if(typeof bytes === 'string') {
    bytes = forge.util.createBuffer(bytes);
  }

  var n = bytes.length() * 8;
  if(n > 32) {
    throw new Error('Integer too large; max is 32-bits.');
  }
  return bytes.getSignedInt(n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.derToOid"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>derToOid (bytes)](#apidoc.element.node-forge.asn1.derToOid)
- description and source-code
```javascript
derToOid = function (bytes) {
  var oid;

  // wrap in buffer if needed
  if(typeof bytes === 'string') {
    bytes = forge.util.createBuffer(bytes);
  }

  // first byte is 40 * value1 + value2
  var b = bytes.getByte();
  oid = Math.floor(b / 40) + '.' + (b % 40);

  // other bytes are each value in base 128 with 8th bit set except for
  // the last byte for each value
  var value = 0;
  while(bytes.length() > 0) {
    b = bytes.getByte();
    value = value << 7;
    // not the last byte for the value
    if(b & 0x80) {
      value += b & 0x7F;
    } else {
      // last byte
      oid += '.' + (value + b);
      value = 0;
    }
  }

  return oid;
}
```
- example usage
```shell
...
// deserialize to an ASN.1 object from a byte buffer filled with DER data
var object = asn1.fromDer(derBuffer);

// convert an OID dot-separated string to a byte buffer
var derOidBuffer = asn1.oidToDer('1.2.840.113549.1.1.5');

// convert a byte buffer with a DER-encoded OID to a dot-separated string
console.log(asn1.derToOid(derOidBuffer));
// output: 1.2.840.113549.1.1.5

// validates that an ASN.1 object matches a particular ASN.1 structure and
// captures data of interest from that structure for easy access
var publicKeyValidator = {
name: 'SubjectPublicKeyInfo',
tagClass: asn1.Class.UNIVERSAL,
...
```

#### <a name="apidoc.element.node-forge.asn1.equals"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>equals (obj1, obj2, options)](#apidoc.element.node-forge.asn1.equals)
- description and source-code
```javascript
equals = function (obj1, obj2, options) {
  if(forge.util.isArray(obj1)) {
    if(!forge.util.isArray(obj2)) {
      return false;
    }
    if(obj1.length !== obj2.length) {
      return false;
    }
    for(var i = 0; i < obj1.length; ++i) {
      if(!asn1.equals(obj1[i], obj2[i])) {
        return false;
      }
      return true;
    }
  }

  if(typeof obj1 !== typeof obj2) {
    return false;
  }

  if(typeof obj1 === 'string') {
    return obj1 === obj2;
  }

  var equal = obj1.tagClass === obj2.tagClass &&
    obj1.type === obj2.type &&
    obj1.constructed === obj2.constructed &&
    obj1.composed === obj2.composed &&
    asn1.equals(obj1.value, obj2.value);
  if(options && options.includeBitStringContents) {
    equal = equal && (obj1.bitStringContents === obj2.bitStringContents);
  }

  return equal;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.fromDer"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>fromDer (bytes, options)](#apidoc.element.node-forge.asn1.fromDer)
- description and source-code
```javascript
fromDer = function (bytes, options) {
  if(options === undefined) {
    options = {
      strict: true,
      decodeBitStrings: true
    };
  }
  if(typeof options === 'boolean') {
    options = {
      strict: options,
      decodeBitStrings: true
    };
  }
  if(!('strict' in options)) {
    options.strict = true;
  }
  if(!('decodeBitStrings' in options)) {
    options.decodeBitStrings = true;
  }

  // wrap in buffer if needed
  if(typeof bytes === 'string') {
    bytes = forge.util.createBuffer(bytes);
  }

  return _fromDer(bytes, bytes.length(), 0, options);
}
```
- example usage
```shell
...

__Examples__

'''js
// decode p12 from base64
var p12Der = forge.util.decode64(p12b64);
// get p12 as ASN.1 object
var p12Asn1 = forge.asn1.fromDer(p12Der);
// decrypt p12 using the password 'password'
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, 'password');
// decrypt p12 using non-strict parsing mode (resolves some ASN.1 parse errors)
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, false, 'password');
// decrypt p12 using literally no password (eg: Mac OS X/apple push)
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1);
// decrypt p12 using an "empty" password (eg: OpenSSL with no password input)
...
```

#### <a name="apidoc.element.node-forge.asn1.generalizedTimeToDate"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>generalizedTimeToDate (gentime)](#apidoc.element.node-forge.asn1.generalizedTimeToDate)
- description and source-code
```javascript
generalizedTimeToDate = function (gentime) {
<span class="apidocCodeCommentSpan">  /* The following formats can be used:

    YYYYMMDDHHMMSS
    YYYYMMDDHHMMSS.fff
    YYYYMMDDHHMMSSZ
    YYYYMMDDHHMMSS.fffZ
    YYYYMMDDHHMMSS+hh'mm'
    YYYYMMDDHHMMSS.fff+hh'mm'
    YYYYMMDDHHMMSS-hh'mm'
    YYYYMMDDHHMMSS.fff-hh'mm'

    Where:

    YYYY is the year
    MM is the month (01 to 12)
    DD is the day (01 to 31)
    hh is the hour (00 to 23)
    mm are the minutes (00 to 59)
    ss are the seconds (00 to 59)
    .fff is the second fraction, accurate to three decimal places
    Z indicates that local time is GMT, + indicates that local time is
    later than GMT, and - indicates that local time is earlier than GMT
    hh' is the absolute value of the offset from GMT in hours
    mm' is the absolute value of the offset from GMT in minutes */
</span>  var date = new Date();

  var YYYY = parseInt(gentime.substr(0, 4), 10);
  var MM = parseInt(gentime.substr(4, 2), 10) - 1; // use 0-11 for month
  var DD = parseInt(gentime.substr(6, 2), 10);
  var hh = parseInt(gentime.substr(8, 2), 10);
  var mm = parseInt(gentime.substr(10, 2), 10);
  var ss = parseInt(gentime.substr(12, 2), 10);
  var fff = 0;
  var offset = 0;
  var isUTC = false;

  if(gentime.charAt(gentime.length - 1) === 'Z') {
    isUTC = true;
  }

  var end = gentime.length - 5, c = gentime.charAt(end);
  if(c === '+' || c === '-') {
    // get hours+minutes offset
    var hhoffset = parseInt(gentime.substr(end + 1, 2), 10);
    var mmoffset = parseInt(gentime.substr(end + 4, 2), 10);

    // calculate offset in milliseconds
    offset = hhoffset * 60 + mmoffset;
    offset *= 60000;

    // apply offset
    if(c === '+') {
      offset *= -1;
    }

    isUTC = true;
  }

  // check for second fraction
  if(gentime.charAt(14) === '.') {
    fff = parseFloat(gentime.substr(14), 10) * 1000;
  }

  if(isUTC) {
    date.setUTCFullYear(YYYY, MM, DD);
    date.setUTCHours(hh, mm, ss, fff);

    // apply offset
    date.setTime(+date + offset);
  } else {
    date.setFullYear(YYYY, MM, DD);
    date.setHours(hh, mm, ss, fff);
  }

  return date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.getBerValueLength"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>getBerValueLength (b)](#apidoc.element.node-forge.asn1.getBerValueLength)
- description and source-code
```javascript
getBerValueLength = function (b) {
  // TODO: move this function and related DER/BER functions to a der.js
  // file; better abstract ASN.1 away from der/ber.
  var b2 = b.getByte();
  if(b2 === 0x80) {
    return undefined;
  }

  // see if the length is "short form" or "long form" (bit 8 set)
  var length;
  var longForm = b2 & 0x80;
  if(!longForm) {
    // length is just the first byte
    length = b2;
  } else {
    // the number of bytes the length is specified in bits 7 through 1
    // and each length byte is in big-endian base-256
    length = b.getInt((b2 & 0x7F) << 3);
  }
  return length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.integerToDer"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>integerToDer (x)](#apidoc.element.node-forge.asn1.integerToDer)
- description and source-code
```javascript
integerToDer = function (x) {
  var rval = forge.util.createBuffer();
  if(x >= -0x80 && x < 0x80) {
    return rval.putSignedInt(x, 8);
  }
  if(x >= -0x8000 && x < 0x8000) {
    return rval.putSignedInt(x, 16);
  }
  if(x >= -0x800000 && x < 0x800000) {
    return rval.putSignedInt(x, 24);
  }
  if(x >= -0x80000000 && x < 0x80000000) {
    return rval.putSignedInt(x, 32);
  }
  var error = new Error('Integer too large; max is 32-bits.');
  error.integer = x;
  throw error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.oidToDer"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>oidToDer (oid)](#apidoc.element.node-forge.asn1.oidToDer)
- description and source-code
```javascript
oidToDer = function (oid) {
  // split OID into individual values
  var values = oid.split('.');
  var bytes = forge.util.createBuffer();

  // first byte is 40 * value1 + value2
  bytes.putByte(40 * parseInt(values[0], 10) + parseInt(values[1], 10));
  // other bytes are each value in base 128 with 8th bit set except for
  // the last byte for each value
  var last, valueBytes, value, b;
  for(var i = 2; i < values.length; ++i) {
    // produce value bytes in reverse because we don't know how many
    // bytes it will take to store the value
    last = true;
    valueBytes = [];
    value = parseInt(values[i], 10);
    do {
      b = value & 0x7F;
      value = value >>> 7;
      // if value is not last, then turn on 8th bit
      if(!last) {
        b |= 0x80;
      }
      valueBytes.push(b);
      last = false;
    } while(value > 0);

    // add value bytes in reverse (needs to be in big endian)
    for(var n = valueBytes.length - 1; n >= 0; --n) {
      bytes.putByte(valueBytes[n]);
    }
  }

  return bytes;
}
```
- example usage
```shell
...
// create a SubjectPublicKeyInfo
var subjectPublicKeyInfo =
asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
  // AlgorithmIdentifier
  asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // algorithm
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
      asn1.oidToDer(pki.oids['rsaEncryption']).getBytes()),
    // parameters (null)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.NULL, false, '')
  ]),
  // subjectPublicKey
  asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false, [
    // RSAPublicKey
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
...
```

#### <a name="apidoc.element.node-forge.asn1.prettyPrint"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>prettyPrint (obj, level, indentation)](#apidoc.element.node-forge.asn1.prettyPrint)
- description and source-code
```javascript
prettyPrint = function (obj, level, indentation) {
  var rval = '';

  // set default level and indentation
  level = level || 0;
  indentation = indentation || 2;

  // start new line for deep levels
  if(level > 0) {
    rval += '\n';
  }

  // create indent
  var indent = '';
  for(var i = 0; i < level * indentation; ++i) {
    indent += ' ';
  }

  // print class:type
  rval += indent + 'Tag: ';
  switch(obj.tagClass) {
  case asn1.Class.UNIVERSAL:
    rval += 'Universal:';
    break;
  case asn1.Class.APPLICATION:
    rval += 'Application:';
    break;
  case asn1.Class.CONTEXT_SPECIFIC:
    rval += 'Context-Specific:';
    break;
  case asn1.Class.PRIVATE:
    rval += 'Private:';
    break;
  }

  if(obj.tagClass === asn1.Class.UNIVERSAL) {
    rval += obj.type;

    // known types
    switch(obj.type) {
    case asn1.Type.NONE:
      rval += ' (None)';
      break;
    case asn1.Type.BOOLEAN:
      rval += ' (Boolean)';
      break;
    case asn1.Type.INTEGER:
      rval += ' (Integer)';
      break;
    case asn1.Type.BITSTRING:
      rval += ' (Bit string)';
      break;
    case asn1.Type.OCTETSTRING:
      rval += ' (Octet string)';
      break;
    case asn1.Type.NULL:
      rval += ' (Null)';
      break;
    case asn1.Type.OID:
      rval += ' (Object Identifier)';
      break;
    case asn1.Type.ODESC:
      rval += ' (Object Descriptor)';
      break;
    case asn1.Type.EXTERNAL:
      rval += ' (External or Instance of)';
      break;
    case asn1.Type.REAL:
      rval += ' (Real)';
      break;
    case asn1.Type.ENUMERATED:
      rval += ' (Enumerated)';
      break;
    case asn1.Type.EMBEDDED:
      rval += ' (Embedded PDV)';
      break;
    case asn1.Type.UTF8:
      rval += ' (UTF8)';
      break;
    case asn1.Type.ROID:
      rval += ' (Relative Object Identifier)';
      break;
    case asn1.Type.SEQUENCE:
      rval += ' (Sequence)';
      break;
    case asn1.Type.SET:
      rval += ' (Set)';
      break;
    case asn1.Type.PRINTABLESTRING:
      rval += ' (Printable String)';
      break;
    case asn1.Type.IA5String:
      rval += ' (IA5String (ASCII))';
      break;
    case asn1.Type.UTCTIME:
      rval += ' (UTC time)';
      break;
    case asn1.Type.GENERALIZEDTIME:
      rval += ' (Generalized time)';
      break;
    case asn1.Type.BMPSTRING:
      rval += ' (BMP String)';
      break;
    }
  } else {
    rval += obj.type;
  }

  rval += '\n';
  rval += indent + 'Constructed: ' + obj.constructed + '\n';

  if(obj.composed) {
    var subvalues = 0;
    var sub = '';
    for(var i = 0; i < obj.value.length; ++i) {
      if(obj.value[i] !== undefined) {
        subvalues += 1;
        sub += asn1.prettyPrint(obj.value[i], level + 1, indentation);
        if((i + 1) < obj.value.length) {
          sub += ',';
        }
      }
    }
    rval += indent + 'Sub values: ' + subvalues + sub;
  } else {
    rval += indent + 'Value: ';
    if(obj.type === asn1.Type.OID) {
      var oid = asn1.derToOid(obj.value);
      rval += oid;
      if(forge.pki && forge.pki.oids) {
        if(oid in forge.pki.oids) {
          rval += ' (' + forge.pki.oids[oid] + ') ';
        }
      }
    }
    if(obj.type === asn1.Type.INTEGER) {
      try {
        rval += asn1.derToInteger(obj.value);
      } catch(ex) {
        rval += '0x' + forge.util.bytesToHex(obj.value);
      }
    } else if(obj.type === asn1.Type.BITSTRING) {
      // TODO: shift bits as needed to display without padding
      if(obj.value.length > 1) {
        // remove unused bits field
        rval += '0x' + forge.util.bytesToHex(obj.value.slice(1));
      } else {
        rval += '(none)';
      }
      // show unused bit count
      if(obj.value.length > 0) {
        var unused = obj.value.charCodeAt(0);
        if(unused == 1) {
          rval += ' (1 unused bit shown)';
        } else if(unused > 1) {
          rval += ' (' + unused + ' unused bits shown)';
        }
      }
    } else if(obj.type === asn1.Type.OCTETSTRING) {
      if(!_nonLatinRegex.test(obj.value)) {
        rval += '(' + obj.value + ') ';
      }
      rval += '0x' + forge.util ...
```
- example usage
```shell
...
// capture.publicKeyOid only contains the value for the OID
var oid = asn1.derToOid(capture.publicKeyOid);
if(oid !== pki.oids['rsaEncryption']) {
  throw 'Unsupported OID.';
}

// pretty print an ASN.1 object to a string for debugging purposes
asn1.prettyPrint(object);
'''

Message Digests
----------------

<a name="sha1" />
### SHA1
...
```

#### <a name="apidoc.element.node-forge.asn1.toDer"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>toDer (obj)](#apidoc.element.node-forge.asn1.toDer)
- description and source-code
```javascript
toDer = function (obj) {
  var bytes = forge.util.createBuffer();

  // build the first byte
  var b1 = obj.tagClass | obj.type;

  // for storing the ASN.1 value
  var value = forge.util.createBuffer();

  // use BIT STRING contents if available and data not changed
  var useBitStringContents = false;
  if('bitStringContents' in obj) {
    useBitStringContents = true;
    if(obj.original) {
      useBitStringContents = asn1.equals(obj, obj.original);
    }
  }

  if(useBitStringContents) {
    value.putBytes(obj.bitStringContents);
  } else if(obj.composed) {
    // if composed, use each child asn1 object's DER bytes as value
    // turn on 6th bit (0x20 = 32) to indicate asn1 is constructed
    // from other asn1 objects
    if(obj.constructed) {
      b1 |= 0x20;
    } else {
      // type is a bit string, add unused bits of 0x00
      value.putByte(0x00);
    }

    // add all of the child DER bytes together
    for(var i = 0; i < obj.value.length; ++i) {
      if(obj.value[i] !== undefined) {
        value.putBuffer(asn1.toDer(obj.value[i]));
      }
    }
  } else {
    // use asn1.value directly
    if(obj.type === asn1.Type.BMPSTRING) {
      for(var i = 0; i < obj.value.length; ++i) {
        value.putInt16(obj.value.charCodeAt(i));
      }
    } else {
      // ensure integer is minimally-encoded
      // TODO: should all leading bytes be stripped vs just one?
      // .. ex '00 00 01' => '01'?
      if(obj.type === asn1.Type.INTEGER &&
        obj.value.length > 1 &&
        // leading 0x00 for positive integer
        ((obj.value.charCodeAt(0) === 0 &&
        (obj.value.charCodeAt(1) & 0x80) === 0) ||
        // leading 0xFF for negative integer
        (obj.value.charCodeAt(0) === 0xFF &&
        (obj.value.charCodeAt(1) & 0x80) === 0x80))) {
        value.putBytes(obj.value.substr(1));
      } else {
        value.putBytes(obj.value);
      }
    }
  }

  // add tag byte
  bytes.putByte(b1);

  // use "short form" encoding
  if(value.length() <= 127) {
    // one byte describes the length
    // bit 8 = 0 and bits 7-1 = length
    bytes.putByte(value.length() & 0x7F);
  } else {
    // use "long form" encoding
    // 2 to 127 bytes describe the length
    // first byte: bit 8 = 1 and bits 7-1 = # of additional bytes
    // other bytes: length in base 256, big-endian
    var len = value.length();
    var lenBytes = '';
    do {
      lenBytes += String.fromCharCode(len & 0xFF);
      len = len >>> 8;
    } while(len > 0);

    // set first byte to # bytes used to store the length and turn on
    // bit 8 to indicate long-form length is used
    bytes.putByte(lenBytes.length | 0x80);

    // concatenate length bytes in reverse since they were generated
    // little endian and we need big endian
    for(var i = lenBytes.length - 1; i >= 0; --i) {
      bytes.putByte(lenBytes.charCodeAt(i));
    }
  }

  // concatenate value bytes
  bytes.putBuffer(value);
  return bytes;
}
```
- example usage
```shell
...
// generate a p12 that can be imported by Chrome/Firefox/iOS
// (requires the use of Triple DES instead of AES)
var p12Asn1 = forge.pkcs12.toPkcs12Asn1(
  privateKey, certificateChain, 'password',
  {algorithm: '3des'});

// base64-encode p12
var p12Der = forge.asn1.toDer(p12Asn1).getBytes();
var p12b64 = forge.util.encode64(p12Der);

// create download link for p12
var a = document.createElement('a');
a.download = 'example.p12';
a.setAttribute('href', 'data:application/x-pkcs12;base64,' + p12b64);
a.appendChild(document.createTextNode('Download'));
...
```

#### <a name="apidoc.element.node-forge.asn1.utcTimeToDate"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>utcTimeToDate (utc)](#apidoc.element.node-forge.asn1.utcTimeToDate)
- description and source-code
```javascript
utcTimeToDate = function (utc) {
<span class="apidocCodeCommentSpan">  /* The following formats can be used:

    YYMMDDhhmmZ
    YYMMDDhhmm+hh'mm'
    YYMMDDhhmm-hh'mm'
    YYMMDDhhmmssZ
    YYMMDDhhmmss+hh'mm'
    YYMMDDhhmmss-hh'mm'

    Where:

    YY is the least significant two digits of the year
    MM is the month (01 to 12)
    DD is the day (01 to 31)
    hh is the hour (00 to 23)
    mm are the minutes (00 to 59)
    ss are the seconds (00 to 59)
    Z indicates that local time is GMT, + indicates that local time is
    later than GMT, and - indicates that local time is earlier than GMT
    hh' is the absolute value of the offset from GMT in hours
    mm' is the absolute value of the offset from GMT in minutes */
</span>  var date = new Date();

  // if YY >= 50 use 19xx, if YY < 50 use 20xx
  var year = parseInt(utc.substr(0, 2), 10);
  year = (year >= 50) ? 1900 + year : 2000 + year;
  var MM = parseInt(utc.substr(2, 2), 10) - 1; // use 0-11 for month
  var DD = parseInt(utc.substr(4, 2), 10);
  var hh = parseInt(utc.substr(6, 2), 10);
  var mm = parseInt(utc.substr(8, 2), 10);
  var ss = 0;

  // not just YYMMDDhhmmZ
  if(utc.length > 11) {
    // get character after minutes
    var c = utc.charAt(10);
    var end = 10;

    // see if seconds are present
    if(c !== '+' && c !== '-') {
      // get seconds
      ss = parseInt(utc.substr(10, 2), 10);
      end += 2;
    }
  }

  // update date
  date.setUTCFullYear(year, MM, DD);
  date.setUTCHours(hh, mm, ss, 0);

  if(end) {
    // get +/- after end of time
    c = utc.charAt(end);
    if(c === '+' || c === '-') {
      // get hours+minutes offset
      var hhoffset = parseInt(utc.substr(end + 1, 2), 10);
      var mmoffset = parseInt(utc.substr(end + 4, 2), 10);

      // calculate offset in milliseconds
      var offset = hhoffset * 60 + mmoffset;
      offset *= 60000;

      // apply offset
      if(c === '+') {
        date.setTime(+date - offset);
      } else {
        date.setTime(+date + offset);
      }
    }
  }

  return date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.asn1.validate"></a>[function <span class="apidocSignatureSpan">node-forge.asn1.</span>validate (obj, v, capture, errors)](#apidoc.element.node-forge.asn1.validate)
- description and source-code
```javascript
validate = function (obj, v, capture, errors) {
  var rval = false;

  // ensure tag class and type are the same if specified
  if((obj.tagClass === v.tagClass || typeof(v.tagClass) === 'undefined') &&
    (obj.type === v.type || typeof(v.type) === 'undefined')) {
    // ensure constructed flag is the same if specified
    if(obj.constructed === v.constructed ||
      typeof(v.constructed) === 'undefined') {
      rval = true;

      // handle sub values
      if(v.value && forge.util.isArray(v.value)) {
        var j = 0;
        for(var i = 0; rval && i < v.value.length; ++i) {
          rval = v.value[i].optional || false;
          if(obj.value[j]) {
            rval = asn1.validate(obj.value[j], v.value[i], capture, errors);
            if(rval) {
              ++j;
            } else if(v.value[i].optional) {
              rval = true;
            }
          }
          if(!rval && errors) {
            errors.push(
              '[' + v.name + '] ' +
              'Tag class "' + v.tagClass + '", type "' +
              v.type + '" expected value length "' +
              v.value.length + '", got "' +
              obj.value.length + '"');
          }
        }
      }

      if(rval && capture) {
        if(v.capture) {
          capture[v.capture] = obj.value;
        }
        if(v.captureAsn1) {
          capture[v.captureAsn1] = obj;
        }
        if(v.captureBitStringContents && 'bitStringContents' in obj) {
          capture[v.captureBitStringContents] = obj.bitStringContents;
        }
        if(v.captureBitStringValue && 'bitStringContents' in obj) {
          var value;
          if(obj.bitStringContents.length < 2) {
            capture[v.captureBitStringValue] = '';
          } else {
            // FIXME: support unused bits with data shifting
            var unused = obj.bitStringContents.charCodeAt(0);
            if(unused !== 0) {
              throw new Error(
                'captureBitStringValue only supported for zero unused bits');
            }
            capture[v.captureBitStringValue] = obj.bitStringContents.slice(1);
          }
        }
      }
    } else if(errors) {
      errors.push(
        '[' + v.name + '] ' +
        'Expected constructed "' + v.constructed + '", got "' +
        obj.constructed + '"');
    }
  } else if(errors) {
    if(obj.tagClass !== v.tagClass) {
      errors.push(
        '[' + v.name + '] ' +
        'Expected tag class "' + v.tagClass + '", got "' +
        obj.tagClass + '"');
    }
    if(obj.type !== v.type) {
      errors.push(
        '[' + v.name + '] ' +
        'Expected type "' + v.type + '", got "' + obj.type + '"');
    }
  }
  return rval;
}
```
- example usage
```shell
...
      captureAsn1: 'rsaPublicKey'
    }]
  }]
};

var capture = {};
var errors = [];
if(!asn1.validate(
  publicKeyValidator, subjectPublicKeyInfo, validator, capture, errors)) {
  throw 'ASN.1 object is not a SubjectPublicKeyInfo.';
}
// capture.subjectPublicKeyInfo contains the full ASN.1 object
// capture.rsaPublicKey contains the full ASN.1 object for the RSA public key
// capture.publicKeyOid only contains the value for the OID
var oid = asn1.derToOid(capture.publicKeyOid);
...
```



# <a name="apidoc.module.node-forge.cipher"></a>[module node-forge.cipher](#apidoc.module.node-forge.cipher)

#### <a name="apidoc.element.node-forge.cipher.BlockCipher"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.</span>BlockCipher (options)](#apidoc.element.node-forge.cipher.BlockCipher)
- description and source-code
```javascript
BlockCipher = function (options) {
  this.algorithm = options.algorithm;
  this.mode = this.algorithm.mode;
  this.blockSize = this.mode.blockSize;
  this._finish = false;
  this._input = null;
  this.output = null;
  this._op = options.decrypt ? this.mode.decrypt : this.mode.encrypt;
  this._decrypt = options.decrypt;
  this.algorithm.initialize(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.createCipher"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.</span>createCipher (algorithm, key)](#apidoc.element.node-forge.cipher.createCipher)
- description and source-code
```javascript
createCipher = function (algorithm, key) {
  var api = algorithm;
  if(typeof api === 'string') {
    api = forge.cipher.getAlgorithm(api);
    if(api) {
      api = api();
    }
  }
  if(!api) {
    throw new Error('Unsupported algorithm: ' + algorithm);
  }

  // assume block cipher
  return new forge.cipher.BlockCipher({
    algorithm: api,
    key: key,
    decrypt: false
  });
}
```
- example usage
```shell
...
var salt = forge.random.getBytesSync(128);
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());
...
```

#### <a name="apidoc.element.node-forge.cipher.createDecipher"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.</span>createDecipher (algorithm, key)](#apidoc.element.node-forge.cipher.createDecipher)
- description and source-code
```javascript
createDecipher = function (algorithm, key) {
  var api = algorithm;
  if(typeof api === 'string') {
    api = forge.cipher.getAlgorithm(api);
    if(api) {
      api = api();
    }
  }
  if(!api) {
    throw new Error('Unsupported algorithm: ' + algorithm);
  }

  // assume block cipher
  return new forge.cipher.BlockCipher({
    algorithm: api,
    key: key,
    decrypt: true
  });
}
```
- example usage
```shell
...
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
// (other modes include: CFB, OFB, CTR, and GCM)
var decipher = forge.cipher.createDecipher('AES-CBC', key);
decipher.start({iv: iv});
decipher.update(encrypted);
decipher.finish();
// outputs decrypted hex
console.log(decipher.output.toHex());

// encrypt some bytes using GCM mode
...
```

#### <a name="apidoc.element.node-forge.cipher.getAlgorithm"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.</span>getAlgorithm (name)](#apidoc.element.node-forge.cipher.getAlgorithm)
- description and source-code
```javascript
getAlgorithm = function (name) {
  name = name.toUpperCase();
  if(name in forge.cipher.algorithms) {
    return forge.cipher.algorithms[name];
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.registerAlgorithm"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.</span>registerAlgorithm (name, algorithm)](#apidoc.element.node-forge.cipher.registerAlgorithm)
- description and source-code
```javascript
registerAlgorithm = function (name, algorithm) {
  name = name.toUpperCase();
  forge.cipher.algorithms[name] = algorithm;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.BlockCipher"></a>[module node-forge.cipher.BlockCipher](#apidoc.module.node-forge.cipher.BlockCipher)

#### <a name="apidoc.element.node-forge.cipher.BlockCipher.BlockCipher"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.</span>BlockCipher (options)](#apidoc.element.node-forge.cipher.BlockCipher.BlockCipher)
- description and source-code
```javascript
BlockCipher = function (options) {
  this.algorithm = options.algorithm;
  this.mode = this.algorithm.mode;
  this.blockSize = this.mode.blockSize;
  this._finish = false;
  this._input = null;
  this.output = null;
  this._op = options.decrypt ? this.mode.decrypt : this.mode.encrypt;
  this._decrypt = options.decrypt;
  this.algorithm.initialize(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.BlockCipher.prototype"></a>[module node-forge.cipher.BlockCipher.prototype](#apidoc.module.node-forge.cipher.BlockCipher.prototype)

#### <a name="apidoc.element.node-forge.cipher.BlockCipher.prototype.finish"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.BlockCipher.prototype.</span>finish (pad)](#apidoc.element.node-forge.cipher.BlockCipher.prototype.finish)
- description and source-code
```javascript
finish = function (pad) {
  // backwards-compatibility w/deprecated padding API
  // Note: will overwrite padding functions even after another start() call
  if(pad && (this.mode.name === 'ECB' || this.mode.name === 'CBC')) {
    this.mode.pad = function(input) {
      return pad(this.blockSize, input, false);
    };
    this.mode.unpad = function(output) {
      return pad(this.blockSize, output, true);
    };
  }

  // build options for padding and afterFinish functions
  var options = {};
  options.decrypt = this._decrypt;

  // get # of bytes that won't fill a block
  options.overflow = this._input.length() % this.blockSize;

  if(!this._decrypt && this.mode.pad) {
    if(!this.mode.pad(this._input, options)) {
      return false;
    }
  }

  // do final update
  this._finish = true;
  this.update();

  if(this._decrypt && this.mode.unpad) {
    if(!this.mode.unpad(this.output, options)) {
      return false;
    }
  }

  if(this.mode.afterFinish) {
    if(!this.mode.afterFinish(this.output, options)) {
      return false;
    }
  }

  return true;
}
```
- example usage
```shell
...

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
// (other modes include: CFB, OFB, CTR, and GCM)
var decipher = forge.cipher.createDecipher('AES-CBC', key);
...
```

#### <a name="apidoc.element.node-forge.cipher.BlockCipher.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.BlockCipher.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.BlockCipher.prototype.start)
- description and source-code
```javascript
start = function (options) {
  options = options || {};
  var opts = {};
  for(var key in options) {
    opts[key] = options[key];
  }
  opts.decrypt = this._decrypt;
  this._finish = false;
  this._input = forge.util.createBuffer();
  this.output = options.output || forge.util.createBuffer();
  this.mode.start(opts);
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```

#### <a name="apidoc.element.node-forge.cipher.BlockCipher.prototype.update"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.BlockCipher.prototype.</span>update (input)](#apidoc.element.node-forge.cipher.BlockCipher.prototype.update)
- description and source-code
```javascript
update = function (input) {
  if(input) {
    // input given, so empty it into the input buffer
    this._input.putBuffer(input);
  }

  // do cipher operation until it needs more input and not finished
  while(!this._op.call(this.mode, this._input, this.output, this._finish) &&
    !this._finish) {}

  // free consumed memory from input buffer
  this._input.compact();
}
```
- example usage
```shell
...
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
// (other modes include: CFB, OFB, CTR, and GCM)
...
```



# <a name="apidoc.module.node-forge.cipher.algorithms"></a>[module node-forge.cipher.algorithms](#apidoc.module.node-forge.cipher.algorithms)

#### <a name="apidoc.element.node-forge.cipher.algorithms.3DES-CBC"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-CBC ()](#apidoc.element.node-forge.cipher.algorithms.3DES-CBC)
- description and source-code
```javascript
3DES-CBC = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.3DES-CFB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-CFB ()](#apidoc.element.node-forge.cipher.algorithms.3DES-CFB)
- description and source-code
```javascript
3DES-CFB = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.3DES-CTR"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-CTR ()](#apidoc.element.node-forge.cipher.algorithms.3DES-CTR)
- description and source-code
```javascript
3DES-CTR = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.3DES-ECB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-ECB ()](#apidoc.element.node-forge.cipher.algorithms.3DES-ECB)
- description and source-code
```javascript
3DES-ECB = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.3DES-OFB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>3DES-OFB ()](#apidoc.element.node-forge.cipher.algorithms.3DES-OFB)
- description and source-code
```javascript
3DES-OFB = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.AES-CBC"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-CBC ()](#apidoc.element.node-forge.cipher.algorithms.AES-CBC)
- description and source-code
```javascript
AES-CBC = function () {
  return new forge.aes.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.AES-CFB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-CFB ()](#apidoc.element.node-forge.cipher.algorithms.AES-CFB)
- description and source-code
```javascript
AES-CFB = function () {
  return new forge.aes.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.AES-CTR"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-CTR ()](#apidoc.element.node-forge.cipher.algorithms.AES-CTR)
- description and source-code
```javascript
AES-CTR = function () {
  return new forge.aes.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.AES-ECB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-ECB ()](#apidoc.element.node-forge.cipher.algorithms.AES-ECB)
- description and source-code
```javascript
AES-ECB = function () {
  return new forge.aes.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.AES-GCM"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-GCM ()](#apidoc.element.node-forge.cipher.algorithms.AES-GCM)
- description and source-code
```javascript
AES-GCM = function () {
  return new forge.aes.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.AES-OFB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>AES-OFB ()](#apidoc.element.node-forge.cipher.algorithms.AES-OFB)
- description and source-code
```javascript
AES-OFB = function () {
  return new forge.aes.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.DES-CBC"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-CBC ()](#apidoc.element.node-forge.cipher.algorithms.DES-CBC)
- description and source-code
```javascript
DES-CBC = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.DES-CFB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-CFB ()](#apidoc.element.node-forge.cipher.algorithms.DES-CFB)
- description and source-code
```javascript
DES-CFB = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.DES-CTR"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-CTR ()](#apidoc.element.node-forge.cipher.algorithms.DES-CTR)
- description and source-code
```javascript
DES-CTR = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.DES-ECB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-ECB ()](#apidoc.element.node-forge.cipher.algorithms.DES-ECB)
- description and source-code
```javascript
DES-ECB = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.algorithms.DES-OFB"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.algorithms.</span>DES-OFB ()](#apidoc.element.node-forge.cipher.algorithms.DES-OFB)
- description and source-code
```javascript
DES-OFB = function () {
  return new forge.des.Algorithm(name, mode);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.modes"></a>[module node-forge.cipher.modes](#apidoc.module.node-forge.cipher.modes)

#### <a name="apidoc.element.node-forge.cipher.modes.cbc"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>cbc (options)](#apidoc.element.node-forge.cipher.modes.cbc)
- description and source-code
```javascript
cbc = function (options) {
  options = options || {};
  this.name = 'CBC';
  this.cipher = options.cipher;
  this.blockSize = options.blockSize || 16;
  this._ints = this.blockSize / 4;
  this._inBlock = new Array(this._ints);
  this._outBlock = new Array(this._ints);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.cfb"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>cfb (options)](#apidoc.element.node-forge.cipher.modes.cfb)
- description and source-code
```javascript
cfb = function (options) {
  options = options || {};
  this.name = 'CFB';
  this.cipher = options.cipher;
  this.blockSize = options.blockSize || 16;
  this._ints = this.blockSize / 4;
  this._inBlock = null;
  this._outBlock = new Array(this._ints);
  this._partialBlock = new Array(this._ints);
  this._partialOutput = forge.util.createBuffer();
  this._partialBytes = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.ctr"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>ctr (options)](#apidoc.element.node-forge.cipher.modes.ctr)
- description and source-code
```javascript
ctr = function (options) {
  options = options || {};
  this.name = 'CTR';
  this.cipher = options.cipher;
  this.blockSize = options.blockSize || 16;
  this._ints = this.blockSize / 4;
  this._inBlock = null;
  this._outBlock = new Array(this._ints);
  this._partialOutput = forge.util.createBuffer();
  this._partialBytes = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.ecb"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>ecb (options)](#apidoc.element.node-forge.cipher.modes.ecb)
- description and source-code
```javascript
ecb = function (options) {
  options = options || {};
  this.name = 'ECB';
  this.cipher = options.cipher;
  this.blockSize = options.blockSize || 16;
  this._ints = this.blockSize / 4;
  this._inBlock = new Array(this._ints);
  this._outBlock = new Array(this._ints);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>gcm (options)](#apidoc.element.node-forge.cipher.modes.gcm)
- description and source-code
```javascript
gcm = function (options) {
  options = options || {};
  this.name = 'GCM';
  this.cipher = options.cipher;
  this.blockSize = options.blockSize || 16;
  this._ints = this.blockSize / 4;
  this._inBlock = new Array(this._ints);
  this._outBlock = new Array(this._ints);
  this._partialOutput = forge.util.createBuffer();
  this._partialBytes = 0;

  // R is actually this value concatenated with 120 more zero bits, but
  // we only XOR against R so the other zeros have no effect -- we just
  // apply this value to the first integer in a block
  this._R = 0xE1000000;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.ofb"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.</span>ofb (options)](#apidoc.element.node-forge.cipher.modes.ofb)
- description and source-code
```javascript
ofb = function (options) {
  options = options || {};
  this.name = 'OFB';
  this.cipher = options.cipher;
  this.blockSize = options.blockSize || 16;
  this._ints = this.blockSize / 4;
  this._inBlock = null;
  this._outBlock = new Array(this._ints);
  this._partialOutput = forge.util.createBuffer();
  this._partialBytes = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.modes.cbc.prototype"></a>[module node-forge.cipher.modes.cbc.prototype](#apidoc.module.node-forge.cipher.modes.cbc.prototype)

#### <a name="apidoc.element.node-forge.cipher.modes.cbc.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (input, output, finish) {
  // not enough input to decrypt
  if(input.length() < this.blockSize && !(finish && input.length() > 0)) {
    return true;
  }

  // get next block
  for(var i = 0; i < this._ints; ++i) {
    this._inBlock[i] = input.getInt32();
  }

  // decrypt block
  this.cipher.decrypt(this._inBlock, this._outBlock);

  // write output, save previous ciphered block
  // CBC XOR's IV (or previous block) with ciphertext
  for(var i = 0; i < this._ints; ++i) {
    output.putInt32(this._prev[i] ^ this._outBlock[i]);
  }
  this._prev = this._inBlock.slice(0);
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.cbc.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (input, output, finish) {
  // not enough input to encrypt
  if(input.length() < this.blockSize && !(finish && input.length() > 0)) {
    return true;
  }

  // get next block
  // CBC XOR's IV (or previous block) with plaintext
  for(var i = 0; i < this._ints; ++i) {
    this._inBlock[i] = this._prev[i] ^ input.getInt32();
  }

  // encrypt block
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // write output, save previous block
  for(var i = 0; i < this._ints; ++i) {
    output.putInt32(this._outBlock[i]);
  }
  this._prev = this._outBlock;
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.cbc.prototype.pad"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>pad (input, options)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.pad)
- description and source-code
```javascript
pad = function (input, options) {
  // add PKCS#7 padding to block (each pad byte is the
  // value of the number of pad bytes)
  var padding = (input.length() === this.blockSize ?
    this.blockSize : (this.blockSize - input.length()));
  input.fillWithByte(padding, padding);
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.cbc.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.start)
- description and source-code
```javascript
start = function (options) {
  // Note: legacy support for using IV residue (has security flaws)
  // if IV is null, reuse block from previous processing
  if(options.iv === null) {
    // must have a previous block
    if(!this._prev) {
      throw new Error('Invalid IV parameter.');
    }
    this._iv = this._prev.slice(0);
  } else if(!('iv' in options)) {
    throw new Error('Invalid IV parameter.');
  } else {
    // save IV as "previous" block
    this._iv = transformIV(options.iv);
    this._prev = this._iv.slice(0);
  }
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.cbc.prototype.unpad"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cbc.prototype.</span>unpad (output, options)](#apidoc.element.node-forge.cipher.modes.cbc.prototype.unpad)
- description and source-code
```javascript
unpad = function (output, options) {
  // check for error: input data not a multiple of blockSize
  if(options.overflow > 0) {
    return false;
  }

  // ensure padding byte count is valid
  var len = output.length();
  var count = output.at(len - 1);
  if(count > (this.blockSize << 2)) {
    return false;
  }

  // trim off padding bytes
  output.truncate(count);
  return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.modes.cfb.prototype"></a>[module node-forge.cipher.modes.cfb.prototype](#apidoc.module.node-forge.cipher.modes.cfb.prototype)

#### <a name="apidoc.element.node-forge.cipher.modes.cfb.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cfb.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cfb.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (input, output, finish) {
  // not enough input to decrypt
  var inputLength = input.length();
  if(inputLength === 0) {
    return true;
  }

  // encrypt block (CFB always uses encryption mode)
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output, write input as output
    for(var i = 0; i < this._ints; ++i) {
      this._inBlock[i] = input.getInt32();
      output.putInt32(this._inBlock[i] ^ this._outBlock[i]);
    }
    return;
  }

  // handle partial block
  var partialBytes = (this.blockSize - inputLength) % this.blockSize;
  if(partialBytes > 0) {
    partialBytes = this.blockSize - partialBytes;
  }

  // XOR input with output, write input as partial output
  this._partialOutput.clear();
  for(var i = 0; i < this._ints; ++i) {
    this._partialBlock[i] = input.getInt32();
    this._partialOutput.putInt32(this._partialBlock[i] ^ this._outBlock[i]);
  }

  if(partialBytes > 0) {
    // block still incomplete, restore input buffer
    input.read -= this.blockSize;
  } else {
    // block complete, update input block
    for(var i = 0; i < this._ints; ++i) {
      this._inBlock[i] = this._partialBlock[i];
    }
  }

  // skip any previous partial bytes
  if(this._partialBytes > 0) {
    this._partialOutput.getBytes(this._partialBytes);
  }

  if(partialBytes > 0 && !finish) {
    output.putBytes(this._partialOutput.getBytes(
      partialBytes - this._partialBytes));
    this._partialBytes = partialBytes;
    return true;
  }

  output.putBytes(this._partialOutput.getBytes(
    inputLength - this._partialBytes));
  this._partialBytes = 0;
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.cfb.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cfb.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.cfb.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (input, output, finish) {
  // not enough input to encrypt
  var inputLength = input.length();
  if(inputLength === 0) {
    return true;
  }

  // encrypt block
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output, write input as output
    for(var i = 0; i < this._ints; ++i) {
      this._inBlock[i] = input.getInt32() ^ this._outBlock[i];
      output.putInt32(this._inBlock[i]);
    }
    return;
  }

  // handle partial block
  var partialBytes = (this.blockSize - inputLength) % this.blockSize;
  if(partialBytes > 0) {
    partialBytes = this.blockSize - partialBytes;
  }

  // XOR input with output, write input as partial output
  this._partialOutput.clear();
  for(var i = 0; i < this._ints; ++i) {
    this._partialBlock[i] = input.getInt32() ^ this._outBlock[i];
    this._partialOutput.putInt32(this._partialBlock[i]);
  }

  if(partialBytes > 0) {
    // block still incomplete, restore input buffer
    input.read -= this.blockSize;
  } else {
    // block complete, update input block
    for(var i = 0; i < this._ints; ++i) {
      this._inBlock[i] = this._partialBlock[i];
    }
  }

  // skip any previous partial bytes
  if(this._partialBytes > 0) {
    this._partialOutput.getBytes(this._partialBytes);
  }

  if(partialBytes > 0 && !finish) {
    output.putBytes(this._partialOutput.getBytes(
      partialBytes - this._partialBytes));
    this._partialBytes = partialBytes;
    return true;
  }

  output.putBytes(this._partialOutput.getBytes(
    inputLength - this._partialBytes));
  this._partialBytes = 0;
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.cfb.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.cfb.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.cfb.prototype.start)
- description and source-code
```javascript
start = function (options) {
  if(!('iv' in options)) {
    throw new Error('Invalid IV parameter.');
  }
  // use IV as first input
  this._iv = transformIV(options.iv);
  this._inBlock = this._iv.slice(0);
  this._partialBytes = 0;
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```



# <a name="apidoc.module.node-forge.cipher.modes.ctr.prototype"></a>[module node-forge.cipher.modes.ctr.prototype](#apidoc.module.node-forge.cipher.modes.ctr.prototype)

#### <a name="apidoc.element.node-forge.cipher.modes.ctr.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ctr.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ctr.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (input, output, finish) {
  // not enough input to encrypt
  var inputLength = input.length();
  if(inputLength === 0) {
    return true;
  }

  // encrypt block (CTR always uses encryption mode)
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output
    for(var i = 0; i < this._ints; ++i) {
      output.putInt32(input.getInt32() ^ this._outBlock[i]);
    }
  } else {
    // handle partial block
    var partialBytes = (this.blockSize - inputLength) % this.blockSize;
    if(partialBytes > 0) {
      partialBytes = this.blockSize - partialBytes;
    }

    // XOR input with output
    this._partialOutput.clear();
    for(var i = 0; i < this._ints; ++i) {
      this._partialOutput.putInt32(input.getInt32() ^ this._outBlock[i]);
    }

    if(partialBytes > 0) {
      // block still incomplete, restore input buffer
      input.read -= this.blockSize;
    }

    // skip any previous partial bytes
    if(this._partialBytes > 0) {
      this._partialOutput.getBytes(this._partialBytes);
    }

    if(partialBytes > 0 && !finish) {
      output.putBytes(this._partialOutput.getBytes(
        partialBytes - this._partialBytes));
      this._partialBytes = partialBytes;
      return true;
    }

    output.putBytes(this._partialOutput.getBytes(
      inputLength - this._partialBytes));
    this._partialBytes = 0;
  }

  // block complete, increment counter (input block)
  inc32(this._inBlock);
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ctr.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ctr.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ctr.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (input, output, finish) {
  // not enough input to encrypt
  var inputLength = input.length();
  if(inputLength === 0) {
    return true;
  }

  // encrypt block (CTR always uses encryption mode)
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output
    for(var i = 0; i < this._ints; ++i) {
      output.putInt32(input.getInt32() ^ this._outBlock[i]);
    }
  } else {
    // handle partial block
    var partialBytes = (this.blockSize - inputLength) % this.blockSize;
    if(partialBytes > 0) {
      partialBytes = this.blockSize - partialBytes;
    }

    // XOR input with output
    this._partialOutput.clear();
    for(var i = 0; i < this._ints; ++i) {
      this._partialOutput.putInt32(input.getInt32() ^ this._outBlock[i]);
    }

    if(partialBytes > 0) {
      // block still incomplete, restore input buffer
      input.read -= this.blockSize;
    }

    // skip any previous partial bytes
    if(this._partialBytes > 0) {
      this._partialOutput.getBytes(this._partialBytes);
    }

    if(partialBytes > 0 && !finish) {
      output.putBytes(this._partialOutput.getBytes(
        partialBytes - this._partialBytes));
      this._partialBytes = partialBytes;
      return true;
    }

    output.putBytes(this._partialOutput.getBytes(
      inputLength - this._partialBytes));
    this._partialBytes = 0;
  }

  // block complete, increment counter (input block)
  inc32(this._inBlock);
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ctr.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ctr.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.ctr.prototype.start)
- description and source-code
```javascript
start = function (options) {
  if(!('iv' in options)) {
    throw new Error('Invalid IV parameter.');
  }
  // use IV as first input
  this._iv = transformIV(options.iv);
  this._inBlock = this._iv.slice(0);
  this._partialBytes = 0;
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```



# <a name="apidoc.module.node-forge.cipher.modes.ecb.prototype"></a>[module node-forge.cipher.modes.ecb.prototype](#apidoc.module.node-forge.cipher.modes.ecb.prototype)

#### <a name="apidoc.element.node-forge.cipher.modes.ecb.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (input, output, finish) {
  // not enough input to decrypt
  if(input.length() < this.blockSize && !(finish && input.length() > 0)) {
    return true;
  }

  // get next block
  for(var i = 0; i < this._ints; ++i) {
    this._inBlock[i] = input.getInt32();
  }

  // decrypt block
  this.cipher.decrypt(this._inBlock, this._outBlock);

  // write output
  for(var i = 0; i < this._ints; ++i) {
    output.putInt32(this._outBlock[i]);
  }
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ecb.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (input, output, finish) {
  // not enough input to encrypt
  if(input.length() < this.blockSize && !(finish && input.length() > 0)) {
    return true;
  }

  // get next block
  for(var i = 0; i < this._ints; ++i) {
    this._inBlock[i] = input.getInt32();
  }

  // encrypt block
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // write output
  for(var i = 0; i < this._ints; ++i) {
    output.putInt32(this._outBlock[i]);
  }
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ecb.prototype.pad"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>pad (input, options)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.pad)
- description and source-code
```javascript
pad = function (input, options) {
  // add PKCS#7 padding to block (each pad byte is the
  // value of the number of pad bytes)
  var padding = (input.length() === this.blockSize ?
    this.blockSize : (this.blockSize - input.length()));
  input.fillWithByte(padding, padding);
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.ecb.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.start)
- description and source-code
```javascript
start = function (options) {}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ecb.prototype.unpad"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ecb.prototype.</span>unpad (output, options)](#apidoc.element.node-forge.cipher.modes.ecb.prototype.unpad)
- description and source-code
```javascript
unpad = function (output, options) {
  // check for error: input data not a multiple of blockSize
  if(options.overflow > 0) {
    return false;
  }

  // ensure padding byte count is valid
  var len = output.length();
  var count = output.at(len - 1);
  if(count > (this.blockSize << 2)) {
    return false;
  }

  // trim off padding bytes
  output.truncate(count);
  return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.modes.gcm.prototype"></a>[module node-forge.cipher.modes.gcm.prototype](#apidoc.module.node-forge.cipher.modes.gcm.prototype)

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.afterFinish"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>afterFinish (output, options)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.afterFinish)
- description and source-code
```javascript
afterFinish = function (output, options) {
  var rval = true;

  // handle overflow
  if(options.decrypt && options.overflow) {
    output.truncate(this.blockSize - options.overflow);
  }

  // handle authentication tag
  this.tag = forge.util.createBuffer();

  // concatenate additional data length with cipher length
  var lengths = this._aDataLength.concat(from64To32(this._cipherLength * 8));

  // include lengths in hash
  this._s = this.ghash(this._hashSubkey, this._s, lengths);

  // do GCTR(J_0, S)
  var tag = [];
  this.cipher.encrypt(this._j0, tag);
  for(var i = 0; i < this._ints; ++i) {
    this.tag.putInt32(this._s[i] ^ tag[i]);
  }

  // trim tag to length
  this.tag.truncate(this.tag.length() % (this._tagLength / 8));

  // check authentication tag
  if(options.decrypt && this.tag.bytes() !== this._tag) {
    rval = false;
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (input, output, finish) {
  // not enough input to decrypt
  var inputLength = input.length();
  if(inputLength < this.blockSize && !(finish && inputLength > 0)) {
    return true;
  }

  // encrypt block (GCM always uses encryption mode)
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // increment counter (input block)
  inc32(this._inBlock);

  // update hash block S
  this._hashBlock[0] = input.getInt32();
  this._hashBlock[1] = input.getInt32();
  this._hashBlock[2] = input.getInt32();
  this._hashBlock[3] = input.getInt32();
  this._s = this.ghash(this._hashSubkey, this._s, this._hashBlock);

  // XOR hash input with output
  for(var i = 0; i < this._ints; ++i) {
    output.putInt32(this._outBlock[i] ^ this._hashBlock[i]);
  }

  // increment cipher data length
  if(inputLength < this.blockSize) {
    this._cipherLength += inputLength % this.blockSize;
  } else {
    this._cipherLength += this.blockSize;
  }
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (input, output, finish) {
  // not enough input to encrypt
  var inputLength = input.length();
  if(inputLength === 0) {
    return true;
  }

  // encrypt block
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output
    for(var i = 0; i < this._ints; ++i) {
      output.putInt32(this._outBlock[i] ^= input.getInt32());
    }
    this._cipherLength += this.blockSize;
  } else {
    // handle partial block
    var partialBytes = (this.blockSize - inputLength) % this.blockSize;
    if(partialBytes > 0) {
      partialBytes = this.blockSize - partialBytes;
    }

    // XOR input with output
    this._partialOutput.clear();
    for(var i = 0; i < this._ints; ++i) {
      this._partialOutput.putInt32(input.getInt32() ^ this._outBlock[i]);
    }

    if(partialBytes === 0 || finish) {
      // handle overflow prior to hashing
      if(finish) {
        // get block overflow
        var overflow = inputLength % this.blockSize;
        this._cipherLength += overflow;
        // truncate for hash function
        this._partialOutput.truncate(this.blockSize - overflow);
      } else {
        this._cipherLength += this.blockSize;
      }

      // get output block for hashing
      for(var i = 0; i < this._ints; ++i) {
        this._outBlock[i] = this._partialOutput.getInt32();
      }
      this._partialOutput.read -= this.blockSize;
    }

    // skip any previous partial bytes
    if(this._partialBytes > 0) {
      this._partialOutput.getBytes(this._partialBytes);
    }

    if(partialBytes > 0 && !finish) {
      // block still incomplete, restore input buffer, get partial output,
      // and return early
      input.read -= this.blockSize;
      output.putBytes(this._partialOutput.getBytes(
        partialBytes - this._partialBytes));
      this._partialBytes = partialBytes;
      return true;
    }

    output.putBytes(this._partialOutput.getBytes(
      inputLength - this._partialBytes));
    this._partialBytes = 0;
  }

  // update hash block S
  this._s = this.ghash(this._hashSubkey, this._s, this._outBlock);

  // increment counter (input block)
  inc32(this._inBlock);
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.generateHashTable"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>generateHashTable (h, bits)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.generateHashTable)
- description and source-code
```javascript
generateHashTable = function (h, bits) {
  // TODO: There are further optimizations that would use only the
  // first table M_0 (or some variant) along with a remainder table;
  // this can be explored in the future
  var multiplier = 8 / bits;
  var perInt = 4 * multiplier;
  var size = 16 * multiplier;
  var m = new Array(size);
  for(var i = 0; i < size; ++i) {
    var tmp = [0, 0, 0, 0];
    var idx = (i / perInt) | 0;
    var shft = ((perInt - 1 - (i % perInt)) * bits);
    tmp[idx] = (1 << (bits - 1)) << shft;
    m[i] = this.generateSubHashTable(this.multiply(tmp, h), bits);
  }
  return m;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.generateSubHashTable"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>generateSubHashTable (mid, bits)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.generateSubHashTable)
- description and source-code
```javascript
generateSubHashTable = function (mid, bits) {
  // compute the table quickly by minimizing the number of
  // POW operations -- they only need to be performed for powers of 2,
  // all other entries can be composed from those powers using XOR
  var size = 1 << bits;
  var half = size >>> 1;
  var m = new Array(size);
  m[half] = mid.slice(0);
  var i = half >>> 1;
  while(i > 0) {
    // raise m0[2 * i] and store in m0[i]
    this.pow(m[2 * i], m[i] = []);
    i >>= 1;
  }
  i = 2;
  while(i < half) {
    for(var j = 1; j < i; ++j) {
      var m_i = m[i];
      var m_j = m[j];
      m[i + j] = [
        m_i[0] ^ m_j[0],
        m_i[1] ^ m_j[1],
        m_i[2] ^ m_j[2],
        m_i[3] ^ m_j[3]
      ];
    }
    i *= 2;
  }
  m[0] = [0, 0, 0, 0];
<span class="apidocCodeCommentSpan">  /* Note: We could avoid storing these by doing composition during multiply
  calculate top half using composition by speed is preferred. */
</span>  for(i = half + 1; i < size; ++i) {
    var c = m[i ^ half];
    m[i] = [mid[0] ^ c[0], mid[1] ^ c[1], mid[2] ^ c[2], mid[3] ^ c[3]];
  }
  return m;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.ghash"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>ghash (h, y, x)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.ghash)
- description and source-code
```javascript
ghash = function (h, y, x) {
  y[0] ^= x[0];
  y[1] ^= x[1];
  y[2] ^= x[2];
  y[3] ^= x[3];
  return this.tableMultiply(y);
  //return this.multiply(y, h);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.multiply"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>multiply (x, y)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.multiply)
- description and source-code
```javascript
multiply = function (x, y) {
  var z_i = [0, 0, 0, 0];
  var v_i = y.slice(0);

  // calculate Z_128 (block has 128 bits)
  for(var i = 0; i < 128; ++i) {
    // if x_i is 0, Z_{i+1} = Z_i (unchanged)
    // else Z_{i+1} = Z_i ^ V_i
    // get x_i by finding 32-bit int position, then left shift 1 by remainder
    var x_i = x[(i / 32) | 0] & (1 << (31 - i % 32));
    if(x_i) {
      z_i[0] ^= v_i[0];
      z_i[1] ^= v_i[1];
      z_i[2] ^= v_i[2];
      z_i[3] ^= v_i[3];
    }

    // if LSB(V_i) is 1, V_i = V_i >> 1
    // else V_i = (V_i >> 1) ^ R
    this.pow(v_i, v_i);
  }

  return z_i;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.pow"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>pow (x, out)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.pow)
- description and source-code
```javascript
pow = function (x, out) {
  // if LSB(x) is 1, x = x >>> 1
  // else x = (x >>> 1) ^ R
  var lsb = x[3] & 1;

  // always do x >>> 1:
  // starting with the rightmost integer, shift each integer to the right
  // one bit, pulling in the bit from the integer to the left as its top
  // most bit (do this for the last 3 integers)
  for(var i = 3; i > 0; --i) {
    out[i] = (x[i] >>> 1) | ((x[i - 1] & 1) << 31);
  }
  // shift the first integer normally
  out[0] = x[0] >>> 1;

  // if lsb was not set, then polynomial had a degree of 127 and doesn't
  // need to divided; otherwise, XOR with R to find the remainder; we only
  // need to XOR the first integer since R technically ends w/120 zero bits
  if(lsb) {
    out[0] ^= this._R;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.start)
- description and source-code
```javascript
start = function (options) {
  if(!('iv' in options)) {
    throw new Error('Invalid IV parameter.');
  }
  // ensure IV is a byte buffer
  var iv = forge.util.createBuffer(options.iv);

  // no ciphered data processed yet
  this._cipherLength = 0;

  // default additional data is none
  var additionalData;
  if('additionalData' in options) {
    additionalData = forge.util.createBuffer(options.additionalData);
  } else {
    additionalData = forge.util.createBuffer();
  }

  // default tag length is 128 bits
  if('tagLength' in options) {
    this._tagLength = options.tagLength;
  } else {
    this._tagLength = 128;
  }

  // if tag is given, ensure tag matches tag length
  this._tag = null;
  if(options.decrypt) {
    // save tag to check later
    this._tag = forge.util.createBuffer(options.tag).getBytes();
    if(this._tag.length !== (this._tagLength / 8)) {
      throw new Error('Authentication tag does not match tag length.');
    }
  }

  // create tmp storage for hash calculation
  this._hashBlock = new Array(this._ints);

  // no tag generated yet
  this.tag = null;

  // generate hash subkey
  // (apply block cipher to "zero" block)
  this._hashSubkey = new Array(this._ints);
  this.cipher.encrypt([0, 0, 0, 0], this._hashSubkey);

  // generate table M
  // use 4-bit tables (32 component decomposition of a 16 byte value)
  // 8-bit tables take more space and are known to have security
  // vulnerabilities (in native implementations)
  this.componentBits = 4;
  this._m = this.generateHashTable(this._hashSubkey, this.componentBits);

  // Note: support IV length different from 96 bits? (only supporting
  // 96 bits is recommended by NIST SP-800-38D)
  // generate J_0
  var ivLength = iv.length();
  if(ivLength === 12) {
    // 96-bit IV
    this._j0 = [iv.getInt32(), iv.getInt32(), iv.getInt32(), 1];
  } else {
    // IV is NOT 96-bits
    this._j0 = [0, 0, 0, 0];
    while(iv.length() > 0) {
      this._j0 = this.ghash(
        this._hashSubkey, this._j0,
        [iv.getInt32(), iv.getInt32(), iv.getInt32(), iv.getInt32()]);
    }
    this._j0 = this.ghash(
      this._hashSubkey, this._j0, [0, 0].concat(from64To32(ivLength * 8)));
  }

  // generate ICB (initial counter block)
  this._inBlock = this._j0.slice(0);
  inc32(this._inBlock);
  this._partialBytes = 0;

  // consume authentication data
  additionalData = forge.util.createBuffer(additionalData);
  // save additional data length as a BE 64-bit number
  this._aDataLength = from64To32(additionalData.length() * 8);
  // pad additional data to 128 bit (16 byte) block size
  var overflow = additionalData.length() % this.blockSize;
  if(overflow) {
    additionalData.fillWithByte(0, this.blockSize - overflow);
  }
  this._s = [0, 0, 0, 0];
  while(additionalData.length() > 0) {
    this._s = this.ghash(this._hashSubkey, this._s, [
      additionalData.getInt32(),
      additionalData.getInt32(),
      additionalData.getInt32(),
      additionalData.getInt32()
    ]);
  }
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.gcm.prototype.tableMultiply"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.gcm.prototype.</span>tableMultiply (x)](#apidoc.element.node-forge.cipher.modes.gcm.prototype.tableMultiply)
- description and source-code
```javascript
tableMultiply = function (x) {
  // assumes 4-bit tables are used
  var z = [0, 0, 0, 0];
  for(var i = 0; i < 32; ++i) {
    var idx = (i / 8) | 0;
    var x_i = (x[idx] >>> ((7 - (i % 8)) * 4)) & 0xF;
    var ah = this._m[i][x_i];
    z[0] ^= ah[0];
    z[1] ^= ah[1];
    z[2] ^= ah[2];
    z[3] ^= ah[3];
  }
  return z;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.cipher.modes.ofb.prototype"></a>[module node-forge.cipher.modes.ofb.prototype](#apidoc.module.node-forge.cipher.modes.ofb.prototype)

#### <a name="apidoc.element.node-forge.cipher.modes.ofb.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ofb.prototype.</span>decrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ofb.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (input, output, finish) {
  // not enough input to encrypt
  var inputLength = input.length();
  if(input.length() === 0) {
    return true;
  }

  // encrypt block (OFB always uses encryption mode)
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output and update next input
    for(var i = 0; i < this._ints; ++i) {
      output.putInt32(input.getInt32() ^ this._outBlock[i]);
      this._inBlock[i] = this._outBlock[i];
    }
    return;
  }

  // handle partial block
  var partialBytes = (this.blockSize - inputLength) % this.blockSize;
  if(partialBytes > 0) {
    partialBytes = this.blockSize - partialBytes;
  }

  // XOR input with output
  this._partialOutput.clear();
  for(var i = 0; i < this._ints; ++i) {
    this._partialOutput.putInt32(input.getInt32() ^ this._outBlock[i]);
  }

  if(partialBytes > 0) {
    // block still incomplete, restore input buffer
    input.read -= this.blockSize;
  } else {
    // block complete, update input block
    for(var i = 0; i < this._ints; ++i) {
      this._inBlock[i] = this._outBlock[i];
    }
  }

  // skip any previous partial bytes
  if(this._partialBytes > 0) {
    this._partialOutput.getBytes(this._partialBytes);
  }

  if(partialBytes > 0 && !finish) {
    output.putBytes(this._partialOutput.getBytes(
      partialBytes - this._partialBytes));
    this._partialBytes = partialBytes;
    return true;
  }

  output.putBytes(this._partialOutput.getBytes(
    inputLength - this._partialBytes));
  this._partialBytes = 0;
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ofb.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ofb.prototype.</span>encrypt (input, output, finish)](#apidoc.element.node-forge.cipher.modes.ofb.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (input, output, finish) {
  // not enough input to encrypt
  var inputLength = input.length();
  if(input.length() === 0) {
    return true;
  }

  // encrypt block (OFB always uses encryption mode)
  this.cipher.encrypt(this._inBlock, this._outBlock);

  // handle full block
  if(this._partialBytes === 0 && inputLength >= this.blockSize) {
    // XOR input with output and update next input
    for(var i = 0; i < this._ints; ++i) {
      output.putInt32(input.getInt32() ^ this._outBlock[i]);
      this._inBlock[i] = this._outBlock[i];
    }
    return;
  }

  // handle partial block
  var partialBytes = (this.blockSize - inputLength) % this.blockSize;
  if(partialBytes > 0) {
    partialBytes = this.blockSize - partialBytes;
  }

  // XOR input with output
  this._partialOutput.clear();
  for(var i = 0; i < this._ints; ++i) {
    this._partialOutput.putInt32(input.getInt32() ^ this._outBlock[i]);
  }

  if(partialBytes > 0) {
    // block still incomplete, restore input buffer
    input.read -= this.blockSize;
  } else {
    // block complete, update input block
    for(var i = 0; i < this._ints; ++i) {
      this._inBlock[i] = this._outBlock[i];
    }
  }

  // skip any previous partial bytes
  if(this._partialBytes > 0) {
    this._partialOutput.getBytes(this._partialBytes);
  }

  if(partialBytes > 0 && !finish) {
    output.putBytes(this._partialOutput.getBytes(
      partialBytes - this._partialBytes));
    this._partialBytes = partialBytes;
    return true;
  }

  output.putBytes(this._partialOutput.getBytes(
    inputLength - this._partialBytes));
  this._partialBytes = 0;
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.cipher.modes.ofb.prototype.start"></a>[function <span class="apidocSignatureSpan">node-forge.cipher.modes.ofb.prototype.</span>start (options)](#apidoc.element.node-forge.cipher.modes.ofb.prototype.start)
- description and source-code
```javascript
start = function (options) {
  if(!('iv' in options)) {
    throw new Error('Invalid IV parameter.');
  }
  // use IV as first input
  this._iv = transformIV(options.iv);
  this._inBlock = this._iv.slice(0);
  this._partialBytes = 0;
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```



# <a name="apidoc.module.node-forge.debug"></a>[module node-forge.debug](#apidoc.module.node-forge.debug)

#### <a name="apidoc.element.node-forge.debug.clear"></a>[function <span class="apidocSignatureSpan">node-forge.debug.</span>clear (cat, name)](#apidoc.element.node-forge.debug.clear)
- description and source-code
```javascript
clear = function (cat, name) {
  if(typeof(cat) === 'undefined') {
    forge.debug.storage = {};
  } else if(cat in forge.debug.storage) {
    if(typeof(name) === 'undefined') {
      delete forge.debug.storage[cat];
    } else {
      delete forge.debug.storage[cat][name];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.debug.get"></a>[function <span class="apidocSignatureSpan">node-forge.debug.</span>get (cat, name)](#apidoc.element.node-forge.debug.get)
- description and source-code
```javascript
get = function (cat, name) {
  var rval;
  if(typeof(cat) === 'undefined') {
    rval = forge.debug.storage;
  } else if(cat in forge.debug.storage) {
    if(typeof(name) === 'undefined') {
      rval = forge.debug.storage[cat];
    } else {
      rval = forge.debug.storage[cat][name];
    }
  }
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.debug.set"></a>[function <span class="apidocSignatureSpan">node-forge.debug.</span>set (cat, name, data)](#apidoc.element.node-forge.debug.set)
- description and source-code
```javascript
set = function (cat, name, data) {
  if(!(cat in forge.debug.storage)) {
    forge.debug.storage[cat] = {};
  }
  forge.debug.storage[cat][name] = data;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.des"></a>[module node-forge.des](#apidoc.module.node-forge.des)

#### <a name="apidoc.element.node-forge.des.Algorithm"></a>[function <span class="apidocSignatureSpan">node-forge.des.</span>Algorithm (name, mode)](#apidoc.element.node-forge.des.Algorithm)
- description and source-code
```javascript
Algorithm = function (name, mode) {
  var self = this;
  self.name = name;
  self.mode = new mode({
    blockSize: 8,
    cipher: {
      encrypt: function(inBlock, outBlock) {
        return _updateBlock(self._keys, inBlock, outBlock, false);
      },
      decrypt: function(inBlock, outBlock) {
        return _updateBlock(self._keys, inBlock, outBlock, true);
      }
    }
  });
  self._init = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.des.createDecryptionCipher"></a>[function <span class="apidocSignatureSpan">node-forge.des.</span>createDecryptionCipher (key, mode)](#apidoc.element.node-forge.des.createDecryptionCipher)
- description and source-code
```javascript
createDecryptionCipher = function (key, mode) {
  return _createCipher({
    key: key,
    output: null,
    decrypt: true,
    mode: mode
  });
}
```
- example usage
```shell
...
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes
var cipher = forge.rc2.createDecryptionCipher(key);
cipher.start(iv);
cipher.update(encrypted);
cipher.finish();
// outputs decrypted hex
console.log(cipher.output.toHex());
'''
...
```

#### <a name="apidoc.element.node-forge.des.createEncryptionCipher"></a>[function <span class="apidocSignatureSpan">node-forge.des.</span>createEncryptionCipher (key, mode)](#apidoc.element.node-forge.des.createEncryptionCipher)
- description and source-code
```javascript
createEncryptionCipher = function (key, mode) {
  return _createCipher({
    key: key,
    output: null,
    decrypt: false,
    mode: mode
  });
}
```
- example usage
```shell
...

'''js
// generate a random key and IV
var key = forge.random.getBytesSync(16);
var iv = forge.random.getBytesSync(8);

// encrypt some bytes
var cipher = forge.rc2.createEncryptionCipher(key);
cipher.start(iv);
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());
...
```

#### <a name="apidoc.element.node-forge.des.startDecrypting"></a>[function <span class="apidocSignatureSpan">node-forge.des.</span>startDecrypting (key, iv, output, mode)](#apidoc.element.node-forge.des.startDecrypting)
- description and source-code
```javascript
startDecrypting = function (key, iv, output, mode) {
  var cipher = _createCipher({
    key: key,
    output: output,
    decrypt: true,
    mode: mode || (iv === null ? 'ECB' : 'CBC')
  });
  cipher.start(iv);
  return cipher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.des.startEncrypting"></a>[function <span class="apidocSignatureSpan">node-forge.des.</span>startEncrypting (key, iv, output, mode)](#apidoc.element.node-forge.des.startEncrypting)
- description and source-code
```javascript
startEncrypting = function (key, iv, output, mode) {
  var cipher = _createCipher({
    key: key,
    output: output,
    decrypt: false,
    mode: mode || (iv === null ? 'ECB' : 'CBC')
  });
  cipher.start(iv);
  return cipher;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.des.Algorithm"></a>[module node-forge.des.Algorithm](#apidoc.module.node-forge.des.Algorithm)

#### <a name="apidoc.element.node-forge.des.Algorithm.Algorithm"></a>[function <span class="apidocSignatureSpan">node-forge.des.</span>Algorithm (name, mode)](#apidoc.element.node-forge.des.Algorithm.Algorithm)
- description and source-code
```javascript
Algorithm = function (name, mode) {
  var self = this;
  self.name = name;
  self.mode = new mode({
    blockSize: 8,
    cipher: {
      encrypt: function(inBlock, outBlock) {
        return _updateBlock(self._keys, inBlock, outBlock, false);
      },
      decrypt: function(inBlock, outBlock) {
        return _updateBlock(self._keys, inBlock, outBlock, true);
      }
    }
  });
  self._init = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.des.Algorithm.prototype"></a>[module node-forge.des.Algorithm.prototype](#apidoc.module.node-forge.des.Algorithm.prototype)

#### <a name="apidoc.element.node-forge.des.Algorithm.prototype.initialize"></a>[function <span class="apidocSignatureSpan">node-forge.des.Algorithm.prototype.</span>initialize (options)](#apidoc.element.node-forge.des.Algorithm.prototype.initialize)
- description and source-code
```javascript
initialize = function (options) {
  if(this._init) {
    return;
  }

  var key = forge.util.createBuffer(options.key);
  if(this.name.indexOf('3DES') === 0) {
    if(key.length() !== 24) {
      throw new Error('Invalid Triple-DES key size: ' + key.length() * 8);
    }
  }

  // do key expansion to 16 or 48 subkeys (single or triple DES)
  this._keys = _createKeys(key);
  this._init = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.hmac"></a>[module node-forge.hmac](#apidoc.module.node-forge.hmac)

#### <a name="apidoc.element.node-forge.hmac.create"></a>[function <span class="apidocSignatureSpan">node-forge.hmac.</span>create ()](#apidoc.element.node-forge.hmac.create)
- description and source-code
```javascript
create = function () {
  // the hmac key to use
  var _key = null;

  // the message digest to use
  var _md = null;

  // the inner padding
  var _ipadding = null;

  // the outer padding
  var _opadding = null;

  // hmac context
  var ctx = {};

<span class="apidocCodeCommentSpan">  /**
   * Starts or restarts the HMAC with the given key and message digest.
   *
   * @param md the message digest to use, null to reuse the previous one,
   *           a string to use builtin 'sha1', 'md5', 'sha256'.
   * @param key the key to use as a string, array of bytes, byte buffer,
   *           or null to reuse the previous key.
   */
</span>  ctx.start = function(md, key) {
    if(md !== null) {
      if(typeof md === 'string') {
        // create builtin message digest
        md = md.toLowerCase();
        if(md in forge.md.algorithms) {
          _md = forge.md.algorithms[md].create();
        } else {
          throw new Error('Unknown hash algorithm "' + md + '"');
        }
      } else {
        // store message digest
        _md = md;
      }
    }

    if(key === null) {
      // reuse previous key
      key = _key;
    } else {
      if(typeof key === 'string') {
        // convert string into byte buffer
        key = forge.util.createBuffer(key);
      } else if(forge.util.isArray(key)) {
        // convert byte array into byte buffer
        var tmp = key;
        key = forge.util.createBuffer();
        for(var i = 0; i < tmp.length; ++i) {
          key.putByte(tmp[i]);
        }
      }

      // if key is longer than blocksize, hash it
      var keylen = key.length();
      if(keylen > _md.blockLength) {
        _md.start();
        _md.update(key.bytes());
        key = _md.digest();
      }

      // mix key into inner and outer padding
      // ipadding = [0x36 * blocksize] ^ key
      // opadding = [0x5C * blocksize] ^ key
      _ipadding = forge.util.createBuffer();
      _opadding = forge.util.createBuffer();
      keylen = key.length();
      for(var i = 0; i < keylen; ++i) {
        var tmp = key.at(i);
        _ipadding.putByte(0x36 ^ tmp);
        _opadding.putByte(0x5C ^ tmp);
      }

      // if key is shorter than blocksize, add additional padding
      if(keylen < _md.blockLength) {
        var tmp = _md.blockLength - keylen;
        for(var i = 0; i < tmp; ++i) {
          _ipadding.putByte(0x36);
          _opadding.putByte(0x5C);
        }
      }
      _key = key;
      _ipadding = _ipadding.bytes();
      _opadding = _opadding.bytes();
    }

    // digest is done like so: hash(opadding | hash(ipadding | message))

    // prepare to do inner hash
    // hash(ipadding | message)
    _md.start();
    _md.update(_ipadding);
  };

  /**
   * Updates the HMAC with the given message bytes.
   *
   * @param bytes the bytes to update with.
   */
  ctx.update = function(bytes) {
    _md.update(bytes);
  };

  /**
   * Produces the Message Authentication Code (MAC).
   *
   * @return a byte buffer containing the digest value.
   */
  ctx.getMac = function() {
    // digest is done like so: hash(opadding | hash(ipadding | message))
    // here we do the outer hashing
    var inner = _md.digest().bytes();
    _md.start();
    _md.update(_opadding);
    _md.update(inner);
    return _md.digest();
  };
  // alias for getMac
  ctx.digest = ctx.getMac;

  return ctx;
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.http"></a>[module node-forge.http](#apidoc.module.node-forge.http)

#### <a name="apidoc.element.node-forge.http.createClient"></a>[function <span class="apidocSignatureSpan">node-forge.http.</span>createClient (options)](#apidoc.element.node-forge.http.createClient)
- description and source-code
```javascript
createClient = function (options) {
  // create CA store to share with all TLS connections
  var caStore = null;
  if(options.caCerts) {
    caStore = forge.pki.createCaStore(options.caCerts);
  }

  // get scheme, host, and port from url
  options.url = (options.url ||
    window.location.protocol + '//' + window.location.host);
  var url = http.parseUrl(options.url);
  if(!url) {
    var error = new Error('Invalid url.');
    error.details = {url: options.url};
    throw error;
  }

  // default to 1 connection
  options.connections = options.connections || 1;

  // create client
  var sp = options.socketPool;
  var client = {
    // url
    url: url,
    // socket pool
    socketPool: sp,
    // the policy port to use
    policyPort: options.policyPort,
    // policy url to use
    policyUrl: options.policyUrl,
    // queue of requests to service
    requests: [],
    // all sockets
    sockets: [],
    // idle sockets
    idle: [],
    // whether or not the connections are secure
    secure: (url.scheme === 'https'),
    // cookie jar (key'd off of name and then path, there is only 1 domain
    // and one setting for secure per client so name+path is unique)
    cookies: {},
    // default to flash storage of cookies
    persistCookies: (typeof(options.persistCookies) === 'undefined') ?
      true : options.persistCookies
  };

  // add client to debug storage
  if(forge.debug) {
    forge.debug.get('forge.http', 'clients').push(client);
  }

  // load cookies from disk
  _loadCookies(client);

<span class="apidocCodeCommentSpan">  /**
   * A default certificate verify function that checks a certificate common
   * name against the client's URL host.
   *
   * @param c the TLS connection.
   * @param verified true if cert is verified, otherwise alert number.
   * @param depth the chain depth.
   * @param certs the cert chain.
   *
   * @return true if verified and the common name matches the host, error
   *         otherwise.
   */
</span>  var _defaultCertificateVerify = function(c, verified, depth, certs) {
    if(depth === 0 && verified === true) {
      // compare common name to url host
      var cn = certs[depth].subject.getField('CN');
      if(cn === null || client.url.host !== cn.value) {
        verified = {
          message: 'Certificate common name does not match url host.'
        };
      }
    }
    return verified;
  };

  // determine if TLS is used
  var tlsOptions = null;
  if(client.secure) {
    tlsOptions = {
      caStore: caStore,
      cipherSuites: options.cipherSuites || null,
      virtualHost: options.virtualHost || url.host,
      verify: options.verify || _defaultCertificateVerify,
      getCertificate: options.getCertificate || null,
      getPrivateKey: options.getPrivateKey || null,
      getSignature: options.getSignature || null,
      prime: options.primeTlsSockets || false
    };

    // if socket pool uses a flash api, then add deflate support to TLS
    if(sp.flashApi !== null) {
      tlsOptions.deflate = function(bytes) {
        // strip 2 byte zlib header and 4 byte trailer
        return forge.util.deflate(sp.flashApi, bytes, true);
      };
      tlsOptions.inflate = function(bytes) {
        return forge.util.inflate(sp.flashApi, bytes, true);
      };
    }
  }

  // create and initialize sockets
  for(var i = 0; i < options.connections; ++i) {
    _initSocket(client, sp.createSocket(), tlsOptions);
  }

  /**
   * Sends a request. A method 'abort' will be set on the request that
   * can be called to attempt to abort the request.
   *
   * @param options:
   *          request: the request to send.
   *          connected: a callback for when the connection is open.
   *          closed: a callback for when the connection is closed.
   *          headerReady: a callback for when the response header arrives.
   *          bodyReady: a callback for when the response body arrives.
   *          error: a callback for if an error occurs.
   */
  client.send = function(options) {
    // add host header if not set
    if(options.request.getField('Host') === null) {
      options.request.setField('Host', client.url.fullHost);
    } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.http.createRequest"></a>[function <span class="apidocSignatureSpan">node-forge.http.</span>createRequest (options)](#apidoc.element.node-forge.http.createRequest)
- description and source-code
```javascript
createRequest = function (options) {
  options = options || {};
  var request = _createHeader();
  request.version = options.version || 'HTTP/1.1';
  request.method = options.method || null;
  request.path = options.path || null;
  request.body = options.body || null;
  request.bodyDeflated = false;
  request.flashApi = null;

  // add custom headers
  var headers = options.headers || [];
  if(!forge.util.isArray(headers)) {
    headers = [headers];
  }
  for(var i = 0; i < headers.length; ++i) {
    for(var name in headers[i]) {
      request.appendField(name, headers[i][name]);
    }
  }

<span class="apidocCodeCommentSpan">  /**
   * Adds a cookie to the request 'Cookie' header.
   *
   * @param cookie a cookie to add.
   */
</span>  request.addCookie = function(cookie) {
    var value = '';
    var field = request.getField('Cookie');
    if(field !== null) {
      // separate cookies by semi-colons
      value = field + '; ';
    }

    // get current time in utc seconds
    var now = _getUtcTime(new Date());

    // output cookie name and value
    value += cookie.name + '=' + cookie.value;
    request.setField('Cookie', value);
  };

  /**
   * Converts an http request into a string that can be sent as an
   * HTTP request. Does not include any data.
   *
   * @return the string representation of the request.
   */
  request.toString = function() {
    /* Sample request header:
      GET /some/path/?query HTTP/1.1
      Host: www.someurl.com
      Connection: close
      Accept-Encoding: deflate
      Accept: image/gif, text/html
      User-Agent: Mozilla 4.0
     */

    // set default headers
    if(request.getField('User-Agent') === null) {
      request.setField('User-Agent', 'forge.http 1.0');
    }
    if(request.getField('Accept') === null) {
      request.setField('Accept', '*/*');
    }
    if(request.getField('Connection') === null) {
      request.setField('Connection', 'keep-alive');
      request.setField('Keep-Alive', '115');
    }

    // add Accept-Encoding if not specified
    if(request.flashApi !== null &&
      request.getField('Accept-Encoding') === null) {
      request.setField('Accept-Encoding', 'deflate');
    }

    // if the body isn't null, deflate it if its larger than 100 bytes
    if(request.flashApi !== null && request.body !== null &&
      request.getField('Content-Encoding') === null &&
      !request.bodyDeflated && request.body.length > 100) {
      // use flash to compress data
      request.body = forge.util.deflate(request.flashApi, request.body);
      request.bodyDeflated = true;
      request.setField('Content-Encoding', 'deflate');
      request.setField('Content-Length', request.body.length);
    } else if(request.body !== null) {
      // set content length for body
      request.setField('Content-Length', request.body.length);
    }

    // build start line
    var rval =
      request.method.toUpperCase() + ' ' + request.path + ' ' +
      request.version + '\r\n';

    // add each header
    for(var name in request.fields) {
      var fields = request.fields[name];
      for(var i = 0; i < fields.length; ++i) {
        rval += name + ': ' + fields[i] + '\r\n';
      }
    }
    // final terminating CRLF
    rval += '\r\n';

    return rval;
  };

  return request;
}
```
- example usage
```shell
...
Provides a native [JavaScript][] mini-implementation of an http client that
uses pooled sockets.

__Examples__

'''js
// create an HTTP GET request
var request = forge.http.createRequest({method: 'GET', path: url.path});

// send the request somewhere
sendSomehow(request.toString());

// receive response
var buffer = forge.util.createBuffer();
var response = forge.http.createResponse();
...
```

#### <a name="apidoc.element.node-forge.http.createResponse"></a>[function <span class="apidocSignatureSpan">node-forge.http.</span>createResponse ()](#apidoc.element.node-forge.http.createResponse)
- description and source-code
```javascript
createResponse = function () {
  // private vars
  var _first = true;
  var _chunkSize = 0;
  var _chunksFinished = false;

  // create response
  var response = _createHeader();
  response.version = null;
  response.code = 0;
  response.message = null;
  response.body = null;
  response.headerReceived = false;
  response.bodyReceived = false;
  response.flashApi = null;

<span class="apidocCodeCommentSpan">  /**
   * Reads a line that ends in CRLF from a byte buffer.
   *
   * @param b the byte buffer.
   *
   * @return the line or null if none was found.
   */
</span>  var _readCrlf = function(b) {
    var line = null;
    var i = b.data.indexOf('\r\n', b.read);
    if(i != -1) {
      // read line, skip CRLF
      line = b.getBytes(i - b.read);
      b.getBytes(2);
    }
    return line;
  };

  /**
   * Parses a header field and appends it to the response.
   *
   * @param line the header field line.
   */
  var _parseHeader = function(line) {
    var tmp = line.indexOf(':');
    var name = line.substring(0, tmp++);
    response.appendField(
      name, (tmp < line.length) ? line.substring(tmp) : '');
  };

  /**
   * Reads an http response header from a buffer of bytes.
   *
   * @param b the byte buffer to parse the header from.
   *
   * @return true if the whole header was read, false if not.
   */
  response.readHeader = function(b) {
    // read header lines (each ends in CRLF)
    var line = '';
    while(!response.headerReceived && line !== null) {
      line = _readCrlf(b);
      if(line !== null) {
        // parse first line
        if(_first) {
          _first = false;
          var tmp = line.split(' ');
          if(tmp.length >= 3) {
            response.version = tmp[0];
            response.code = parseInt(tmp[1], 10);
            response.message = tmp.slice(2).join(' ');
          } else {
            // invalid header
            var error = new Error('Invalid http response header.');
            error.details = {'line': line};
            throw error;
          }
        } else if(line.length === 0) {
          // handle final line, end of header
          response.headerReceived = true;
        } else {
          _parseHeader(line);
        }
      }
    }

    return response.headerReceived;
  };

  /**
   * Reads some chunked http response entity-body from the given buffer of
   * bytes.
   *
   * @param b the byte buffer to read from.
   *
   * @return true if the whole body was read, false if not.
   */
  var _readChunkedBody = function(b) {
    /* Chunked transfer-encoding sends data in a series of chunks,
      followed by a set of 0-N http trailers.
      The format is as follows:

      chunk-size (in hex) CRLF
      chunk data (with "chunk-size" many bytes) CRLF
      ... (N many chunks)
      chunk-size (of 0 indicating the last chunk) CRLF
      N many http trailers followed by CRLF
      blank line + CRLF (terminates the trailers)

      If there are no http trailers, then after the chunk-size of 0,
      there is still a single CRLF (indicating the blank line + CRLF
      that terminates the trailers). In other words, you always terminate
      the trailers with blank line + CRLF, regardless of 0-N trailers. */

      /* From RFC-2616, section 3.6.1, here is the pseudo-code for
      implementing chunked transfer-encoding:

      length := 0
      read chunk-size, chunk-extension (if any) and CRLF
      while (chunk-size > 0) {
        read chunk-data and CRLF
        append chunk-data to entity-body
        length := length + chunk-size
        read chunk-size and CRLF
      }
      read entity-header
      while (entity-header not empty) {
        append entity-header to existing header fields
        read entity-header
      }
      Content-Length := length
      Remove "chunked" from Transfer-Encoding
    */

    var line = '';
    while(line !== null && b.length() > 0) {
      // if in the process of reading a chunk
      if(_chunkSize > 0) {
        // if there are not enough bytes to read chunk and its
        // trailing CRLF,  we must wait for more data to be received
        if(_chunkSize + 2 > b.length()) {
          break; ...
```
- example usage
```shell
...
var request = forge.http.createRequest({method: 'GET', path: url.path});

// send the request somewhere
sendSomehow(request.toString());

// receive response
var buffer = forge.util.createBuffer();
var response = forge.http.createResponse();
var someAsyncDataHandler = function(bytes) {
if(!response.bodyReceived) {
  buffer.putBytes(bytes);
  if(!response.headerReceived) {
    if(response.readHeader(buffer)) {
      console.log('HTTP response header: ' + response.toString());
    }
...
```

#### <a name="apidoc.element.node-forge.http.parseUrl"></a>[function <span class="apidocSignatureSpan">node-forge.http.</span>parseUrl (str)](#apidoc.element.node-forge.http.parseUrl)
- description and source-code
```javascript
parseUrl = function (str) {
  // FIXME: this regex looks a bit broken
  var regex = /^(https?):\/\/([^:&^\/]*):?(\d*)(.*)$/g;
  regex.lastIndex = 0;
  var m = regex.exec(str);
  var url = (m === null) ? null : {
    full: str,
    scheme: m[1],
    host: m[2],
    port: m[3],
    path: m[4]
  };
  if(url) {
    url.fullHost = url.host;
    if(url.port) {
      if(url.port !== 80 && url.scheme === 'http') {
        url.fullHost += ':' + url.port;
      } else if(url.port !== 443 && url.scheme === 'https') {
        url.fullHost += ':' + url.port;
      }
    } else if(url.scheme === 'http') {
      url.port = 80;
    } else if(url.scheme === 'https') {
      url.port = 443;
    }
    url.full = url.scheme + '://' + url.fullHost;
  }
  return url;
}
```
- example usage
```shell
...

// convert a Node.js Buffer into a forge buffer
// make sure you specify the encoding as 'binary'
var nodeBuffer = new Buffer();
var forgeBuffer = forge.util.createBuffer(nodeBuffer.toString('binary'));

// parse a URL
var parsed = forge.util.parseUrl('http://example.com/foo?bar=baz');
// parsed.scheme, parsed.host, parsed.port, parsed.path, parsed.fullHost
'''

<a name="log" />
### Logging

Provides logging to a javascript console using various categories and
...
```

#### <a name="apidoc.element.node-forge.http.withinCookieDomain"></a>[function <span class="apidocSignatureSpan">node-forge.http.</span>withinCookieDomain (url, cookie)](#apidoc.element.node-forge.http.withinCookieDomain)
- description and source-code
```javascript
withinCookieDomain = function (url, cookie) {
  var rval = false;

  // cookie may be null, a cookie object, or a domain string
  var domain = (cookie === null || typeof cookie === 'string') ?
    cookie : cookie.domain;

  // any domain will do
  if(domain === null) {
    rval = true;
  } else if(domain.charAt(0) === '.') {
    // ensure domain starts with a '.'
    // parse URL as necessary
    if(typeof url === 'string') {
      url = http.parseUrl(url);
    }

    // add '.' to front of URL host to match against domain
    var host = '.' + url.host;

    // if the host ends with domain then it falls within it
    var idx = host.lastIndexOf(domain);
    if(idx !== -1 && (idx + domain.length === host.length)) {
      rval = true;
    }
  }

  return rval;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.jsbn"></a>[module node-forge.jsbn](#apidoc.module.node-forge.jsbn)

#### <a name="apidoc.element.node-forge.jsbn.BigInteger"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.</span>BigInteger (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger)
- description and source-code
```javascript
function BigInteger(a, b, c) {
  this.data = [];
  if(a != null)
    if("number" == typeof a) this.fromNumber(a,b,c);
    else if(b == null && "string" != typeof a) this.fromString(a,256);
    else this.fromString(a,b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.jsbn.BigInteger"></a>[module node-forge.jsbn.BigInteger](#apidoc.module.node-forge.jsbn.BigInteger)

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.BigInteger"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.</span>BigInteger (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger.BigInteger)
- description and source-code
```javascript
function BigInteger(a, b, c) {
  this.data = [];
  if(a != null)
    if("number" == typeof a) this.fromNumber(a,b,c);
    else if(b == null && "string" != typeof a) this.fromString(a,256);
    else this.fromString(a,b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.jsbn.BigInteger.prototype"></a>[module node-forge.jsbn.BigInteger.prototype](#apidoc.module.node-forge.jsbn.BigInteger.prototype)

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.abs"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>abs ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.abs)
- description and source-code
```javascript
function bnAbs() { return (this.s<0)?this.negate():this; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.add"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>add (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.add)
- description and source-code
```javascript
function bnAdd(a) { var r = nbi(); this.addTo(a,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.addTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>addTo (a, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.addTo)
- description and source-code
```javascript
function bnpAddTo(a, r) {
var i = 0, c = 0, m = Math.min(a.t,this.t);
while(i < m) {
 c += this.data[i]+a.data[i];
 r.data[i++] = c&this.DM;
 c >>= this.DB;
}
if(a.t < this.t) {
 c += a.s;
 while(i < this.t) {
   c += this.data[i];
   r.data[i++] = c&this.DM;
   c >>= this.DB;
 }
 c += this.s;
} else {
 c += this.s;
 while(i < a.t) {
   c += a.data[i];
   r.data[i++] = c&this.DM;
   c >>= this.DB;
 }
 c += a.s;
}
r.s = (c<0)?-1:0;
if(c > 0) r.data[i++] = c;
else if(c < -1) r.data[i++] = this.DV+c;
r.t = i;
r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.am"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>am (i, x, w, j, c, n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.am)
- description and source-code
```javascript
function am3(i, x, w, j, c, n) {
  var xl = x&0x3fff, xh = x>>14;
  while(--n >= 0) {
    var l = this.data[i]&0x3fff;
    var h = this.data[i++]>>14;
    var m = xh*l+h*xl;
    l = xl*l+((m&0x3fff)<<14)+w.data[j]+c;
    c = (l>>28)+(m>>14)+xh*h;
    w.data[j++] = l&0xfffffff;
  }
  return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.and"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>and (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.and)
- description and source-code
```javascript
function bnAnd(a) { var r = nbi(); this.bitwiseTo(a,op_and,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.andNot"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>andNot (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.andNot)
- description and source-code
```javascript
function bnAndNot(a) { var r = nbi(); this.bitwiseTo(a,op_andnot,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.bitCount"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>bitCount ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.bitCount)
- description and source-code
```javascript
function bnBitCount() {
var r = 0, x = this.s&this.DM;
for(var i = 0; i < this.t; ++i) r += cbit(this.data[i]^x);
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.bitLength"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>bitLength ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.bitLength)
- description and source-code
```javascript
function bnBitLength() {
  if(this.t <= 0) return 0;
  return this.DB*(this.t-1)+nbits(this.data[this.t-1]^(this.s&this.DM));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.bitwiseTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>bitwiseTo (a, op, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.bitwiseTo)
- description and source-code
```javascript
function bnpBitwiseTo(a, op, r) {
var i, f, m = Math.min(a.t,this.t);
for(i = 0; i < m; ++i) r.data[i] = op(this.data[i],a.data[i]);
if(a.t < this.t) {
 f = a.s&this.DM;
 for(i = m; i < this.t; ++i) r.data[i] = op(this.data[i],f);
 r.t = this.t;
} else {
 f = this.s&this.DM;
 for(i = m; i < a.t; ++i) r.data[i] = op(f,a.data[i]);
 r.t = a.t;
}
r.s = op(this.s,a.s);
r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.byteValue"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>byteValue ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.byteValue)
- description and source-code
```javascript
function bnByteValue() { return (this.t==0)?this.s:(this.data[0]<<24)>>24; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.changeBit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>changeBit (n, op)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.changeBit)
- description and source-code
```javascript
function bnpChangeBit(n, op) {
var r = BigInteger.ONE.shiftLeft(n);
this.bitwiseTo(r,op,r);
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.chunkSize"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>chunkSize (r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.chunkSize)
- description and source-code
```javascript
function bnpChunkSize(r) { return Math.floor(Math.LN2*this.DB/Math.log(r)); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.clamp"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>clamp ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.clamp)
- description and source-code
```javascript
function bnpClamp() {
  var c = this.s&this.DM;
  while(this.t > 0 && this.data[this.t-1] == c) --this.t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.clearBit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>clearBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.clearBit)
- description and source-code
```javascript
function bnClearBit(n) { return this.changeBit(n,op_andnot); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.clone"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>clone ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.clone)
- description and source-code
```javascript
function bnClone() { var r = nbi(); this.copyTo(r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.compareTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>compareTo (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.compareTo)
- description and source-code
```javascript
function bnCompareTo(a) {
  var r = this.s-a.s;
  if(r != 0) return r;
  var i = this.t;
  r = i-a.t;
  if(r != 0) return (this.s<0)?-r:r;
  while(--i >= 0) if((r=this.data[i]-a.data[i]) != 0) return r;
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.copyTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>copyTo (r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.copyTo)
- description and source-code
```javascript
function bnpCopyTo(r) {
  for(var i = this.t-1; i >= 0; --i) r.data[i] = this.data[i];
  r.t = this.t;
  r.s = this.s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.dAddOffset"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>dAddOffset (n, w)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.dAddOffset)
- description and source-code
```javascript
function bnpDAddOffset(n, w) {
if(n == 0) return;
while(this.t <= w) this.data[this.t++] = 0;
this.data[w] += n;
while(this.data[w] >= this.DV) {
 this.data[w] -= this.DV;
 if(++w >= this.t) this.data[this.t++] = 0;
 ++this.data[w];
}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.dMultiply"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>dMultiply (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.dMultiply)
- description and source-code
```javascript
function bnpDMultiply(n) {
this.data[this.t] = this.am(0,n-1,this,0,0,this.t);
++this.t;
this.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.divRemTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>divRemTo (m, q, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.divRemTo)
- description and source-code
```javascript
function bnpDivRemTo(m, q, r) {
  var pm = m.abs();
  if(pm.t <= 0) return;
  var pt = this.abs();
  if(pt.t < pm.t) {
    if(q != null) q.fromInt(0);
    if(r != null) this.copyTo(r);
    return;
  }
  if(r == null) r = nbi();
  var y = nbi(), ts = this.s, ms = m.s;
  var nsh = this.DB-nbits(pm.data[pm.t-1]);	// normalize modulus
  if(nsh > 0) { pm.lShiftTo(nsh,y); pt.lShiftTo(nsh,r); } else { pm.copyTo(y); pt.copyTo(r); }
  var ys = y.t;
  var y0 = y.data[ys-1];
  if(y0 == 0) return;
  var yt = y0*(1<<this.F1)+((ys>1)?y.data[ys-2]>>this.F2:0);
  var d1 = this.FV/yt, d2 = (1<<this.F1)/yt, e = 1<<this.F2;
  var i = r.t, j = i-ys, t = (q==null)?nbi():q;
  y.dlShiftTo(j,t);
  if(r.compareTo(t) >= 0) {
    r.data[r.t++] = 1;
    r.subTo(t,r);
  }
  BigInteger.ONE.dlShiftTo(ys,t);
  t.subTo(y,y);	// "negative" y so we can replace sub with am later
  while(y.t < ys) y.data[y.t++] = 0;
  while(--j >= 0) {
    // Estimate quotient digit
    var qd = (r.data[--i]==y0)?this.DM:Math.floor(r.data[i]*d1+(r.data[i-1]+e)*d2);
    if((r.data[i]+=y.am(0,qd,r,j,0,ys)) < qd) {	// Try it out
      y.dlShiftTo(j,t);
      r.subTo(t,r);
      while(r.data[i] < --qd) r.subTo(t,r);
    }
  }
  if(q != null) {
    r.drShiftTo(ys,q);
    if(ts != ms) BigInteger.ZERO.subTo(q,q);
  }
  r.t = ys;
  r.clamp();
  if(nsh > 0) r.rShiftTo(nsh,r);	// Denormalize remainder
  if(ts < 0) BigInteger.ZERO.subTo(r,r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.divide"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>divide (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.divide)
- description and source-code
```javascript
function bnDivide(a) { var r = nbi(); this.divRemTo(a,r,null); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.divideAndRemainder"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>divideAndRemainder (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.divideAndRemainder)
- description and source-code
```javascript
function bnDivideAndRemainder(a) {
var q = nbi(), r = nbi();
this.divRemTo(a,q,r);
return new Array(q,r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.dlShiftTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>dlShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.dlShiftTo)
- description and source-code
```javascript
function bnpDLShiftTo(n, r) {
  var i;
  for(i = this.t-1; i >= 0; --i) r.data[i+n] = this.data[i];
  for(i = n-1; i >= 0; --i) r.data[i] = 0;
  r.t = this.t+n;
  r.s = this.s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.drShiftTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>drShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.drShiftTo)
- description and source-code
```javascript
function bnpDRShiftTo(n, r) {
  for(var i = n; i < this.t; ++i) r.data[i-n] = this.data[i];
  r.t = Math.max(this.t-n,0);
  r.s = this.s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.equals"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>equals (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.equals)
- description and source-code
```javascript
function bnEquals(a) { return(this.compareTo(a)==0); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.exp"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>exp (e, z)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.exp)
- description and source-code
```javascript
function bnpExp(e, z) {
  if(e > 0xffffffff || e < 1) return BigInteger.ONE;
  var r = nbi(), r2 = nbi(), g = z.convert(this), i = nbits(e)-1;
  g.copyTo(r);
  while(--i >= 0) {
    z.sqrTo(r,r2);
    if((e&(1<<i)) > 0) z.mulTo(r2,g,r);
    else { var t = r; r = r2; r2 = t; }
  }
  return z.revert(r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.flipBit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>flipBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.flipBit)
- description and source-code
```javascript
function bnFlipBit(n) { return this.changeBit(n,op_xor); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.fromInt"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromInt (x)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromInt)
- description and source-code
```javascript
function bnpFromInt(x) {
  this.t = 1;
  this.s = (x<0)?-1:0;
  if(x > 0) this.data[0] = x;
  else if(x < -1) this.data[0] = x+this.DV;
  else this.t = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.fromNumber"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromNumber (a, b, c)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromNumber)
- description and source-code
```javascript
function bnpFromNumber(a, b, c) {
if("number" == typeof b) {
 // new BigInteger(int,int,RNG)
 if(a < 2) this.fromInt(1);
 else {
   this.fromNumber(a,c);
   if(!this.testBit(a-1))  // force MSB set
     this.bitwiseTo(BigInteger.ONE.shiftLeft(a-1),op_or,this);
   if(this.isEven()) this.dAddOffset(1,0); // force odd
   while(!this.isProbablePrime(b)) {
     this.dAddOffset(2,0);
     if(this.bitLength() > a) this.subTo(BigInteger.ONE.shiftLeft(a-1),this);
   }
 }
} else {
 // new BigInteger(int,RNG)
 var x = new Array(), t = a&7;
 x.length = (a>>3)+1;
 b.nextBytes(x);
 if(t > 0) x[0] &= ((1<<t)-1); else x[0] = 0;
 this.fromString(x,256);
}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.fromRadix"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromRadix (s, b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromRadix)
- description and source-code
```javascript
function bnpFromRadix(s, b) {
this.fromInt(0);
if(b == null) b = 10;
var cs = this.chunkSize(b);
var d = Math.pow(b,cs), mi = false, j = 0, w = 0;
for(var i = 0; i < s.length; ++i) {
 var x = intAt(s,i);
 if(x < 0) {
   if(s.charAt(i) == "-" && this.signum() == 0) mi = true;
   continue;
 }
 w = b*w+x;
 if(++j >= cs) {
   this.dMultiply(d);
   this.dAddOffset(w,0);
   j = 0;
   w = 0;
 }
}
if(j > 0) {
 this.dMultiply(Math.pow(b,j));
 this.dAddOffset(w,0);
}
if(mi) BigInteger.ZERO.subTo(this,this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.fromString"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>fromString (s, b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.fromString)
- description and source-code
```javascript
function bnpFromString(s, b) {
  var k;
  if(b == 16) k = 4;
  else if(b == 8) k = 3;
  else if(b == 256) k = 8; // byte array
  else if(b == 2) k = 1;
  else if(b == 32) k = 5;
  else if(b == 4) k = 2;
  else { this.fromRadix(s,b); return; }
  this.t = 0;
  this.s = 0;
  var i = s.length, mi = false, sh = 0;
  while(--i >= 0) {
    var x = (k==8)?s[i]&0xff:intAt(s,i);
    if(x < 0) {
      if(s.charAt(i) == "-") mi = true;
      continue;
    }
    mi = false;
    if(sh == 0)
      this.data[this.t++] = x;
    else if(sh+k > this.DB) {
      this.data[this.t-1] |= (x&((1<<(this.DB-sh))-1))<<sh;
      this.data[this.t++] = (x>>(this.DB-sh));
    } else
      this.data[this.t-1] |= x<<sh;
    sh += k;
    if(sh >= this.DB) sh -= this.DB;
  }
  if(k == 8 && (s[0]&0x80) != 0) {
    this.s = -1;
    if(sh > 0) this.data[this.t-1] |= ((1<<(this.DB-sh))-1)<<sh;
  }
  this.clamp();
  if(mi) BigInteger.ZERO.subTo(this,this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.gcd"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>gcd (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.gcd)
- description and source-code
```javascript
function bnGCD(a) {
var x = (this.s<0)?this.negate():this.clone();
var y = (a.s<0)?a.negate():a.clone();
if(x.compareTo(y) < 0) { var t = x; x = y; y = t; }
var i = x.getLowestSetBit(), g = y.getLowestSetBit();
if(g < 0) return x;
if(i < g) g = i;
if(g > 0) {
 x.rShiftTo(g,x);
 y.rShiftTo(g,y);
}
while(x.signum() > 0) {
 if((i = x.getLowestSetBit()) > 0) x.rShiftTo(i,x);
 if((i = y.getLowestSetBit()) > 0) y.rShiftTo(i,y);
 if(x.compareTo(y) >= 0) {
   x.subTo(y,x);
   x.rShiftTo(1,x);
 } else {
   y.subTo(x,y);
   y.rShiftTo(1,y);
 }
}
if(g > 0) y.lShiftTo(g,y);
return y;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.getLowestSetBit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>getLowestSetBit ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.getLowestSetBit)
- description and source-code
```javascript
function bnGetLowestSetBit() {
for(var i = 0; i < this.t; ++i)
 if(this.data[i] != 0) return i*this.DB+lbit(this.data[i]);
if(this.s < 0) return this.t*this.DB;
return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.intValue"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>intValue ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.intValue)
- description and source-code
```javascript
function bnIntValue() {
if(this.s < 0) {
 if(this.t == 1) return this.data[0]-this.DV;
 else if(this.t == 0) return -1;
} else if(this.t == 1) return this.data[0];
else if(this.t == 0) return 0;
// assumes 16 < DB < 32
return ((this.data[1]&((1<<(32-this.DB))-1))<<this.DB)|this.data[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.invDigit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>invDigit ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.invDigit)
- description and source-code
```javascript
function bnpInvDigit() {
  if(this.t < 1) return 0;
  var x = this.data[0];
  if((x&1) == 0) return 0;
  var y = x&3;		// y == 1/x mod 2^2
  y = (y*(2-(x&0xf)*y))&0xf;	// y == 1/x mod 2^4
  y = (y*(2-(x&0xff)*y))&0xff;	// y == 1/x mod 2^8
  y = (y*(2-(((x&0xffff)*y)&0xffff)))&0xffff;	// y == 1/x mod 2^16
  // last step - calculate inverse mod DV directly;
  // assumes 16 < DB <= 32 and assumes ability to handle 48-bit ints
  y = (y*(2-x*y%this.DV))%this.DV;		// y == 1/x mod 2^dbits
  // we really want the negative inverse, and -DV < y < DV
  return (y>0)?this.DV-y:-y;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.isEven"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>isEven ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.isEven)
- description and source-code
```javascript
function bnpIsEven() { return ((this.t>0)?(this.data[0]&1):this.s) == 0; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.isProbablePrime"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>isProbablePrime (t)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.isProbablePrime)
- description and source-code
```javascript
function bnIsProbablePrime(t) {
var i, x = this.abs();
if(x.t == 1 && x.data[0] <= lowprimes[lowprimes.length-1]) {
 for(i = 0; i < lowprimes.length; ++i)
   if(x.data[0] == lowprimes[i]) return true;
 return false;
}
if(x.isEven()) return false;
i = 1;
while(i < lowprimes.length) {
 var m = lowprimes[i], j = i+1;
 while(j < lowprimes.length && m < lplim) m *= lowprimes[j++];
 m = x.modInt(m);
 while(i < j) if(m%lowprimes[i++] == 0) return false;
}
return x.millerRabin(t);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.lShiftTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>lShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.lShiftTo)
- description and source-code
```javascript
function bnpLShiftTo(n, r) {
  var bs = n%this.DB;
  var cbs = this.DB-bs;
  var bm = (1<<cbs)-1;
  var ds = Math.floor(n/this.DB), c = (this.s<<bs)&this.DM, i;
  for(i = this.t-1; i >= 0; --i) {
    r.data[i+ds+1] = (this.data[i]>>cbs)|c;
    c = (this.data[i]&bm)<<bs;
  }
  for(i = ds-1; i >= 0; --i) r.data[i] = 0;
  r.data[ds] = c;
  r.t = this.t+ds+1;
  r.s = this.s;
  r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.max"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>max (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.max)
- description and source-code
```javascript
function bnMax(a) { return(this.compareTo(a)>0)?this:a; }
```
- example usage
```shell
...
  // drop data if connection not open
  if(!c.open) {
    socket.receive(e.bytesAvailable);
  } else {
    // only receive if there are enough bytes available to
    // process a record
    if(e.bytesAvailable >= _requiredBytes) {
      var count = Math.max(e.bytesAvailable, _requiredBytes);
      var data = socket.receive(count);
      if(data !== null) {
        _requiredBytes = c.process(data);
      }
    }
  }
};
...
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.millerRabin"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>millerRabin (t)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.millerRabin)
- description and source-code
```javascript
function bnpMillerRabin(t) {
var n1 = this.subtract(BigInteger.ONE);
var k = n1.getLowestSetBit();
if(k <= 0) return false;
var r = n1.shiftRight(k);
var prng = bnGetPrng();
var a;
for(var i = 0; i < t; ++i) {
 // select witness 'a' at random from between 1 and n1
 do {
   a = new BigInteger(this.bitLength(), prng);
 }
 while(a.compareTo(BigInteger.ONE) <= 0 || a.compareTo(n1) >= 0);
 var y = a.modPow(r,this);
 if(y.compareTo(BigInteger.ONE) != 0 && y.compareTo(n1) != 0) {
   var j = 1;
   while(j++ < k && y.compareTo(n1) != 0) {
     y = y.modPowInt(2,this);
     if(y.compareTo(BigInteger.ONE) == 0) return false;
   }
   if(y.compareTo(n1) != 0) return false;
 }
}
return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.min"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>min (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.min)
- description and source-code
```javascript
function bnMin(a) { return(this.compareTo(a)<0)?this:a; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.mod"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>mod (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.mod)
- description and source-code
```javascript
function bnMod(a) {
  var r = nbi();
  this.abs().divRemTo(a,null,r);
  if(this.s < 0 && r.compareTo(BigInteger.ZERO) > 0) a.subTo(r,r);
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.modInt"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modInt (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modInt)
- description and source-code
```javascript
function bnpModInt(n) {
if(n <= 0) return 0;
var d = this.DV%n, r = (this.s<0)?n-1:0;
if(this.t > 0)
 if(d == 0) r = this.data[0]%n;
 else for(var i = this.t-1; i >= 0; --i) r = (d*r+this.data[i])%n;
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.modInverse"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modInverse (m)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modInverse)
- description and source-code
```javascript
function bnModInverse(m) {
var ac = m.isEven();
if((this.isEven() && ac) || m.signum() == 0) return BigInteger.ZERO;
var u = m.clone(), v = this.clone();
var a = nbv(1), b = nbv(0), c = nbv(0), d = nbv(1);
while(u.signum() != 0) {
 while(u.isEven()) {
   u.rShiftTo(1,u);
   if(ac) {
     if(!a.isEven() || !b.isEven()) { a.addTo(this,a); b.subTo(m,b); }
     a.rShiftTo(1,a);
   } else if(!b.isEven()) b.subTo(m,b);
   b.rShiftTo(1,b);
 }
 while(v.isEven()) {
   v.rShiftTo(1,v);
   if(ac) {
     if(!c.isEven() || !d.isEven()) { c.addTo(this,c); d.subTo(m,d); }
     c.rShiftTo(1,c);
   } else if(!d.isEven()) d.subTo(m,d);
   d.rShiftTo(1,d);
 }
 if(u.compareTo(v) >= 0) {
   u.subTo(v,u);
   if(ac) a.subTo(c,a);
   b.subTo(d,b);
 } else {
   v.subTo(u,v);
   if(ac) c.subTo(a,c);
   d.subTo(b,d);
 }
}
if(v.compareTo(BigInteger.ONE) != 0) return BigInteger.ZERO;
if(d.compareTo(m) >= 0) return d.subtract(m);
if(d.signum() < 0) d.addTo(m,d); else return d;
if(d.signum() < 0) return d.add(m); else return d;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.modPow"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modPow (e, m)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modPow)
- description and source-code
```javascript
function bnModPow(e, m) {
var i = e.bitLength(), k, r = nbv(1), z;
if(i <= 0) return r;
else if(i < 18) k = 1;
else if(i < 48) k = 3;
else if(i < 144) k = 4;
else if(i < 768) k = 5;
else k = 6;
if(i < 8)
 z = new Classic(m);
else if(m.isEven())
 z = new Barrett(m);
else
 z = new Montgomery(m);

// precomputation
var g = new Array(), n = 3, k1 = k-1, km = (1<<k)-1;
g[1] = z.convert(this);
if(k > 1) {
 var g2 = nbi();
 z.sqrTo(g[1],g2);
 while(n <= km) {
   g[n] = nbi();
   z.mulTo(g2,g[n-2],g[n]);
   n += 2;
 }
}

var j = e.t-1, w, is1 = true, r2 = nbi(), t;
i = nbits(e.data[j])-1;
while(j >= 0) {
 if(i >= k1) w = (e.data[j]>>(i-k1))&km;
 else {
   w = (e.data[j]&((1<<(i+1))-1))<<(k1-i);
   if(j > 0) w |= e.data[j-1]>>(this.DB+i-k1);
 }

 n = k;
 while((w&1) == 0) { w >>= 1; --n; }
 if((i -= n) < 0) { i += this.DB; --j; }
 if(is1) {  // ret == 1, don't bother squaring or multiplying it
   g[w].copyTo(r);
   is1 = false;
 } else {
   while(n > 1) { z.sqrTo(r,r2); z.sqrTo(r2,r); n -= 2; }
   if(n > 0) z.sqrTo(r,r2); else { t = r; r = r2; r2 = t; }
   z.mulTo(r2,g[w],r);
 }

 while(j >= 0 && (e.data[j]&(1<<i)) == 0) {
   z.sqrTo(r,r2); t = r; r = r2; r2 = t;
   if(--i < 0) { i = this.DB-1; --j; }
 }
}
return z.revert(r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.modPowInt"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>modPowInt (e, m)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.modPowInt)
- description and source-code
```javascript
function bnModPowInt(e, m) {
  var z;
  if(e < 256 || m.isEven()) z = new Classic(m); else z = new Montgomery(m);
  return this.exp(e,z);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.multiply"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiply (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiply)
- description and source-code
```javascript
function bnMultiply(a) { var r = nbi(); this.multiplyTo(a,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyLowerTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiplyLowerTo (a, n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyLowerTo)
- description and source-code
```javascript
function bnpMultiplyLowerTo(a, n, r) {
var i = Math.min(this.t+a.t,n);
r.s = 0; // assumes a,this >= 0
r.t = i;
while(i > 0) r.data[--i] = 0;
var j;
for(j = r.t-this.t; i < j; ++i) r.data[i+this.t] = this.am(0,a.data[i],r,i,0,this.t);
for(j = Math.min(a.t,n); i < j; ++i) this.am(0,a.data[i],r,i,0,n-i);
r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiplyTo (a, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyTo)
- description and source-code
```javascript
function bnpMultiplyTo(a, r) {
  var x = this.abs(), y = a.abs();
  var i = x.t;
  r.t = i+y.t;
  while(--i >= 0) r.data[i] = 0;
  for(i = 0; i < y.t; ++i) r.data[i+x.t] = x.am(0,y.data[i],r,i,0,x.t);
  r.s = 0;
  r.clamp();
  if(this.s != a.s) BigInteger.ZERO.subTo(r,r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyUpperTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>multiplyUpperTo (a, n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.multiplyUpperTo)
- description and source-code
```javascript
function bnpMultiplyUpperTo(a, n, r) {
--n;
var i = r.t = this.t+a.t-n;
r.s = 0; // assumes a,this >= 0
while(--i >= 0) r.data[i] = 0;
for(i = Math.max(n-this.t,0); i < a.t; ++i)
 r.data[this.t+i-n] = this.am(n-i,a.data[i],r,0,0,this.t+i-n);
r.clamp();
r.drShiftTo(1,r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.negate"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>negate ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.negate)
- description and source-code
```javascript
function bnNegate() { var r = nbi(); BigInteger.ZERO.subTo(this,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.not"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>not ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.not)
- description and source-code
```javascript
function bnNot() {
var r = nbi();
for(var i = 0; i < this.t; ++i) r.data[i] = this.DM&~this.data[i];
r.t = this.t;
r.s = ~this.s;
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.or"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>or (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.or)
- description and source-code
```javascript
function bnOr(a) { var r = nbi(); this.bitwiseTo(a,op_or,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.pow"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>pow (e)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.pow)
- description and source-code
```javascript
function bnPow(e) { return this.exp(e,new NullExp()); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.rShiftTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>rShiftTo (n, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.rShiftTo)
- description and source-code
```javascript
function bnpRShiftTo(n, r) {
  r.s = this.s;
  var ds = Math.floor(n/this.DB);
  if(ds >= this.t) { r.t = 0; return; }
  var bs = n%this.DB;
  var cbs = this.DB-bs;
  var bm = (1<<bs)-1;
  r.data[0] = this.data[ds]>>bs;
  for(var i = ds+1; i < this.t; ++i) {
    r.data[i-ds-1] |= (this.data[i]&bm)<<cbs;
    r.data[i-ds] = this.data[i]>>bs;
  }
  if(bs > 0) r.data[this.t-ds-1] |= (this.s&bm)<<cbs;
  r.t = this.t-ds;
  r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.remainder"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>remainder (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.remainder)
- description and source-code
```javascript
function bnRemainder(a) { var r = nbi(); this.divRemTo(a,null,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.setBit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>setBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.setBit)
- description and source-code
```javascript
function bnSetBit(n) { return this.changeBit(n,op_or); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.shiftLeft"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>shiftLeft (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.shiftLeft)
- description and source-code
```javascript
function bnShiftLeft(n) {
var r = nbi();
if(n < 0) this.rShiftTo(-n,r); else this.lShiftTo(n,r);
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.shiftRight"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>shiftRight (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.shiftRight)
- description and source-code
```javascript
function bnShiftRight(n) {
var r = nbi();
if(n < 0) this.lShiftTo(-n,r); else this.rShiftTo(n,r);
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.shortValue"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>shortValue ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.shortValue)
- description and source-code
```javascript
function bnShortValue() { return (this.t==0)?this.s:(this.data[0]<<16)>>16; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.signum"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>signum ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.signum)
- description and source-code
```javascript
function bnSigNum() {
if(this.s < 0) return -1;
else if(this.t <= 0 || (this.t == 1 && this.data[0] <= 0)) return 0;
else return 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.squareTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>squareTo (r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.squareTo)
- description and source-code
```javascript
function bnpSquareTo(r) {
  var x = this.abs();
  var i = r.t = 2*x.t;
  while(--i >= 0) r.data[i] = 0;
  for(i = 0; i < x.t-1; ++i) {
    var c = x.am(i,x.data[i],r,2*i,0,1);
    if((r.data[i+x.t]+=x.am(i+1,2*x.data[i],r,2*i+1,c,x.t-i-1)) >= x.DV) {
      r.data[i+x.t] -= x.DV;
      r.data[i+x.t+1] = 1;
    }
  }
  if(r.t > 0) r.data[r.t-1] += x.am(i,x.data[i],r,2*i,0,1);
  r.s = 0;
  r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.subTo"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>subTo (a, r)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.subTo)
- description and source-code
```javascript
function bnpSubTo(a, r) {
  var i = 0, c = 0, m = Math.min(a.t,this.t);
  while(i < m) {
    c += this.data[i]-a.data[i];
    r.data[i++] = c&this.DM;
    c >>= this.DB;
  }
  if(a.t < this.t) {
    c -= a.s;
    while(i < this.t) {
      c += this.data[i];
      r.data[i++] = c&this.DM;
      c >>= this.DB;
    }
    c += this.s;
  } else {
    c += this.s;
    while(i < a.t) {
      c -= a.data[i];
      r.data[i++] = c&this.DM;
      c >>= this.DB;
    }
    c -= a.s;
  }
  r.s = (c<0)?-1:0;
  if(c < -1) r.data[i++] = this.DV+c;
  else if(c > 0) r.data[i++] = c;
  r.t = i;
  r.clamp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.subtract"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>subtract (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.subtract)
- description and source-code
```javascript
function bnSubtract(a) { var r = nbi(); this.subTo(a,r); return r; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.testBit"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>testBit (n)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.testBit)
- description and source-code
```javascript
function bnTestBit(n) {
var j = Math.floor(n/this.DB);
if(j >= this.t) return(this.s!=0);
return((this.data[j]&(1<<(n%this.DB)))!=0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.toByteArray"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>toByteArray ()](#apidoc.element.node-forge.jsbn.BigInteger.prototype.toByteArray)
- description and source-code
```javascript
function bnToByteArray() {
var i = this.t, r = new Array();
r[0] = this.s;
var p = this.DB-(i*this.DB)%8, d, k = 0;
if(i-- > 0) {
 if(p < this.DB && (d = this.data[i]>>p) != (this.s&this.DM)>>p)
   r[k++] = d|(this.s<<(this.DB-p));
 while(i >= 0) {
   if(p < 8) {
     d = (this.data[i]&((1<<p)-1))<<(8-p);
     d |= this.data[--i]>>(p+=this.DB-8);
   } else {
     d = (this.data[i]>>(p-=8))&0xff;
     if(p <= 0) { p += this.DB; --i; }
   }
   if((d&0x80) != 0) d |= -256;
   if(k == 0 && (this.s&0x80) != (d&0x80)) ++k;
   if(k > 0 || d != this.s) r[k++] = d;
 }
}
return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.toRadix"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>toRadix (b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.toRadix)
- description and source-code
```javascript
function bnpToRadix(b) {
if(b == null) b = 10;
if(this.signum() == 0 || b < 2 || b > 36) return "0";
var cs = this.chunkSize(b);
var a = Math.pow(b,cs);
var d = nbv(a), y = nbi(), z = nbi(), r = "";
this.divRemTo(d,y,z);
while(y.signum() > 0) {
 r = (a+z.intValue()).toString(b).substr(1) + r;
 y.divRemTo(d,y,z);
}
return z.intValue().toString(b) + r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.toString"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>toString (b)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.toString)
- description and source-code
```javascript
function bnToString(b) {
  if(this.s < 0) return "-"+this.negate().toString(b);
  var k;
  if(b == 16) k = 4;
  else if(b == 8) k = 3;
  else if(b == 2) k = 1;
  else if(b == 32) k = 5;
  else if(b == 4) k = 2;
  else return this.toRadix(b);
  var km = (1<<k)-1, d, m = false, r = "", i = this.t;
  var p = this.DB-(i*this.DB)%k;
  if(i-- > 0) {
    if(p < this.DB && (d = this.data[i]>>p) > 0) { m = true; r = int2char(d); }
    while(i >= 0) {
      if(p < k) {
        d = (this.data[i]&((1<<p)-1))<<(k-p);
        d |= this.data[--i]>>(p+=this.DB-k);
      } else {
        d = (this.data[i]>>(p-=k))&km;
        if(p <= 0) { p += this.DB; --i; }
      }
      if(d > 0) m = true;
      if(m) r += int2char(d);
    }
  }
  return m?r:"0";
}
```
- example usage
```shell
...
});

socket.on('connect', function() {
  console.log('[socket] connected');
  client.handshake();
});
socket.on('data', function(data) {
  client.process(data.toString('binary')); // encoding should be 'binary'
});
socket.on('end', function() {
  console.log('[socket] disconnected');
});

// connect to google.com
socket.connect(443, 'google.com');
...
```

#### <a name="apidoc.element.node-forge.jsbn.BigInteger.prototype.xor"></a>[function <span class="apidocSignatureSpan">node-forge.jsbn.BigInteger.prototype.</span>xor (a)](#apidoc.element.node-forge.jsbn.BigInteger.prototype.xor)
- description and source-code
```javascript
function bnXor(a) { var r = nbi(); this.bitwiseTo(a,op_xor,r); return r; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.kem"></a>[module node-forge.kem](#apidoc.module.node-forge.kem)

#### <a name="apidoc.element.node-forge.kem.kdf1"></a>[function <span class="apidocSignatureSpan">node-forge.kem.</span>kdf1 (md, digestLength)](#apidoc.element.node-forge.kem.kdf1)
- description and source-code
```javascript
kdf1 = function (md, digestLength) {
  _createKDF(this, md, 0, digestLength || md.digestLength);
}
```
- example usage
```shell
...
// generate an RSA key pair asynchronously (uses web workers if available)
// use workers: -1 to run a fast core estimator to optimize # of workers
forge.rsa.generateKeyPair({bits: 2048, workers: -1}, function(err, keypair) {
  // keypair.privateKey, keypair.publicKey
});

// generate and encapsulate a 16-byte secret key
var kdf1 = new forge.kem.kdf1(forge.md.sha1.create());
var kem = forge.kem.rsa.create(kdf1);
var result = kem.encrypt(keypair.publicKey, 16);
// result has 'encapsulation' and 'key'

// encrypt some bytes
var iv = forge.random.getBytesSync(12);
var someBytes = 'hello world!';
...
```

#### <a name="apidoc.element.node-forge.kem.kdf2"></a>[function <span class="apidocSignatureSpan">node-forge.kem.</span>kdf2 (md, digestLength)](#apidoc.element.node-forge.kem.kdf2)
- description and source-code
```javascript
kdf2 = function (md, digestLength) {
  _createKDF(this, md, 1, digestLength || md.digestLength);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.kem.rsa"></a>[module node-forge.kem.rsa](#apidoc.module.node-forge.kem.rsa)

#### <a name="apidoc.element.node-forge.kem.rsa.create"></a>[function <span class="apidocSignatureSpan">node-forge.kem.rsa.</span>create (kdf, options)](#apidoc.element.node-forge.kem.rsa.create)
- description and source-code
```javascript
create = function (kdf, options) {
  options = options || {};
  var prng = options.prng || forge.random;

  var kem = {};

<span class="apidocCodeCommentSpan">  /**
   * Generates a secret key and its encapsulation.
   *
   * @param publicKey the RSA public key to encrypt with.
   * @param keyLength the length, in bytes, of the secret key to generate.
   *
   * @return an object with:
   *   encapsulation: the ciphertext for generating the secret key, as a
   *     binary-encoded string of bytes.
   *   key: the secret key to use for encrypting a message.
   */
</span>  kem.encrypt = function(publicKey, keyLength) {
    // generate a random r where 1 > r > n
    var byteLength = Math.ceil(publicKey.n.bitLength() / 8);
    var r;
    do {
      r = new BigInteger(
        forge.util.bytesToHex(prng.getBytesSync(byteLength)),
        16).mod(publicKey.n);
    } while(r.equals(BigInteger.ZERO));

    // prepend r with zeros
    r = forge.util.hexToBytes(r.toString(16));
    var zeros = byteLength - r.length;
    if(zeros > 0) {
      r = forge.util.fillString(String.fromCharCode(0), zeros) + r;
    }

    // encrypt the random
    var encapsulation = publicKey.encrypt(r, 'NONE');

    // generate the secret key
    var key = kdf.generate(r, keyLength);

    return {encapsulation: encapsulation, key: key};
  };

  /**
   * Decrypts an encapsulated secret key.
   *
   * @param privateKey the RSA private key to decrypt with.
   * @param encapsulation the ciphertext for generating the secret key, as
   *          a binary-encoded string of bytes.
   * @param keyLength the length, in bytes, of the secret key to generate.
   *
   * @return the secret key as a binary-encoded string of bytes.
   */
  kem.decrypt = function(privateKey, encapsulation, keyLength) {
    // decrypt the encapsulation and generate the secret key
    var r = privateKey.decrypt(encapsulation, 'NONE');
    return kdf.generate(r, keyLength);
  };

  return kem;
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.log"></a>[module node-forge.log](#apidoc.module.node-forge.log)

#### <a name="apidoc.element.node-forge.log.addLogger"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>addLogger (logger)](#apidoc.element.node-forge.log.addLogger)
- description and source-code
```javascript
addLogger = function (logger) {
  sLoggers.push(logger);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.debug"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>debug (category, message)](#apidoc.element.node-forge.log.debug)
- description and source-code
```javascript
debug = function (category, message) {
  // convert arguments to real array, remove category and message
  var args = Array.prototype.slice.call(arguments).slice(2);
  // create message object
  // Note: interpolation and standard formatting is done lazily
  var msg = {
    timestamp: new Date(),
    level: level,
    category: category,
    message: message,
    'arguments': args
<span class="apidocCodeCommentSpan">    /*standard*/
</span>    /*full*/
    /*fullMessage*/
  };
  // process this message
  forge.log.logMessage(msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.error"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>error (category, message)](#apidoc.element.node-forge.log.error)
- description and source-code
```javascript
error = function (category, message) {
  // convert arguments to real array, remove category and message
  var args = Array.prototype.slice.call(arguments).slice(2);
  // create message object
  // Note: interpolation and standard formatting is done lazily
  var msg = {
    timestamp: new Date(),
    level: level,
    category: category,
    message: message,
    'arguments': args
<span class="apidocCodeCommentSpan">    /*standard*/
</span>    /*full*/
    /*fullMessage*/
  };
  // process this message
  forge.log.logMessage(msg);
}
```
- example usage
```shell
...
},
closed: function(c) {
  // close socket
  socket.close();
},
error: function(c, e) {
  // send error, close socket
  tlsSocket.error({
    id: socket.id,
    type: 'tlsError',
    message: e.message,
    bytesAvailable: 0,
    error: e
  });
  socket.close();
...
```

#### <a name="apidoc.element.node-forge.log.info"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>info (category, message)](#apidoc.element.node-forge.log.info)
- description and source-code
```javascript
info = function (category, message) {
  // convert arguments to real array, remove category and message
  var args = Array.prototype.slice.call(arguments).slice(2);
  // create message object
  // Note: interpolation and standard formatting is done lazily
  var msg = {
    timestamp: new Date(),
    level: level,
    category: category,
    message: message,
    'arguments': args
<span class="apidocCodeCommentSpan">    /*standard*/
</span>    /*full*/
    /*fullMessage*/
  };
  // process this message
  forge.log.logMessage(msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.lock"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>lock (logger, lock)](#apidoc.element.node-forge.log.lock)
- description and source-code
```javascript
lock = function (logger, lock) {
  if(typeof lock === 'undefined' || lock) {
    logger.flags |= forge.log.LEVEL_LOCKED;
  } else {
    logger.flags &= ~forge.log.LEVEL_LOCKED;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.logMessage"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>logMessage (message)](#apidoc.element.node-forge.log.logMessage)
- description and source-code
```javascript
logMessage = function (message) {
  var messageLevelIndex = sLevelInfo[message.level].index;
  for(var i = 0; i < sLoggers.length; ++i) {
    var logger = sLoggers[i];
    if(logger.flags & forge.log.NO_LEVEL_CHECK) {
      logger.f(message);
    } else {
      // get logger level
      var loggerLevelIndex = sLevelInfo[logger.level].index;
      // check level
      if(messageLevelIndex <= loggerLevelIndex) {
        // message critical enough, call logger
        logger.f(logger, message);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.makeLogger"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>makeLogger (logFunction)](#apidoc.element.node-forge.log.makeLogger)
- description and source-code
```javascript
makeLogger = function (logFunction) {
  var logger = {
    flags: 0,
    f: logFunction
  };
  forge.log.setLevel(logger, 'none');
  return logger;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.prepareFull"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>prepareFull (message)](#apidoc.element.node-forge.log.prepareFull)
- description and source-code
```javascript
prepareFull = function (message) {
  if(!('full' in message)) {
    // copy args and insert message at the front
    var args = [message.message];
    args = args.concat([] || message['arguments']);
    // format the message
    message.full = forge.util.format.apply(this, args);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.prepareStandard"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>prepareStandard (message)](#apidoc.element.node-forge.log.prepareStandard)
- description and source-code
```javascript
prepareStandard = function (message) {
  if(!('standard' in message)) {
    message.standard =
      sLevelInfo[message.level].name +
      //' ' + +message.timestamp +
      ' [' + message.category + '] ' +
      message.message;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.prepareStandardFull"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>prepareStandardFull (message)](#apidoc.element.node-forge.log.prepareStandardFull)
- description and source-code
```javascript
prepareStandardFull = function (message) {
  if(!('standardFull' in message)) {
    // FIXME implement 'standardFull' logging
    forge.log.prepareStandard(message);
    message.standardFull = message.standard;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.setLevel"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>setLevel (logger, level)](#apidoc.element.node-forge.log.setLevel)
- description and source-code
```javascript
setLevel = function (logger, level) {
  var rval = false;
  if(logger && !(logger.flags & forge.log.LEVEL_LOCKED)) {
    for(var i = 0; i < forge.log.levels.length; ++i) {
      var aValidLevel = forge.log.levels[i];
      if(level == aValidLevel) {
        // set level
        logger.level = level;
        rval = true;
        break;
      }
    }
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.verbose"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>verbose (category, message)](#apidoc.element.node-forge.log.verbose)
- description and source-code
```javascript
verbose = function (category, message) {
  // convert arguments to real array, remove category and message
  var args = Array.prototype.slice.call(arguments).slice(2);
  // create message object
  // Note: interpolation and standard formatting is done lazily
  var msg = {
    timestamp: new Date(),
    level: level,
    category: category,
    message: message,
    'arguments': args
<span class="apidocCodeCommentSpan">    /*standard*/
</span>    /*full*/
    /*fullMessage*/
  };
  // process this message
  forge.log.logMessage(msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.log.warning"></a>[function <span class="apidocSignatureSpan">node-forge.log.</span>warning (category, message)](#apidoc.element.node-forge.log.warning)
- description and source-code
```javascript
warning = function (category, message) {
  // convert arguments to real array, remove category and message
  var args = Array.prototype.slice.call(arguments).slice(2);
  // create message object
  // Note: interpolation and standard formatting is done lazily
  var msg = {
    timestamp: new Date(),
    level: level,
    category: category,
    message: message,
    'arguments': args
<span class="apidocCodeCommentSpan">    /*standard*/
</span>    /*full*/
    /*fullMessage*/
  };
  // process this message
  forge.log.logMessage(msg);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.log.consoleLogger"></a>[module node-forge.log.consoleLogger](#apidoc.module.node-forge.log.consoleLogger)

#### <a name="apidoc.element.node-forge.log.consoleLogger.f"></a>[function <span class="apidocSignatureSpan">node-forge.log.consoleLogger.</span>f (logger, message)](#apidoc.element.node-forge.log.consoleLogger.f)
- description and source-code
```javascript
f = function (logger, message) {
  forge.log.prepareStandardFull(message);
  console.log(message.standardFull);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.md5"></a>[module node-forge.md5](#apidoc.module.node-forge.md5)

#### <a name="apidoc.element.node-forge.md5.create"></a>[function <span class="apidocSignatureSpan">node-forge.md5.</span>create ()](#apidoc.element.node-forge.md5.create)
- description and source-code
```javascript
create = function () {
  // do initialization as necessary
  if(!_initialized) {
    _init();
  }

  // MD5 state contains four 32-bit integers
  var _state = null;

  // input buffer
  var _input = forge.util.createBuffer();

  // used for word storage
  var _w = new Array(16);

  // message digest object
  var md = {
    algorithm: 'md5',
    blockLength: 64,
    digestLength: 16,
    // 56-bit length of message so far (does not including padding)
    messageLength: 0,
    // true message length
    fullMessageLength: null,
    // size of message length in bytes
    messageLengthSize: 8
  };

<span class="apidocCodeCommentSpan">  /**
   * Starts the digest.
   *
   * @return this digest object.
   */
</span>  md.start = function() {
    // up to 56-bit message length for convenience
    md.messageLength = 0;

    // full message length (set md.messageLength64 for backwards-compatibility)
    md.fullMessageLength = md.messageLength64 = [];
    var int32s = md.messageLengthSize / 4;
    for(var i = 0; i < int32s; ++i) {
      md.fullMessageLength.push(0);
    }
    _input = forge.util.createBuffer();
    _state = {
      h0: 0x67452301,
      h1: 0xEFCDAB89,
      h2: 0x98BADCFE,
      h3: 0x10325476
    };
    return md;
  };
  // start digest automatically for first time
  md.start();

  /**
   * Updates the digest with the given message input. The given input can
   * treated as raw input (no encoding will be applied) or an encoding of
   * 'utf8' maybe given to encode the input using UTF-8.
   *
   * @param msg the message input to update with.
   * @param encoding the encoding to use (default: 'raw', other: 'utf8').
   *
   * @return this digest object.
   */
  md.update = function(msg, encoding) {
    if(encoding === 'utf8') {
      msg = forge.util.encodeUtf8(msg);
    }

    // update message length
    var len = msg.length;
    md.messageLength += len;
    len = [(len / 0x100000000) >>> 0, len >>> 0];
    for(var i = md.fullMessageLength.length - 1; i >= 0; --i) {
      md.fullMessageLength[i] += len[1];
      len[1] = len[0] + ((md.fullMessageLength[i] / 0x100000000) >>> 0);
      md.fullMessageLength[i] = md.fullMessageLength[i] >>> 0;
      len[0] = (len[1] / 0x100000000) >>> 0;
    }

    // add bytes to input buffer
    _input.putBytes(msg);

    // process bytes
    _update(_state, _w, _input);

    // compact input buffer every 2K or if empty
    if(_input.read > 2048 || _input.length() === 0) {
      _input.compact();
    }

    return md;
  };

  /**
   * Produces the digest.
   *
   * @return a byte buffer containing the digest value.
   */
  md.digest = function() {
    /* Note: Here we copy the remaining bytes in the input buffer and
    add the appropriate MD5 padding. Then we do the final update
    on a copy of the state so that if the user wants to get
    intermediate digests they can do so. */

    /* Determine the number of bytes that must be added to the message
    to ensure its length is congruent to 448 mod 512. In other words,
    the data to be digested must be a multiple of 512 bits (or 128 bytes).
    This data includes the message, some padding, and the length of the
    message. Since the length of the message will be encoded as 8 bytes (64
    bits), that means that the last segment of the data must have 56 bytes
    (448 bits) of message and padding. Therefore, the length of the message
    plus the padding must be congruent to 448 mod 512 because
    512 - 128 = 448.

    In order to fill up the message length it must be filled with
    padding that begins with 1 bit followed by all 0 bits. Padding
    must *always* be present, so if the message length is already
    congruent to 448 mod 512, then 512 padding bits must be added. */

    var finalBlock = forge.util.createBuffer();
    finalBlock.putBytes(_input.bytes());

    // compute remaining size to be digested (include message length size)
    var remaining = (
      md.fullMessageLength[md.fullMessageLength.length - 1] +
      md.messageLengthSize);

    // add padding for overflow blockSize - overflow
    // _padding starts with 1 byte with first bit is set (byte value 128), ...
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.mgf1"></a>[module node-forge.mgf1](#apidoc.module.node-forge.mgf1)

#### <a name="apidoc.element.node-forge.mgf1.create"></a>[function <span class="apidocSignatureSpan">node-forge.mgf1.</span>create (md)](#apidoc.element.node-forge.mgf1.create)
- description and source-code
```javascript
create = function (md) {
  var mgf = {
<span class="apidocCodeCommentSpan">    /**
     * Generate mask of specified length.
     *
     * @param {String} seed The seed for mask generation.
     * @param maskLen Number of bytes to generate.
     * @return {String} The generated mask.
     */
</span>    generate: function(seed, maskLen) {
      /* 2. Let T be the empty octet string. */
      var t = new forge.util.ByteBuffer();

      /* 3. For counter from 0 to ceil(maskLen / hLen), do the following: */
      var len = Math.ceil(maskLen / md.digestLength);
      for(var i = 0; i < len; i++) {
        /* a. Convert counter to an octet string C of length 4 octets */
        var c = new forge.util.ByteBuffer();
        c.putInt32(i);

        /* b. Concatenate the hash of the seed mgfSeed and C to the octet
         * string T: */
        md.start();
        md.update(seed + c.getBytes());
        t.putBuffer(md.digest());
      }

      /* Output the leading maskLen octets of T as the octet string mask. */
      t.truncate(t.length() - maskLen);
      return t.getBytes();
    }
  };

  return mgf;
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.net"></a>[module node-forge.net](#apidoc.module.node-forge.net)

#### <a name="apidoc.element.node-forge.net.createSocket"></a>[function <span class="apidocSignatureSpan">node-forge.net.</span>createSocket (options)](#apidoc.element.node-forge.net.createSocket)
- description and source-code
```javascript
createSocket = function (options) {
  var socket = null;
  if(options.flashId in net.socketPools) {
    // get related socket pool
    var sp = net.socketPools[options.flashId];
    socket = sp.createSocket(options);
  }
  return socket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.net.createSocketPool"></a>[function <span class="apidocSignatureSpan">node-forge.net.</span>createSocketPool (options)](#apidoc.element.node-forge.net.createSocketPool)
- description and source-code
```javascript
createSocketPool = function (options) {
  // set default
  options.msie = options.msie || false;

  // initialize the flash interface
  var spId = options.flashId;
  var api = document.getElementById(spId);
  api.init({marshallExceptions: !options.msie});

  // create socket pool entry
  var sp = {
    // ID of the socket pool
    id: spId,
    // flash interface
    flashApi: api,
    // map of socket ID to sockets
    sockets: {},
    // default policy port
    policyPort: options.policyPort || 0,
    // default policy URL
    policyUrl: options.policyUrl || null
  };
  net.socketPools[spId] = sp;

  // create event handler, subscribe to flash events
  if(options.msie === true) {
    sp.handler = function(e) {
      if(e.id in sp.sockets) {
        // get handler function
        var f;
        switch(e.type) {
        case 'connect':
          f = 'connected';
          break;
        case 'close':
          f = 'closed';
          break;
        case 'socketData':
          f = 'data';
          break;
        default:
          f = 'error';
          break;
        }
<span class="apidocCodeCommentSpan">        /* IE calls javascript on the thread of the external object
          that triggered the event (in this case flash) ... which will
          either run concurrently with other javascript or pre-empt any
          running javascript in the middle of its execution (BAD!) ...
          calling setTimeout() will schedule the javascript to run on
          the javascript thread and solve this EVIL problem. */
</span>        setTimeout(function() {sp.sockets[e.id][f](e);}, 0);
      }
    };
  } else {
    sp.handler = function(e) {
      if(e.id in sp.sockets) {
        // get handler function
        var f;
        switch(e.type) {
        case 'connect':
          f = 'connected';
          break;
        case 'close':
          f = 'closed';
          break;
        case 'socketData':
          f = 'data';
          break;
        default:
          f = 'error';
          break;
        }
        sp.sockets[e.id][f](e);
      }
    };
  }
  var handler = 'forge.net.socketPools[\'' + spId + '\'].handler';
  api.subscribe('connect', handler);
  api.subscribe('close', handler);
  api.subscribe('socketData', handler);
  api.subscribe('ioError', handler);
  api.subscribe('securityError', handler);

  /**
   * Destroys a socket pool. The socket pool still needs to be cleaned
   * up via net.cleanup().
   */
  sp.destroy = function() {
    delete net.socketPools[options.flashId];
    for(var id in sp.sockets) {
      sp.sockets[id].destroy();
    }
    sp.sockets = {};
    api.cleanup();
  };

  /**
   * Creates a new socket.
   *
   * @param options:
   *          connected: function(event) called when the socket connects.
   *          closed: function(event) called when the socket closes.
   *          data: function(event) called when socket data has arrived,
   *            it can be read from the socket using receive().
   *          error: function(event) called when a socket error occurs.
   */
   sp.createSocket = function(options) {
     // default to empty options
     options = options || {};

     // create flash socket
     var id = api.create();

     // create javascript socket wrapper
     var socket = {
       id: id,
       // set handlers
       connected: options.connected || function(e) {},
       closed: options.closed || function(e) {},
       data: options.data || function(e) {},
       error: options.error || function(e) {}
     };

     /**
      * Destroys this socket.
      */
     socket.destroy = function() {
       api.destroy(id);
       delete sp.sockets[id];
     };

     /**
      * Connects this socket.
      *
      * @param options:
      *          host: the host to connect to.
      *          port: the port to connect to.
      *          policyPort: the policy port to use (if non-default), 0 to
      *            use the flash default.
      *          policyUrl: the policy file URL to use (instead of port).
      */
     socket.connect = function(options) {
       // give precedence to policy URL over policy port
       // if no policy ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.net.destroySocketPool"></a>[function <span class="apidocSignatureSpan">node-forge.net.</span>destroySocketPool (options)](#apidoc.element.node-forge.net.destroySocketPool)
- description and source-code
```javascript
destroySocketPool = function (options) {
  if(options.flashId in net.socketPools) {
    var sp = net.socketPools[options.flashId];
    sp.destroy();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.pbe"></a>[module node-forge.pbe](#apidoc.module.node-forge.pbe)

#### <a name="apidoc.element.node-forge.pbe.generatePkcs12Key"></a>[function <span class="apidocSignatureSpan">node-forge.pbe.</span>generatePkcs12Key (password, salt, id, iter, n, md)](#apidoc.element.node-forge.pbe.generatePkcs12Key)
- description and source-code
```javascript
generatePkcs12Key = function (password, salt, id, iter, n, md) {
  var j, l;

  if(typeof md === 'undefined' || md === null) {
    if(!('sha1' in forge.md)) {
      throw new Error('"sha1" hash algorithm unavailable.');
    }
    md = forge.md.sha1.create();
  }

  var u = md.digestLength;
  var v = md.blockLength;
  var result = new forge.util.ByteBuffer();

<span class="apidocCodeCommentSpan">  /* Convert password to Unicode byte buffer + trailing 0-byte. */
</span>  var passBuf = new forge.util.ByteBuffer();
  if(password !== null && password !== undefined) {
    for(l = 0; l < password.length; l++) {
      passBuf.putInt16(password.charCodeAt(l));
    }
    passBuf.putInt16(0);
  }

  /* Length of salt and password in BYTES. */
  var p = passBuf.length();
  var s = salt.length();

  /* 1. Construct a string, D (the "diversifier"), by concatenating
        v copies of ID. */
  var D = new forge.util.ByteBuffer();
  D.fillWithByte(id, v);

  /* 2. Concatenate copies of the salt together to create a string S of length
        v * ceil(s / v) bytes (the final copy of the salt may be trunacted
        to create S).
        Note that if the salt is the empty string, then so is S. */
  var Slen = v * Math.ceil(s / v);
  var S = new forge.util.ByteBuffer();
  for(l = 0; l < Slen; l++) {
    S.putByte(salt.at(l % s));
  }

  /* 3. Concatenate copies of the password together to create a string P of
        length v * ceil(p / v) bytes (the final copy of the password may be
        truncated to create P).
        Note that if the password is the empty string, then so is P. */
  var Plen = v * Math.ceil(p / v);
  var P = new forge.util.ByteBuffer();
  for(l = 0; l < Plen; l++) {
    P.putByte(passBuf.at(l % p));
  }

  /* 4. Set I=S||P to be the concatenation of S and P. */
  var I = S;
  I.putBuffer(P);

  /* 5. Set c=ceil(n / u). */
  var c = Math.ceil(n / u);

  /* 6. For i=1, 2, ..., c, do the following: */
  for(var i = 1; i <= c; i++) {
    /* a) Set Ai=H^r(D||I). (l.e. the rth hash of D||I, H(H(H(...H(D||I)))) */
    var buf = new forge.util.ByteBuffer();
    buf.putBytes(D.bytes());
    buf.putBytes(I.bytes());
    for(var round = 0; round < iter; round++) {
      md.start();
      md.update(buf.getBytes());
      buf = md.digest();
    }

    /* b) Concatenate copies of Ai to create a string B of length v bytes (the
          final copy of Ai may be truncated to create B). */
    var B = new forge.util.ByteBuffer();
    for(l = 0; l < v; l++) {
      B.putByte(buf.at(l % u));
    }

    /* c) Treating I as a concatenation I0, I1, ..., Ik-1 of v-byte blocks,
          where k=ceil(s / v) + ceil(p / v), modify I by setting
          Ij=(Ij+B+1) mod 2v for each j.  */
    var k = Math.ceil(s / v) + Math.ceil(p / v);
    var Inew = new forge.util.ByteBuffer();
    for(j = 0; j < k; j++) {
      var chunk = new forge.util.ByteBuffer(I.getBytes(v));
      var x = 0x1ff;
      for(l = B.length() - 1; l >= 0; l--) {
        x = x >> 8;
        x += B.at(l) + chunk.at(l);
        chunk.setAt(l, x & 0xff);
      }
      Inew.putBuffer(chunk);
    }
    I = Inew;

    /* Add Ai to A. */
    result.putBuffer(buf);
  }

  result.truncate(result.length() - n);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pbe.getCipher"></a>[function <span class="apidocSignatureSpan">node-forge.pbe.</span>getCipher (oid, params, password)](#apidoc.element.node-forge.pbe.getCipher)
- description and source-code
```javascript
getCipher = function (oid, params, password) {
  switch(oid) {
  case pki.oids['pkcs5PBES2']:
    return pki.pbe.getCipherForPBES2(oid, params, password);

  case pki.oids['pbeWithSHAAnd3-KeyTripleDES-CBC']:
  case pki.oids['pbewithSHAAnd40BitRC2-CBC']:
    return pki.pbe.getCipherForPKCS12PBE(oid, params, password);

  default:
    var error = new Error('Cannot read encrypted PBE data block. Unsupported OID.');
    error.oid = oid;
    error.supportedOids = [
      'pkcs5PBES2',
      'pbeWithSHAAnd3-KeyTripleDES-CBC',
      'pbewithSHAAnd40BitRC2-CBC'
    ];
    throw error;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pbe.getCipherForPBES2"></a>[function <span class="apidocSignatureSpan">node-forge.pbe.</span>getCipherForPBES2 (oid, params, password)](#apidoc.element.node-forge.pbe.getCipherForPBES2)
- description and source-code
```javascript
getCipherForPBES2 = function (oid, params, password) {
  // get PBE params
  var capture = {};
  var errors = [];
  if(!asn1.validate(params, PBES2AlgorithmsValidator, capture, errors)) {
    var error = new Error('Cannot read password-based-encryption algorithm ' +
      'parameters. ASN.1 object is not a supported EncryptedPrivateKeyInfo.');
    error.errors = errors;
    throw error;
  }

  // check oids
  oid = asn1.derToOid(capture.kdfOid);
  if(oid !== pki.oids['pkcs5PBKDF2']) {
    var error = new Error('Cannot read encrypted private key. ' +
      'Unsupported key derivation function OID.');
    error.oid = oid;
    error.supportedOids = ['pkcs5PBKDF2'];
    throw error;
  }
  oid = asn1.derToOid(capture.encOid);
  if(oid !== pki.oids['aes128-CBC'] &&
    oid !== pki.oids['aes192-CBC'] &&
    oid !== pki.oids['aes256-CBC'] &&
    oid !== pki.oids['des-EDE3-CBC'] &&
    oid !== pki.oids['desCBC']) {
    var error = new Error('Cannot read encrypted private key. ' +
      'Unsupported encryption scheme OID.');
    error.oid = oid;
    error.supportedOids = [
      'aes128-CBC', 'aes192-CBC', 'aes256-CBC', 'des-EDE3-CBC', 'desCBC'];
    throw error;
  }

  // set PBE params
  var salt = capture.kdfSalt;
  var count = forge.util.createBuffer(capture.kdfIterationCount);
  count = count.getInt(count.length() << 3);
  var dkLen;
  var cipherFn;
  switch(pki.oids[oid]) {
  case 'aes128-CBC':
    dkLen = 16;
    cipherFn = forge.aes.createDecryptionCipher;
    break;
  case 'aes192-CBC':
    dkLen = 24;
    cipherFn = forge.aes.createDecryptionCipher;
    break;
  case 'aes256-CBC':
    dkLen = 32;
    cipherFn = forge.aes.createDecryptionCipher;
    break;
  case 'des-EDE3-CBC':
    dkLen = 24;
    cipherFn = forge.des.createDecryptionCipher;
    break;
  case 'desCBC':
    dkLen = 8;
    cipherFn = forge.des.createDecryptionCipher;
    break;
  }

  // get PRF message digest
  var md = prfOidToMessageDigest(capture.prfOid);

  // decrypt private key using pbe with chosen PRF and AES/DES
  var dk = forge.pkcs5.pbkdf2(password, salt, count, dkLen, md);
  var iv = capture.encIv;
  var cipher = cipherFn(dk);
  cipher.start(iv);

  return cipher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pbe.getCipherForPKCS12PBE"></a>[function <span class="apidocSignatureSpan">node-forge.pbe.</span>getCipherForPKCS12PBE (oid, params, password)](#apidoc.element.node-forge.pbe.getCipherForPKCS12PBE)
- description and source-code
```javascript
getCipherForPKCS12PBE = function (oid, params, password) {
  // get PBE params
  var capture = {};
  var errors = [];
  if(!asn1.validate(params, pkcs12PbeParamsValidator, capture, errors)) {
    var error = new Error('Cannot read password-based-encryption algorithm ' +
      'parameters. ASN.1 object is not a supported EncryptedPrivateKeyInfo.');
    error.errors = errors;
    throw error;
  }

  var salt = forge.util.createBuffer(capture.salt);
  var count = forge.util.createBuffer(capture.iterations);
  count = count.getInt(count.length() << 3);

  var dkLen, dIvLen, cipherFn;
  switch(oid) {
    case pki.oids['pbeWithSHAAnd3-KeyTripleDES-CBC']:
      dkLen = 24;
      dIvLen = 8;
      cipherFn = forge.des.startDecrypting;
      break;

    case pki.oids['pbewithSHAAnd40BitRC2-CBC']:
      dkLen = 5;
      dIvLen = 8;
      cipherFn = function(key, iv) {
        var cipher = forge.rc2.createDecryptionCipher(key, 40);
        cipher.start(iv, null);
        return cipher;
      };
      break;

    default:
      var error = new Error('Cannot read PKCS #12 PBE data block. Unsupported OID.');
      error.oid = oid;
      throw error;
  }

  // get PRF message digest
  var md = prfOidToMessageDigest(capture.prfOid);
  var key = pki.pbe.generatePkcs12Key(password, salt, 1, count, dkLen, md);
  md.start();
  var iv = pki.pbe.generatePkcs12Key(password, salt, 2, count, dIvLen, md);

  return cipherFn(key, iv);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pbe.opensslDeriveBytes"></a>[function <span class="apidocSignatureSpan">node-forge.pbe.</span>opensslDeriveBytes (password, salt, dkLen, md)](#apidoc.element.node-forge.pbe.opensslDeriveBytes)
- description and source-code
```javascript
opensslDeriveBytes = function (password, salt, dkLen, md) {
  if(typeof md === 'undefined' || md === null) {
    if(!('md5' in forge.md)) {
      throw new Error('"md5" hash algorithm unavailable.');
    }
    md = forge.md.md5.create();
  }
  if(salt === null) {
    salt = '';
  }
  var digests = [hash(md, password + salt)];
  for(var length = 16, i = 1; length < dkLen; ++i, length += 16) {
    digests.push(hash(md, digests[i - 1] + password + salt));
  }
  return digests.join('').substr(0, dkLen);
}
```
- example usage
```shell
...
// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
var iv = buffer.getBytes(ivSize);

var cipher = forge.cipher.createCipher('3DES-CBC', key);
cipher.start({iv: iv});
...
```



# <a name="apidoc.module.node-forge.pem"></a>[module node-forge.pem](#apidoc.module.node-forge.pem)

#### <a name="apidoc.element.node-forge.pem.decode"></a>[function <span class="apidocSignatureSpan">node-forge.pem.</span>decode (str)](#apidoc.element.node-forge.pem.decode)
- description and source-code
```javascript
decode = function (str) {
  var rval = [];

  // split string into PEM messages (be lenient w/EOF on BEGIN line)
  var rMessage = /\s*-----BEGIN ([A-Z0-9- ]+)-----\r?\n?([\x21-\x7e\s]+?(?:\r?\n\r?\n))?([:A-Za-z0-9+\/=\s]+?)-----END \1-----/g
;
  var rHeader = /([\x21-\x7e]+):\s*([\x21-\x7e\s^:]+)/;
  var rCRLF = /\r?\n/;
  var match;
  while(true) {
    match = rMessage.exec(str);
    if(!match) {
      break;
    }

    var msg = {
      type: match[1],
      procType: null,
      contentDomain: null,
      dekInfo: null,
      headers: [],
      body: forge.util.decode64(match[3])
    };
    rval.push(msg);

    // no headers
    if(!match[2]) {
      continue;
    }

    // parse headers
    var lines = match[2].split(rCRLF);
    var li = 0;
    while(match && li < lines.length) {
      // get line, trim any rhs whitespace
      var line = lines[li].replace(/\s+$/, '');

      // RFC2822 unfold any following folded lines
      for(var nl = li + 1; nl < lines.length; ++nl) {
        var next = lines[nl];
        if(!/\s/.test(next[0])) {
          break;
        }
        line += next;
        li = nl;
      }

      // parse header
      match = line.match(rHeader);
      if(match) {
        var header = {name: match[1], values: []};
        var values = match[2].split(',');
        for(var vi = 0; vi < values.length; ++vi) {
          header.values.push(ltrim(values[vi]));
        }

        // Proc-Type must be the first header
        if(!msg.procType) {
          if(header.name !== 'Proc-Type') {
            throw new Error('Invalid PEM formatted message. The first ' +
              'encapsulated header must be "Proc-Type".');
          } else if(header.values.length !== 2) {
            throw new Error('Invalid PEM formatted message. The "Proc-Type" ' +
              'header must have two subfields.');
          }
          msg.procType = {version: values[0], type: values[1]};
        } else if(!msg.contentDomain && header.name === 'Content-Domain') {
          // special-case Content-Domain
          msg.contentDomain = values[0] || '';
        } else if(!msg.dekInfo && header.name === 'DEK-Info') {
          // special-case DEK-Info
          if(header.values.length === 0) {
            throw new Error('Invalid PEM formatted message. The "DEK-Info" ' +
              'header must have at least one subfield.');
          }
          msg.dekInfo = {algorithm: values[0], parameters: values[1] || null};
        } else {
          msg.headers.push(header);
        }
      }

      ++li;
    }

    if(msg.procType === 'ENCRYPTED' && !msg.dekInfo) {
      throw new Error('Invalid PEM formatted message. The "DEK-Info" ' +
        'header must be present if "Proc-Type" is "ENCRYPTED".');
    }
  }

  if(rval.length === 0) {
    throw new Error('Invalid PEM formatted message.');
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pem.encode"></a>[function <span class="apidocSignatureSpan">node-forge.pem.</span>encode (msg, options)](#apidoc.element.node-forge.pem.encode)
- description and source-code
```javascript
encode = function (msg, options) {
  options = options || {};
  var rval = '-----BEGIN ' + msg.type + '-----\r\n';

  // encode special headers
  var header;
  if(msg.procType) {
    header = {
      name: 'Proc-Type',
      values: [String(msg.procType.version), msg.procType.type]
    };
    rval += foldHeader(header);
  }
  if(msg.contentDomain) {
    header = {name: 'Content-Domain', values: [msg.contentDomain]};
    rval += foldHeader(header);
  }
  if(msg.dekInfo) {
    header = {name: 'DEK-Info', values: [msg.dekInfo.algorithm]};
    if(msg.dekInfo.parameters) {
      header.values.push(msg.dekInfo.parameters);
    }
    rval += foldHeader(header);
  }

  if(msg.headers) {
    // encode all other headers
    for(var i = 0; i < msg.headers.length; ++i) {
      rval += foldHeader(msg.headers[i]);
    }
  }

  // terminate header
  if(msg.procType) {
    rval += '\r\n';
  }

  // add body
  rval += forge.util.encode64(msg.body, options.maxline || 64) + '\r\n';

  rval += '-----END ' + msg.type + '-----\r\n';
  return rval;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.pkcs1"></a>[module node-forge.pkcs1](#apidoc.module.node-forge.pkcs1)

#### <a name="apidoc.element.node-forge.pkcs1.decode_rsa_oaep"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs1.</span>decode_rsa_oaep (key, em, options)](#apidoc.element.node-forge.pkcs1.decode_rsa_oaep)
- description and source-code
```javascript
decode_rsa_oaep = function (key, em, options) {
  // parse args
  var label;
  var md;
  var mgf1Md;
  // legacy args
  if(typeof options === 'string') {
    label = options;
    md = arguments[3] || undefined;
  } else if(options) {
    label = options.label || undefined;
    md = options.md || undefined;
    if(options.mgf1 && options.mgf1.md) {
      mgf1Md = options.mgf1.md;
    }
  }

  // compute length in bytes
  var keyLength = Math.ceil(key.n.bitLength() / 8);

  if(em.length !== keyLength) {
    var error = new Error('RSAES-OAEP encoded message length is invalid.');
    error.length = em.length;
    error.expectedLength = keyLength;
    throw error;
  }

  // default OAEP to SHA-1 message digest
  if(md === undefined) {
    md = forge.md.sha1.create();
  } else {
    md.start();
  }

  // default MGF-1 to same as OAEP
  if(!mgf1Md) {
    mgf1Md = md;
  }

  if(keyLength < 2 * md.digestLength + 2) {
    throw new Error('RSAES-OAEP key is too short for the hash function.');
  }

  if(!label) {
    label = '';
  }
  md.update(label, 'raw');
  var lHash = md.digest().getBytes();

  // split the message into its parts
  var y = em.charAt(0);
  var maskedSeed = em.substring(1, md.digestLength + 1);
  var maskedDB = em.substring(1 + md.digestLength);

  var seedMask = rsa_mgf1(maskedDB, md.digestLength, mgf1Md);
  var seed = forge.util.xorBytes(maskedSeed, seedMask, maskedSeed.length);

  var dbMask = rsa_mgf1(seed, keyLength - md.digestLength - 1, mgf1Md);
  var db = forge.util.xorBytes(maskedDB, dbMask, maskedDB.length);

  var lHashPrime = db.substring(0, md.digestLength);

  // constant time check that all values match what is expected
  var error = (y !== '\x00');

  // constant time check lHash vs lHashPrime
  for(var i = 0; i < md.digestLength; ++i) {
    error |= (lHash.charAt(i) !== lHashPrime.charAt(i));
  }

  // "constant time" find the 0x1 byte separating the padding (zeros) from the
  // message
  // TODO: It must be possible to do this in a better/smarter way?
  var in_ps = 1;
  var index = md.digestLength;
  for(var j = md.digestLength; j < db.length; j++) {
    var code = db.charCodeAt(j);

    var is_0 = (code & 0x1) ^ 0x1;

    // non-zero if not 0 or 1 in the ps section
    var error_mask = in_ps ? 0xfffe : 0x0000;
    error |= (code & error_mask);

    // latch in_ps to zero after we find 0x1
    in_ps = in_ps & is_0;
    index += in_ps;
  }

  if(error || db.charCodeAt(index) !== 0x1) {
    throw new Error('Invalid RSAES-OAEP padding.');
  }

  return db.substring(index + 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pkcs1.encode_rsa_oaep"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs1.</span>encode_rsa_oaep (key, message, options)](#apidoc.element.node-forge.pkcs1.encode_rsa_oaep)
- description and source-code
```javascript
encode_rsa_oaep = function (key, message, options) {
  // parse arguments
  var label;
  var seed;
  var md;
  var mgf1Md;
  // legacy args (label, seed, md)
  if(typeof options === 'string') {
    label = options;
    seed = arguments[3] || undefined;
    md = arguments[4] || undefined;
  } else if(options) {
    label = options.label || undefined;
    seed = options.seed || undefined;
    md = options.md || undefined;
    if(options.mgf1 && options.mgf1.md) {
      mgf1Md = options.mgf1.md;
    }
  }

  // default OAEP to SHA-1 message digest
  if(!md) {
    md = forge.md.sha1.create();
  } else {
    md.start();
  }

  // default MGF-1 to same as OAEP
  if(!mgf1Md) {
    mgf1Md = md;
  }

  // compute length in bytes and check output
  var keyLength = Math.ceil(key.n.bitLength() / 8);
  var maxLength = keyLength - 2 * md.digestLength - 2;
  if(message.length > maxLength) {
    var error = new Error('RSAES-OAEP input message length is too long.');
    error.length = message.length;
    error.maxLength = maxLength;
    throw error;
  }

  if(!label) {
    label = '';
  }
  md.update(label, 'raw');
  var lHash = md.digest();

  var PS = '';
  var PS_length = maxLength - message.length;
  for (var i = 0; i < PS_length; i++) {
    PS += '\x00';
  }

  var DB = lHash.getBytes() + PS + '\x01' + message;

  if(!seed) {
    seed = forge.random.getBytes(md.digestLength);
  } else if(seed.length !== md.digestLength) {
    var error = new Error('Invalid RSAES-OAEP seed. The seed length must ' +
      'match the digest length.');
    error.seedLength = seed.length;
    error.digestLength = md.digestLength;
    throw error;
  }

  var dbMask = rsa_mgf1(seed, keyLength - md.digestLength - 1, mgf1Md);
  var maskedDB = forge.util.xorBytes(DB, dbMask, DB.length);

  var seedMask = rsa_mgf1(maskedDB, md.digestLength, mgf1Md);
  var maskedSeed = forge.util.xorBytes(seed, seedMask, seed.length);

  // return encoded message
  return '\x00' + maskedSeed + maskedDB;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.pkcs12"></a>[module node-forge.pkcs12](#apidoc.module.node-forge.pkcs12)

#### <a name="apidoc.element.node-forge.pkcs12.generateKey"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs12.</span>generateKey (password, salt, id, iter, n, md)](#apidoc.element.node-forge.pkcs12.generateKey)
- description and source-code
```javascript
generateKey = function (password, salt, id, iter, n, md) {
  var j, l;

  if(typeof md === 'undefined' || md === null) {
    if(!('sha1' in forge.md)) {
      throw new Error('"sha1" hash algorithm unavailable.');
    }
    md = forge.md.sha1.create();
  }

  var u = md.digestLength;
  var v = md.blockLength;
  var result = new forge.util.ByteBuffer();

<span class="apidocCodeCommentSpan">  /* Convert password to Unicode byte buffer + trailing 0-byte. */
</span>  var passBuf = new forge.util.ByteBuffer();
  if(password !== null && password !== undefined) {
    for(l = 0; l < password.length; l++) {
      passBuf.putInt16(password.charCodeAt(l));
    }
    passBuf.putInt16(0);
  }

  /* Length of salt and password in BYTES. */
  var p = passBuf.length();
  var s = salt.length();

  /* 1. Construct a string, D (the "diversifier"), by concatenating
        v copies of ID. */
  var D = new forge.util.ByteBuffer();
  D.fillWithByte(id, v);

  /* 2. Concatenate copies of the salt together to create a string S of length
        v * ceil(s / v) bytes (the final copy of the salt may be trunacted
        to create S).
        Note that if the salt is the empty string, then so is S. */
  var Slen = v * Math.ceil(s / v);
  var S = new forge.util.ByteBuffer();
  for(l = 0; l < Slen; l++) {
    S.putByte(salt.at(l % s));
  }

  /* 3. Concatenate copies of the password together to create a string P of
        length v * ceil(p / v) bytes (the final copy of the password may be
        truncated to create P).
        Note that if the password is the empty string, then so is P. */
  var Plen = v * Math.ceil(p / v);
  var P = new forge.util.ByteBuffer();
  for(l = 0; l < Plen; l++) {
    P.putByte(passBuf.at(l % p));
  }

  /* 4. Set I=S||P to be the concatenation of S and P. */
  var I = S;
  I.putBuffer(P);

  /* 5. Set c=ceil(n / u). */
  var c = Math.ceil(n / u);

  /* 6. For i=1, 2, ..., c, do the following: */
  for(var i = 1; i <= c; i++) {
    /* a) Set Ai=H^r(D||I). (l.e. the rth hash of D||I, H(H(H(...H(D||I)))) */
    var buf = new forge.util.ByteBuffer();
    buf.putBytes(D.bytes());
    buf.putBytes(I.bytes());
    for(var round = 0; round < iter; round++) {
      md.start();
      md.update(buf.getBytes());
      buf = md.digest();
    }

    /* b) Concatenate copies of Ai to create a string B of length v bytes (the
          final copy of Ai may be truncated to create B). */
    var B = new forge.util.ByteBuffer();
    for(l = 0; l < v; l++) {
      B.putByte(buf.at(l % u));
    }

    /* c) Treating I as a concatenation I0, I1, ..., Ik-1 of v-byte blocks,
          where k=ceil(s / v) + ceil(p / v), modify I by setting
          Ij=(Ij+B+1) mod 2v for each j.  */
    var k = Math.ceil(s / v) + Math.ceil(p / v);
    var Inew = new forge.util.ByteBuffer();
    for(j = 0; j < k; j++) {
      var chunk = new forge.util.ByteBuffer(I.getBytes(v));
      var x = 0x1ff;
      for(l = B.length() - 1; l >= 0; l--) {
        x = x >> 8;
        x += B.at(l) + chunk.at(l);
        chunk.setAt(l, x & 0xff);
      }
      Inew.putBuffer(chunk);
    }
    I = Inew;

    /* Add Ai to A. */
    result.putBuffer(buf);
  }

  result.truncate(result.length() - n);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pkcs12.pkcs12FromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs12.</span>pkcs12FromAsn1 (obj, strict, password)](#apidoc.element.node-forge.pkcs12.pkcs12FromAsn1)
- description and source-code
```javascript
pkcs12FromAsn1 = function (obj, strict, password) {
  // handle args
  if(typeof strict === 'string') {
    password = strict;
    strict = true;
  } else if(strict === undefined) {
    strict = true;
  }

  // validate PFX and capture data
  var capture = {};
  var errors = [];
  if(!asn1.validate(obj, pfxValidator, capture, errors)) {
    var error = new Error('Cannot read PKCS#12 PFX. ' +
      'ASN.1 object is not an PKCS#12 PFX.');
    error.errors = error;
    throw error;
  }

  var pfx = {
    version: capture.version.charCodeAt(0),
    safeContents: [],

<span class="apidocCodeCommentSpan">    /**
     * Gets bags with matching attributes.
     *
     * @param filter the attributes to filter by:
     *          [localKeyId] the localKeyId to search for.
     *          [localKeyIdHex] the localKeyId in hex to search for.
     *          [friendlyName] the friendly name to search for.
     *          [bagType] bag type to narrow each attribute search by.
     *
     * @return a map of attribute type to an array of matching bags or, if no
     *           attribute was given but a bag type, the map key will be the
     *           bag type.
     */
</span>    getBags: function(filter) {
      var rval = {};

      var localKeyId;
      if('localKeyId' in filter) {
        localKeyId = filter.localKeyId;
      } else if('localKeyIdHex' in filter) {
        localKeyId = forge.util.hexToBytes(filter.localKeyIdHex);
      }

      // filter on bagType only
      if(localKeyId === undefined && !('friendlyName' in filter) &&
        'bagType' in filter) {
        rval[filter.bagType] = _getBagsByAttribute(
          pfx.safeContents, null, null, filter.bagType);
      }

      if(localKeyId !== undefined) {
        rval.localKeyId = _getBagsByAttribute(
          pfx.safeContents, 'localKeyId',
          localKeyId, filter.bagType);
      }
      if('friendlyName' in filter) {
        rval.friendlyName = _getBagsByAttribute(
          pfx.safeContents, 'friendlyName',
          filter.friendlyName, filter.bagType);
      }

      return rval;
    },

    /**
     * DEPRECATED: use getBags() instead.
     *
     * Get bags with matching friendlyName attribute.
     *
     * @param friendlyName the friendly name to search for.
     * @param [bagType] bag type to narrow search by.
     *
     * @return an array of bags with matching friendlyName attribute.
     */
    getBagsByFriendlyName: function(friendlyName, bagType) {
      return _getBagsByAttribute(
        pfx.safeContents, 'friendlyName', friendlyName, bagType);
    },

    /**
     * DEPRECATED: use getBags() instead.
     *
     * Get bags with matching localKeyId attribute.
     *
     * @param localKeyId the localKeyId to search for.
     * @param [bagType] bag type to narrow search by.
     *
     * @return an array of bags with matching localKeyId attribute.
     */
    getBagsByLocalKeyId: function(localKeyId, bagType) {
      return _getBagsByAttribute(
        pfx.safeContents, 'localKeyId', localKeyId, bagType);
    }
  };

  if(capture.version.charCodeAt(0) !== 3) {
    var error = new Error('PKCS#12 PFX of version other than 3 not supported.');
    error.version = capture.version.charCodeAt(0);
    throw error;
  }

  if(asn1.derToOid(capture.contentType) !== pki.oids.data) {
    var error = new Error('Only PKCS#12 PFX in password integrity mode supported.');
    error.oid = asn1.derToOid(capture.contentType);
    throw error;
  }

  var data = capture.content.value[0];
  if(data.tagClass !== asn1.Class.UNIVERSAL ||
     data.type !== asn1.Type.OCTETSTRING) {
    throw new Error('PKCS#12 authSafe content data is not an OCTET STRING.');
  }
  data = _decodePkcs7Data(data);

  // check for MAC
  if(capture.mac) {
    var md = null;
    var macKeyBytes = 0;
    var macAlgorithm = asn1.derToOid(capture.macAlgorithm);
    switch(macAlgorithm) {
    case pki.oids.sha1:
      md = forge.md.sha1.create();
      macKeyBytes = 20;
      break;
    case pki.oids.sha256:
      md = forge.md.sha256.create();
      macKeyBytes = 32;
      break;
    case pki.oids.sha384:
      md = forge.md.sha384.create();
      macKeyByte ...
```
- example usage
```shell
...

'''js
// decode p12 from base64
var p12Der = forge.util.decode64(p12b64);
// get p12 as ASN.1 object
var p12Asn1 = forge.asn1.fromDer(p12Der);
// decrypt p12 using the password 'password'
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, 'password');
// decrypt p12 using non-strict parsing mode (resolves some ASN.1 parse errors)
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, false, 'password');
// decrypt p12 using literally no password (eg: Mac OS X/apple push)
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1);
// decrypt p12 using an "empty" password (eg: OpenSSL with no password input)
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, '');
// p12.safeContents is an array of safe contents, each of
...
```

#### <a name="apidoc.element.node-forge.pkcs12.toPkcs12Asn1"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs12.</span>toPkcs12Asn1 (key, cert, password, options)](#apidoc.element.node-forge.pkcs12.toPkcs12Asn1)
- description and source-code
```javascript
toPkcs12Asn1 = function (key, cert, password, options) {
  // set default options
  options = options || {};
  options.saltSize = options.saltSize || 8;
  options.count = options.count || 2048;
  options.algorithm = options.algorithm || options.encAlgorithm || 'aes128';
  if(!('useMac' in options)) {
    options.useMac = true;
  }
  if(!('localKeyId' in options)) {
    options.localKeyId = null;
  }
  if(!('generateLocalKeyId' in options)) {
    options.generateLocalKeyId = true;
  }

  var localKeyId = options.localKeyId;
  var bagAttrs;
  if(localKeyId !== null) {
    localKeyId = forge.util.hexToBytes(localKeyId);
  } else if(options.generateLocalKeyId) {
    // use SHA-1 of paired cert, if available
    if(cert) {
      var pairedCert = forge.util.isArray(cert) ? cert[0] : cert;
      if(typeof pairedCert === 'string') {
        pairedCert = pki.certificateFromPem(pairedCert);
      }
      var sha1 = forge.md.sha1.create();
      sha1.update(asn1.toDer(pki.certificateToAsn1(pairedCert)).getBytes());
      localKeyId = sha1.digest().getBytes();
    } else {
      // FIXME: consider using SHA-1 of public key (which can be generated
      // from private key components), see: cert.generateSubjectKeyIdentifier
      // generate random bytes
      localKeyId = forge.random.getBytes(20);
    }
  }

  var attrs = [];
  if(localKeyId !== null) {
    attrs.push(
      // localKeyID
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
        // attrId
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
          asn1.oidToDer(pki.oids.localKeyId).getBytes()),
        // attrValues
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SET, true, [
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OCTETSTRING, false,
            localKeyId)
        ])
      ]));
  }
  if('friendlyName' in options) {
    attrs.push(
      // friendlyName
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
        // attrId
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
          asn1.oidToDer(pki.oids.friendlyName).getBytes()),
        // attrValues
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SET, true, [
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BMPSTRING, false,
            options.friendlyName)
        ])
      ]));
  }

  if(attrs.length > 0) {
    bagAttrs = asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SET, true, attrs);
  }

  // collect contents for AuthenticatedSafe
  var contents = [];

  // create safe bag(s) for certificate chain
  var chain = [];
  if(cert !== null) {
    if(forge.util.isArray(cert)) {
      chain = cert;
    } else {
      chain = [cert];
    }
  }

  var certSafeBags = [];
  for(var i = 0; i < chain.length; ++i) {
    // convert cert from PEM as necessary
    cert = chain[i];
    if(typeof cert === 'string') {
      cert = pki.certificateFromPem(cert);
    }

    // SafeBag
    var certBagAttrs = (i === 0) ? bagAttrs : undefined;
    var certAsn1 = pki.certificateToAsn1(cert);
    var certSafeBag =
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
        // bagId
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
          asn1.oidToDer(pki.oids.certBag).getBytes()),
        // bagValue
        asn1.create(asn1.Class.CONTEXT_SPECIFIC, 0, true, [
          // CertBag
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
            // certId
            asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
              asn1.oidToDer(pki.oids.x509Certificate).getBytes()),
            // certValue (x509Certificate)
            asn1.create(asn1.Class.CONTEXT_SPECIFIC, 0, true, [
              asn1.create(
                asn1.Class.UNIVERSAL, asn1.Type.OCTETSTRING, false,
                asn1.toDer(certAsn1).getBytes())
            ])])]),
        // bagAttributes (OPTIONAL)
        certBagAttrs
      ]);
    certSafeBags.push(certSafeBag);
  }

  if(certSafeBags.length > 0) {
    // SafeContents
    var certSafeContents = asn1.create(
      asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, certSafeBags ...
```
- example usage
```shell
...
// representation of the key
if(bag.key === null) {
var keyAsn1 = bag.asn1;
// can now convert back to DER/PEM/etc for export
}

// generate a p12 using AES (default)
var p12Asn1 = forge.pkcs12.toPkcs12Asn1(
privateKey, certificateChain, 'password');

// generate a p12 that can be imported by Chrome/Firefox/iOS
// (requires the use of Triple DES instead of AES)
var p12Asn1 = forge.pkcs12.toPkcs12Asn1(
privateKey, certificateChain, 'password',
{algorithm: '3des'});
...
```



# <a name="apidoc.module.node-forge.pkcs5"></a>[module node-forge.pkcs5](#apidoc.module.node-forge.pkcs5)

#### <a name="apidoc.element.node-forge.pkcs5.pbkdf2"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs5.</span>pbkdf2 ( p, s, c, dkLen, md, callback)](#apidoc.element.node-forge.pkcs5.pbkdf2)
- description and source-code
```javascript
pbkdf2 = function ( p, s, c, dkLen, md, callback) {
  if(typeof md === 'function') {
    callback = md;
    md = null;
  }

  // use native implementation if possible and not disabled, note that
  // some node versions only support SHA-1, others allow digest to be changed
  if(forge.util.isNodejs && !forge.options.usePureJavaScript &&
    crypto.pbkdf2 && (md === null || typeof md !== 'object') &&
    (crypto.pbkdf2Sync.length > 4 || (!md || md === 'sha1'))) {
    if(typeof md !== 'string') {
      // default prf to SHA-1
      md = 'sha1';
    }
    p = new Buffer(p, 'binary');
    s = new Buffer(s, 'binary');
    if(!callback) {
      if(crypto.pbkdf2Sync.length === 4) {
        return crypto.pbkdf2Sync(p, s, c, dkLen).toString('binary');
      }
      return crypto.pbkdf2Sync(p, s, c, dkLen, md).toString('binary');
    }
    if(crypto.pbkdf2Sync.length === 4) {
      return crypto.pbkdf2(p, s, c, dkLen, function(err, key) {
        if(err) {
          return callback(err);
        }
        callback(null, key.toString('binary'));
      });
    }
    return crypto.pbkdf2(p, s, c, dkLen, md, function(err, key) {
      if(err) {
        return callback(err);
      }
      callback(null, key.toString('binary'));
    });
  }

  if(typeof md === 'undefined' || md === null) {
    // default prf to SHA-1
    md = 'sha1';
  }
  if(typeof md === 'string') {
    if(!(md in forge.md.algorithms)) {
      throw new Error('Unknown hash algorithm: ' + md);
    }
    md = forge.md[md].create();
  }

  var hLen = md.digestLength;

<span class="apidocCodeCommentSpan">  /* 1. If dkLen > (2^32 - 1) * hLen, output "derived key too long" and
    stop. */
</span>  if(dkLen > (0xFFFFFFFF * hLen)) {
    var err = new Error('Derived key is too long.');
    if(callback) {
      return callback(err);
    }
    throw err;
  }

  /* 2. Let len be the number of hLen-octet blocks in the derived key,
    rounding up, and let r be the number of octets in the last
    block:

    len = CEIL(dkLen / hLen),
    r = dkLen - (len - 1) * hLen. */
  var len = Math.ceil(dkLen / hLen);
  var r = dkLen - (len - 1) * hLen;

  /* 3. For each block of the derived key apply the function F defined
    below to the password P, the salt S, the iteration count c, and
    the block index to compute the block:

    T_1 = F(P, S, c, 1),
    T_2 = F(P, S, c, 2),
    ...
    T_len = F(P, S, c, len),

    where the function F is defined as the exclusive-or sum of the
    first c iterates of the underlying pseudorandom function PRF
    applied to the password P and the concatenation of the salt S
    and the block index i:

    F(P, S, c, i) = u_1 XOR u_2 XOR ... XOR u_c

    where

    u_1 = PRF(P, S || INT(i)),
    u_2 = PRF(P, u_1),
    ...
    u_c = PRF(P, u_{c-1}).

    Here, INT(i) is a four-octet encoding of the integer i, most
    significant octet first. */
  var prf = forge.hmac.create();
  prf.start(md, p);
  var dk = '';
  var xor, u_c, u_c1;

  // sync version
  if(!callback) {
    for(var i = 1; i <= len; ++i) {
      // PRF(P, S || INT(i)) (first iteration)
      prf.start(null, null);
      prf.update(s);
      prf.update(forge.util.int32ToBytes(i));
      xor = u_c1 = prf.digest().getBytes();

      // PRF(P, u_{c-1}) (other iterations)
      for(var j = 2; j <= c; ++j) {
        prf.start(null, null);
        prf.update(u_c1);
        u_c = prf.digest().getBytes();
        // F(p, s, c, i)
        xor = forge.util.xorBytes(xor, u_c, hLen);
        u_c1 = u_c;
      }

      /* 4. Concatenate the blocks and extract the first dkLen octets to
        produce a derived key DK:

        DK = T_1 || T_2 ||  ...  || T_len<0..r-1> */
      dk += (i < len) ? xor : xor.substr(0, r);
    }
    /* 5. Output the derived key DK. */
    return dk;
  }

  // async version
  var i = 1, j;
  function outer() {
    if(i > len) {
      // done
      return callback(null, dk);
    }

    // PRF(P, S || INT(i)) (first iteration)
    prf.start(null, null);
    prf.update(s);
    prf.update(forge.util.int32ToBytes(i));
    xor = u_c1 = prf.digest().getBytes();

    // PRF(P, u_{c-1}) (other iterations)
    j = 2;
    inner();
  } ...
```
- example usage
```shell
...
// generate a random key and IV
// Note: a key size of 16 bytes will use AES-128, 24 => AES-192, 32 => AES-256
var key = forge.random.getBytesSync(16);
var iv = forge.random.getBytesSync(16);

/* alternatively, generate a password-based 16-byte key
var salt = forge.random.getBytesSync(128);
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
...
```



# <a name="apidoc.module.node-forge.pkcs7"></a>[module node-forge.pkcs7](#apidoc.module.node-forge.pkcs7)

#### <a name="apidoc.element.node-forge.pkcs7.createEncryptedData"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>createEncryptedData ()](#apidoc.element.node-forge.pkcs7.createEncryptedData)
- description and source-code
```javascript
createEncryptedData = function () {
  var msg = null;
  msg = {
    type: forge.pki.oids.encryptedData,
    version: 0,
    encryptedContent: {
      algorithm: forge.pki.oids['aes256-CBC']
    },

<span class="apidocCodeCommentSpan">    /**
     * Reads an EncryptedData content block (in ASN.1 format)
     *
     * @param obj The ASN.1 representation of the EncryptedData content block
     */
</span>    fromAsn1: function(obj) {
      // Validate EncryptedData content block and capture data.
      _fromAsn1(msg, obj, p7.asn1.encryptedDataValidator);
    },

    /**
     * Decrypt encrypted content
     *
     * @param key The (symmetric) key as a byte buffer
     */
    decrypt: function(key) {
      if(key !== undefined) {
        msg.encryptedContent.key = key;
      }
      _decryptContent(msg);
    }
  };
  return msg;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pkcs7.createEnvelopedData"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>createEnvelopedData ()](#apidoc.element.node-forge.pkcs7.createEnvelopedData)
- description and source-code
```javascript
createEnvelopedData = function () {
  var msg = null;
  msg = {
    type: forge.pki.oids.envelopedData,
    version: 0,
    recipients: [],
    encryptedContent: {
      algorithm: forge.pki.oids['aes256-CBC']
    },

<span class="apidocCodeCommentSpan">    /**
     * Reads an EnvelopedData content block (in ASN.1 format)
     *
     * @param obj the ASN.1 representation of the EnvelopedData content block.
     */
</span>    fromAsn1: function(obj) {
      // validate EnvelopedData content block and capture data
      var capture = _fromAsn1(msg, obj, p7.asn1.envelopedDataValidator);
      msg.recipients = _recipientsFromAsn1(capture.recipientInfos.value);
    },

    toAsn1: function() {
      // ContentInfo
      return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
        // ContentType
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
          asn1.oidToDer(msg.type).getBytes()),
        // [0] EnvelopedData
        asn1.create(asn1.Class.CONTEXT_SPECIFIC, 0, true, [
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
            // Version
            asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
              asn1.integerToDer(msg.version).getBytes()),
            // RecipientInfos
            asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SET, true,
              _recipientsToAsn1(msg.recipients)),
            // EncryptedContentInfo
            asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true,
              _encryptedContentToAsn1(msg.encryptedContent))
          ])
        ])
      ]);
    },

    /**
     * Find recipient by X.509 certificate's issuer.
     *
     * @param cert the certificate with the issuer to look for.
     *
     * @return the recipient object.
     */
    findRecipient: function(cert) {
      var sAttr = cert.issuer.attributes;

      for(var i = 0; i < msg.recipients.length; ++i) {
        var r = msg.recipients[i];
        var rAttr = r.issuer;

        if(r.serialNumber !== cert.serialNumber) {
          continue;
        }

        if(rAttr.length !== sAttr.length) {
          continue;
        }

        var match = true;
        for(var j = 0; j < sAttr.length; ++j) {
          if(rAttr[j].type !== sAttr[j].type ||
            rAttr[j].value !== sAttr[j].value) {
            match = false;
            break;
          }
        }

        if(match) {
          return r;
        }
      }

      return null;
    },

    /**
     * Decrypt enveloped content
     *
     * @param recipient The recipient object related to the private key
     * @param privKey The (RSA) private key object
     */
    decrypt: function(recipient, privKey) {
      if(msg.encryptedContent.key === undefined && recipient !== undefined &&
        privKey !== undefined) {
        switch(recipient.encryptedContent.algorithm) {
          case forge.pki.oids.rsaEncryption:
          case forge.pki.oids.desCBC:
            var key = privKey.decrypt(recipient.encryptedContent.content);
            msg.encryptedContent.key = forge.util.createBuffer(key);
            break;

          default:
            throw new Error('Unsupported asymmetric cipher, ' +
              'OID ' + recipient.encryptedContent.algorithm);
        }
      }

      _decryptContent(msg);
    },

    /**
     * Add (another) entity to list of recipients.
     *
     * @param cert The certificate of the entity to add.
     */
    addRecipient: function(cert) {
      msg.recipients.push({
        version: 0,
        issuer: cert.issuer.attributes,
        serialNumber: cert.serialNumber,
        encryptedContent: {
          // We simply assume rsaEncryption here, since forge.pki only
          // supports RSA so far.  If the PKI module supports other
          // ciphers one day, we need to modify this one as well.
          algorithm: forge.pki.oids.rsaEncryption,
          key: cert.publicKey
        }
      });
    },

    /**
     * Encrypt enveloped content.
     *
     * This function supports two optional arguments, cipher and key, which
     * can be used to influence symmetric encryption.  Unless cipher is
     * provided, the cip ...
```
- example usage
```shell
...
// find a recipient by the issuer of a certificate
var recipient = p7.findRecipient(cert);

// decrypt
p7.decrypt(p7.recipients[0], privateKey);

// create a p7 enveloped message
var p7 = forge.pkcs7.createEnvelopedData();

// add a recipient
var cert = forge.pki.certificateFromPem(certPem);
p7.addRecipient(cert);

// set content
p7.content = forge.util.createBuffer('Hello');
...
```

#### <a name="apidoc.element.node-forge.pkcs7.createSignedData"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>createSignedData ()](#apidoc.element.node-forge.pkcs7.createSignedData)
- description and source-code
```javascript
createSignedData = function () {
  var msg = null;
  msg = {
    type: forge.pki.oids.signedData,
    version: 1,
    certificates: [],
    crls: [],
    // TODO: add json-formatted signer stuff here?
    signers: [],
    // populated during sign()
    digestAlgorithmIdentifiers: [],
    contentInfo: null,
    signerInfos: [],

    fromAsn1: function(obj) {
      // validate SignedData content block and capture data.
      _fromAsn1(msg, obj, p7.asn1.signedDataValidator);
      msg.certificates = [];
      msg.crls = [];
      msg.digestAlgorithmIdentifiers = [];
      msg.contentInfo = null;
      msg.signerInfos = [];

      var certs = msg.rawCapture.certificates.value;
      for(var i = 0; i < certs.length; ++i) {
        msg.certificates.push(forge.pki.certificateFromAsn1(certs[i]));
      }

      // TODO: parse crls
    },

    toAsn1: function() {
      // degenerate case with no content
      if(!msg.contentInfo) {
        msg.sign();
      }

      var certs = [];
      for(var i = 0; i < msg.certificates.length; ++i) {
        certs.push(forge.pki.certificateToAsn1(msg.certificates[i]));
      }

      var crls = [];
      // TODO: implement CRLs

      // [0] SignedData
      var signedData = asn1.create(asn1.Class.CONTEXT_SPECIFIC, 0, true, [
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
          // Version
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
            asn1.integerToDer(msg.version).getBytes()),
          // DigestAlgorithmIdentifiers
          asn1.create(
            asn1.Class.UNIVERSAL, asn1.Type.SET, true,
            msg.digestAlgorithmIdentifiers),
          // ContentInfo
          msg.contentInfo
        ])
      ]);
      if(certs.length > 0) {
        // [0] IMPLICIT ExtendedCertificatesAndCertificates OPTIONAL
        signedData.value[0].value.push(
          asn1.create(asn1.Class.CONTEXT_SPECIFIC, 0, true, certs));
      }
      if(crls.length > 0) {
        // [1] IMPLICIT CertificateRevocationLists OPTIONAL
        signedData.value[0].value.push(
          asn1.create(asn1.Class.CONTEXT_SPECIFIC, 1, true, crls));
      }
      // SignerInfos
      signedData.value[0].value.push(
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SET, true,
          msg.signerInfos));

      // ContentInfo
      return asn1.create(
        asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
          // ContentType
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
            asn1.oidToDer(msg.type).getBytes()),
          // [0] SignedData
          signedData
        ]);
    },

    /**
     * Add (another) entity to list of signers.
     *
     * Note: If authenticatedAttributes are provided, then, per RFC 2315,
     * they must include at least two attributes: content type and
     * message digest. The message digest attribute value will be
     * auto-calculated during signing and will be ignored if provided.
     *
     * Here's an example of providing these two attributes:
     *
     * forge.pkcs7.createSignedData();
     * p7.addSigner({
     *   issuer: cert.issuer.attributes,
     *   serialNumber: cert.serialNumber,
     *   key: privateKey,
     *   digestAlgorithm: forge.pki.oids.sha1,
     *   authenticatedAttributes: [{
     *     type: forge.pki.oids.contentType,
     *     value: forge.pki.oids.data
     *   }, {
     *     type: forge.pki.oids.messageDigest
     *   }]
     * });
     *
     * TODO: Support [subjectKeyIdentifier] as signer's ID.
     *
     * @param signer the signer information:
     *          key the signer's private key.
     *          [certificate] a certificate containing the public key
     *            associated with the signer's private key; use this option as
     *            an alternative to specifying signer.issuer and
     *            signer.serialNumber.
     *          [issuer] the issuer attributes (eg: cert.issuer.attributes).
     *          [serialNumber] the signer's certificate's serial number in
     *           hexadecimal (eg: cert.serialNumber).
     *          [digestAlgorithm] the messa ...
```
- example usage
```shell
...
p7.encrypt();

// convert message to PEM
var pem = forge.pkcs7.messageToPem(p7);

// create a degenerate PKCS#7 certificate container
// (CRLs not currently supported, only certificates)
var p7 = forge.pkcs7.createSignedData();
p7.addCertificate(certOrCertPem1);
p7.addCertificate(certOrCertPem2);
var pem = forge.pkcs7.messageToPem(p7);

// create PKCS#7 signed data with authenticatedAttributes
// attributes include: PKCS#9 content-type, message-digest, and signing-time
var p7 = forge.pkcs7.createSignedData();
...
```

#### <a name="apidoc.element.node-forge.pkcs7.messageFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>messageFromAsn1 (obj)](#apidoc.element.node-forge.pkcs7.messageFromAsn1)
- description and source-code
```javascript
messageFromAsn1 = function (obj) {
  // validate root level ContentInfo and capture data
  var capture = {};
  var errors = [];
  if(!asn1.validate(obj, p7.asn1.contentInfoValidator, capture, errors)) {
    var error = new Error('Cannot read PKCS#7 message. ' +
      'ASN.1 object is not an PKCS#7 ContentInfo.');
    error.errors = errors;
    throw error;
  }

  var contentType = asn1.derToOid(capture.contentType);
  var msg;

  switch(contentType) {
    case forge.pki.oids.envelopedData:
      msg = p7.createEnvelopedData();
      break;

    case forge.pki.oids.encryptedData:
      msg = p7.createEncryptedData();
      break;

    case forge.pki.oids.signedData:
      msg = p7.createSignedData();
      break;

    default:
      throw new Error('Cannot read PKCS#7 message. ContentType with OID ' +
        contentType + ' is not (yet) supported.');
  }

  msg.fromAsn1(capture.content.value[0]);
  return msg;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pkcs7.messageFromPem"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>messageFromPem (pem)](#apidoc.element.node-forge.pkcs7.messageFromPem)
- description and source-code
```javascript
messageFromPem = function (pem) {
  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'PKCS7') {
    var error = new Error('Could not convert PKCS#7 message from PEM; PEM ' +
      'header type is not "PKCS#7".');
    error.headerType = msg.type;
    throw error;
  }
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert PKCS#7 message from PEM; PEM is encrypted.');
  }

  // convert DER to ASN.1 object
  var obj = asn1.fromDer(msg.body);

  return p7.messageFromAsn1(obj);
}
```
- example usage
```shell
...

Provides cryptographically protected messages from [PKCS#7][].

__Examples__

'''js
// convert a message from PEM
var p7 = forge.pkcs7.messageFromPem(pem);
// look at p7.recipients

// find a recipient by the issuer of a certificate
var recipient = p7.findRecipient(cert);

// decrypt
p7.decrypt(p7.recipients[0], privateKey);
...
```

#### <a name="apidoc.element.node-forge.pkcs7.messageToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pkcs7.</span>messageToPem (msg, maxline)](#apidoc.element.node-forge.pkcs7.messageToPem)
- description and source-code
```javascript
messageToPem = function (msg, maxline) {
  // convert to ASN.1, then DER, then PEM-encode
  var pemObj = {
    type: 'PKCS7',
    body: asn1.toDer(msg.toAsn1()).getBytes()
  };
  return forge.pem.encode(pemObj, {maxline: maxline});
}
```
- example usage
```shell
...
// set content
p7.content = forge.util.createBuffer('Hello');

// encrypt
p7.encrypt();

// convert message to PEM
var pem = forge.pkcs7.messageToPem(p7);

// create a degenerate PKCS#7 certificate container
// (CRLs not currently supported, only certificates)
var p7 = forge.pkcs7.createSignedData();
p7.addCertificate(certOrCertPem1);
p7.addCertificate(certOrCertPem2);
var pem = forge.pkcs7.messageToPem(p7);
...
```



# <a name="apidoc.module.node-forge.pki"></a>[module node-forge.pki](#apidoc.module.node-forge.pki)

#### <a name="apidoc.element.node-forge.pki.CRIAttributesAsArray"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>CRIAttributesAsArray (attributes)](#apidoc.element.node-forge.pki.CRIAttributesAsArray)
- description and source-code
```javascript
CRIAttributesAsArray = function (attributes) {
  var rval = [];

  // each value in 'attributes' in is a SEQUENCE with an OID and a SET
  for(var si = 0; si < attributes.length; ++si) {
    // get the attribute sequence
    var seq = attributes[si];

    // each value in the SEQUENCE containing first a type (an OID) and
    // second a set of values (defined by the OID)
    var type = asn1.derToOid(seq.value[0].value);
    var values = seq.value[1].value;
    for(var vi = 0; vi < values.length; ++vi) {
      var obj = {};
      obj.type = type;
      obj.value = values[vi].value;
      obj.valueTagClass = values[vi].type;
      // if the OID is known, get its name and short name
      if(obj.type in oids) {
        obj.name = oids[obj.type];
        if(obj.name in _shortNames) {
          obj.shortName = _shortNames[obj.name];
        }
      }
      // parse extensions
      if(obj.type === oids.extensionRequest) {
        obj.extensions = [];
        for(var ei = 0; ei < obj.value.length; ++ei) {
          obj.extensions.push(pki.certificateExtensionFromAsn1(obj.value[ei]));
        }
      }
      rval.push(obj);
    }
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.RDNAttributesAsArray"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>RDNAttributesAsArray (rdn, md)](#apidoc.element.node-forge.pki.RDNAttributesAsArray)
- description and source-code
```javascript
RDNAttributesAsArray = function (rdn, md) {
  var rval = [];

  // each value in 'rdn' in is a SET of RelativeDistinguishedName
  var set, attr, obj;
  for(var si = 0; si < rdn.value.length; ++si) {
    // get the RelativeDistinguishedName set
    set = rdn.value[si];

    // each value in the SET is an AttributeTypeAndValue sequence
    // containing first a type (an OID) and second a value (defined by
    // the OID)
    for(var i = 0; i < set.value.length; ++i) {
      obj = {};
      attr = set.value[i];
      obj.type = asn1.derToOid(attr.value[0].value);
      obj.value = attr.value[1].value;
      obj.valueTagClass = attr.value[1].type;
      // if the OID is known, get its name and short name
      if(obj.type in oids) {
        obj.name = oids[obj.type];
        if(obj.name in _shortNames) {
          obj.shortName = _shortNames[obj.name];
        }
      }
      if(md) {
        md.update(obj.type);
        md.update(obj.value);
      }
      rval.push(obj);
    }
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificateExtensionFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionFromAsn1 (ext)](#apidoc.element.node-forge.pki.certificateExtensionFromAsn1)
- description and source-code
```javascript
certificateExtensionFromAsn1 = function (ext) {
  // an extension has:
  // [0] extnID      OBJECT IDENTIFIER
  // [1] critical    BOOLEAN DEFAULT FALSE
  // [2] extnValue   OCTET STRING
  var e = {};
  e.id = asn1.derToOid(ext.value[0].value);
  e.critical = false;
  if(ext.value[1].type === asn1.Type.BOOLEAN) {
    e.critical = (ext.value[1].value.charCodeAt(0) !== 0x00);
    e.value = ext.value[2].value;
  } else {
    e.value = ext.value[1].value;
  }
  // if the oid is known, get its name
  if(e.id in oids) {
    e.name = oids[e.id];

    // handle key usage
    if(e.name === 'keyUsage') {
      // get value as BIT STRING
      var ev = asn1.fromDer(e.value);
      var b2 = 0x00;
      var b3 = 0x00;
      if(ev.value.length > 1) {
        // skip first byte, just indicates unused bits which
        // will be padded with 0s anyway
        // get bytes with flag bits
        b2 = ev.value.charCodeAt(1);
        b3 = ev.value.length > 2 ? ev.value.charCodeAt(2) : 0;
      }
      // set flags
      e.digitalSignature = (b2 & 0x80) === 0x80;
      e.nonRepudiation = (b2 & 0x40) === 0x40;
      e.keyEncipherment = (b2 & 0x20) === 0x20;
      e.dataEncipherment = (b2 & 0x10) === 0x10;
      e.keyAgreement = (b2 & 0x08) === 0x08;
      e.keyCertSign = (b2 & 0x04) === 0x04;
      e.cRLSign = (b2 & 0x02) === 0x02;
      e.encipherOnly = (b2 & 0x01) === 0x01;
      e.decipherOnly = (b3 & 0x80) === 0x80;
    } else if(e.name === 'basicConstraints') {
      // handle basic constraints
      // get value as SEQUENCE
      var ev = asn1.fromDer(e.value);
      // get cA BOOLEAN flag (defaults to false)
      if(ev.value.length > 0 && ev.value[0].type === asn1.Type.BOOLEAN) {
        e.cA = (ev.value[0].value.charCodeAt(0) !== 0x00);
      } else {
        e.cA = false;
      }
      // get path length constraint
      var value = null;
      if(ev.value.length > 0 && ev.value[0].type === asn1.Type.INTEGER) {
        value = ev.value[0].value;
      } else if(ev.value.length > 1) {
        value = ev.value[1].value;
      }
      if(value !== null) {
        e.pathLenConstraint = asn1.derToInteger(value);
      }
    } else if(e.name === 'extKeyUsage') {
      // handle extKeyUsage
      // value is a SEQUENCE of OIDs
      var ev = asn1.fromDer(e.value);
      for(var vi = 0; vi < ev.value.length; ++vi) {
        var oid = asn1.derToOid(ev.value[vi].value);
        if(oid in oids) {
          e[oids[oid]] = true;
        } else {
          e[oid] = true;
        }
      }
    } else if(e.name === 'nsCertType') {
      // handle nsCertType
      // get value as BIT STRING
      var ev = asn1.fromDer(e.value);
      var b2 = 0x00;
      if(ev.value.length > 1) {
        // skip first byte, just indicates unused bits which
        // will be padded with 0s anyway
        // get bytes with flag bits
        b2 = ev.value.charCodeAt(1);
      }
      // set flags
      e.client = (b2 & 0x80) === 0x80;
      e.server = (b2 & 0x40) === 0x40;
      e.email = (b2 & 0x20) === 0x20;
      e.objsign = (b2 & 0x10) === 0x10;
      e.reserved = (b2 & 0x08) === 0x08;
      e.sslCA = (b2 & 0x04) === 0x04;
      e.emailCA = (b2 & 0x02) === 0x02;
      e.objCA = (b2 & 0x01) === 0x01;
    } else if(
      e.name === 'subjectAltName' ||
      e.name === 'issuerAltName') {
      // handle subjectAltName/issuerAltName
      e.altNames = [];

      // ev is a SYNTAX SEQUENCE
      var gn;
      var ev = asn1.fromDer(e.value);
      for(var n = 0; n < ev.value.length; ++n) {
        // get GeneralName
        gn = ev.value[n];

        var altName = {
          type: gn.type,
          value: gn.value
        };
        e.altNames.push(altName);

        // Note: Support for types 1,2,6,7,8
        switch(gn.type) {
        // rfc822Name
        case 1:
        // dNSName
        case 2:
        // uniformResourceIdentifier (URI)
        case 6:
          break;
        // IPAddress
        case 7:
          // convert to IPv4/IPv6 string representation
          altName.ip = forge.util.bytesToIP(gn.value);
          break;
        // registeredID
        case 8:
          altName.o ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificateExtensionToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionToAsn1 (ext)](#apidoc.element.node-forge.pki.certificateExtensionToAsn1)
- description and source-code
```javascript
certificateExtensionToAsn1 = function (ext) {
  // create a sequence for each extension
  var extseq = asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, []);

  // extnID (OID)
  extseq.value.push(asn1.create(
    asn1.Class.UNIVERSAL, asn1.Type.OID, false,
    asn1.oidToDer(ext.id).getBytes()));

  // critical defaults to false
  if(ext.critical) {
    // critical BOOLEAN DEFAULT FALSE
    extseq.value.push(asn1.create(
      asn1.Class.UNIVERSAL, asn1.Type.BOOLEAN, false,
      String.fromCharCode(0xFF)));
  }

  var value = ext.value;
  if(typeof ext.value !== 'string') {
    // value is asn.1
    value = asn1.toDer(value).getBytes();
  }

  // extnValue (OCTET STRING)
  extseq.value.push(asn1.create(
    asn1.Class.UNIVERSAL, asn1.Type.OCTETSTRING, false, value));

  return extseq;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificateExtensionsFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionsFromAsn1 (exts)](#apidoc.element.node-forge.pki.certificateExtensionsFromAsn1)
- description and source-code
```javascript
certificateExtensionsFromAsn1 = function (exts) {
  var rval = [];
  for(var i = 0; i < exts.value.length; ++i) {
    // get extension sequence
    var extseq = exts.value[i];
    for(var ei = 0; ei < extseq.value.length; ++ei) {
      rval.push(pki.certificateExtensionFromAsn1(extseq.value[ei]));
    }
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificateExtensionsToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateExtensionsToAsn1 (exts)](#apidoc.element.node-forge.pki.certificateExtensionsToAsn1)
- description and source-code
```javascript
certificateExtensionsToAsn1 = function (exts) {
  // create top-level extension container
  var rval = asn1.create(asn1.Class.CONTEXT_SPECIFIC, 3, true, []);

  // create extension sequence (stores a sequence for each extension)
  var seq = asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, []);
  rval.value.push(seq);

  for(var i = 0; i < exts.length; ++i) {
    seq.value.push(pki.certificateExtensionToAsn1(exts[i]));
  }

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificateFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateFromAsn1 (obj, computeHash)](#apidoc.element.node-forge.pki.certificateFromAsn1)
- description and source-code
```javascript
certificateFromAsn1 = function (obj, computeHash) {
  // validate certificate and capture data
  var capture = {};
  var errors = [];
  if(!asn1.validate(obj, x509CertificateValidator, capture, errors)) {
    var error = new Error('Cannot read X.509 certificate. ' +
      'ASN.1 object is not an X509v3 Certificate.');
    error.errors = errors;
    throw error;
  }

  // get oid
  var oid = asn1.derToOid(capture.publicKeyOid);
  if(oid !== pki.oids.rsaEncryption) {
    throw new Error('Cannot read public key. OID is not RSA.');
  }

  // create certificate
  var cert = pki.createCertificate();
  cert.version = capture.certVersion ?
    capture.certVersion.charCodeAt(0) : 0;
  var serial = forge.util.createBuffer(capture.certSerialNumber);
  cert.serialNumber = serial.toHex();
  cert.signatureOid = forge.asn1.derToOid(capture.certSignatureOid);
  cert.signatureParameters = _readSignatureParameters(
    cert.signatureOid, capture.certSignatureParams, true);
  cert.siginfo.algorithmOid = forge.asn1.derToOid(capture.certinfoSignatureOid);
  cert.siginfo.parameters = _readSignatureParameters(cert.siginfo.algorithmOid,
    capture.certinfoSignatureParams, false);
  cert.signature = capture.certSignature;

  var validity = [];
  if(capture.certValidity1UTCTime !== undefined) {
    validity.push(asn1.utcTimeToDate(capture.certValidity1UTCTime));
  }
  if(capture.certValidity2GeneralizedTime !== undefined) {
    validity.push(asn1.generalizedTimeToDate(
      capture.certValidity2GeneralizedTime));
  }
  if(capture.certValidity3UTCTime !== undefined) {
    validity.push(asn1.utcTimeToDate(capture.certValidity3UTCTime));
  }
  if(capture.certValidity4GeneralizedTime !== undefined) {
    validity.push(asn1.generalizedTimeToDate(
      capture.certValidity4GeneralizedTime));
  }
  if(validity.length > 2) {
    throw new Error('Cannot read notBefore/notAfter validity times; more ' +
      'than two times were provided in the certificate.');
  }
  if(validity.length < 2) {
    throw new Error('Cannot read notBefore/notAfter validity times; they ' +
      'were not provided as either UTCTime or GeneralizedTime.');
  }
  cert.validity.notBefore = validity[0];
  cert.validity.notAfter = validity[1];

  // keep TBSCertificate to preserve signature when exporting
  cert.tbsCertificate = capture.tbsCertificate;

  if(computeHash) {
    // check signature OID for supported signature types
    cert.md = null;
    if(cert.signatureOid in oids) {
      var oid = oids[cert.signatureOid];
      switch(oid) {
      case 'sha1WithRSAEncryption':
        cert.md = forge.md.sha1.create();
        break;
      case 'md5WithRSAEncryption':
        cert.md = forge.md.md5.create();
        break;
      case 'sha256WithRSAEncryption':
        cert.md = forge.md.sha256.create();
        break;
      case 'sha512WithRSAEncryption':
        cert.md = forge.md.sha512.create();
        break;
      case 'RSASSA-PSS':
        cert.md = forge.md.sha256.create();
        break;
      }
    }
    if(cert.md === null) {
      var error = new Error('Could not compute certificate digest. ' +
        'Unknown signature OID.');
      error.signatureOid = cert.signatureOid;
      throw error;
    }

    // produce DER formatted TBSCertificate and digest it
    var bytes = asn1.toDer(cert.tbsCertificate);
    cert.md.update(bytes.getBytes());
  }

  // handle issuer, build issuer message digest
  var imd = forge.md.sha1.create();
  cert.issuer.getField = function(sn) {
    return _getAttribute(cert.issuer, sn);
  };
  cert.issuer.addField = function(attr) {
    _fillMissingFields([attr]);
    cert.issuer.attributes.push(attr);
  };
  cert.issuer.attributes = pki.RDNAttributesAsArray(capture.certIssuer, imd);
  if(capture.certIssuerUniqueId) {
    cert.issuer.uniqueId = capture.certIssuerUniqueId;
  }
  cert.issuer.hash = imd.digest().toHex();

  // handle subject, build subject message digest
  var smd = forge.md.sha1.create();
  cert.subject.getField = function(sn) {
    return _getAttribute(cert.subject, sn);
  };
  cert.subject.addField = function(attr) {
    _fillMissingFields([attr]); ...
```
- example usage
```shell
...
// convert a Forge certificate to PEM
var pem = pki.certificateToPem(cert);

// convert a Forge certificate from PEM
var cert = pki.certificateFromPem(pem);

// convert an ASN.1 X.509x3 object to a Forge certificate
var cert = pki.certificateFromAsn1(obj);

// convert a Forge certificate to an ASN.1 X.509v3 object
var asn1Cert = pki.certificateToAsn1(cert);
'''

<a name="pkcs5" />
### PKCS#5
...
```

#### <a name="apidoc.element.node-forge.pki.certificateFromPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateFromPem (pem, computeHash, strict)](#apidoc.element.node-forge.pki.certificateFromPem)
- description and source-code
```javascript
certificateFromPem = function (pem, computeHash, strict) {
  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'CERTIFICATE' &&
    msg.type !== 'X509 CERTIFICATE' &&
    msg.type !== 'TRUSTED CERTIFICATE') {
    var error = new Error('Could not convert certificate from PEM; PEM header type ' +
      'is not "CERTIFICATE", "X509 CERTIFICATE", or "TRUSTED CERTIFICATE".');
    error.headerType = msg.type;
    throw error;
  }
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert certificate from PEM; PEM is encrypted.');
  }

  // convert DER to ASN.1 object
  var obj = asn1.fromDer(msg.body, strict);

  return pki.certificateFromAsn1(obj, computeHash);
}
```
- example usage
```shell
...
// self-sign certificate
cert.sign(keys.privateKey);

// convert a Forge certificate to PEM
var pem = pki.certificateToPem(cert);

// convert a Forge certificate from PEM
var cert = pki.certificateFromPem(pem);

// convert an ASN.1 X.509x3 object to a Forge certificate
var cert = pki.certificateFromAsn1(obj);

// convert a Forge certificate to an ASN.1 X.509v3 object
var asn1Cert = pki.certificateToAsn1(cert);
'''
...
```

#### <a name="apidoc.element.node-forge.pki.certificateToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateToAsn1 (cert)](#apidoc.element.node-forge.pki.certificateToAsn1)
- description and source-code
```javascript
certificateToAsn1 = function (cert) {
  // prefer cached TBSCertificate over generating one
  var tbsCertificate = cert.tbsCertificate || pki.getTBSCertificate(cert);

  // Certificate
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // TBSCertificate
    tbsCertificate,
    // AlgorithmIdentifier (signature algorithm)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      // algorithm
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(cert.signatureOid).getBytes()),
      // parameters
      _signatureParametersToAsn1(cert.signatureOid, cert.signatureParameters)
    ]),
    // SignatureValue
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false,
      String.fromCharCode(0x00) + cert.signature)
  ]);
}
```
- example usage
```shell
...
// convert a Forge certificate from PEM
var cert = pki.certificateFromPem(pem);

// convert an ASN.1 X.509x3 object to a Forge certificate
var cert = pki.certificateFromAsn1(obj);

// convert a Forge certificate to an ASN.1 X.509v3 object
var asn1Cert = pki.certificateToAsn1(cert);
'''

<a name="pkcs5" />
### PKCS#5

Provides the password-based key-derivation function from [PKCS#5][].
...
```

#### <a name="apidoc.element.node-forge.pki.certificateToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificateToPem (cert, maxline)](#apidoc.element.node-forge.pki.certificateToPem)
- description and source-code
```javascript
certificateToPem = function (cert, maxline) {
  // convert to ASN.1, then DER, then PEM-encode
  var msg = {
    type: 'CERTIFICATE',
    body: asn1.toDer(pki.certificateToAsn1(cert)).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
...
}]);
cert.setExtensions(extensions);
*/
// self-sign certificate
cert.sign(keys.privateKey);

// convert a Forge certificate to PEM
var pem = pki.certificateToPem(cert);

// convert a Forge certificate from PEM
var cert = pki.certificateFromPem(pem);

// convert an ASN.1 X.509x3 object to a Forge certificate
var cert = pki.certificateFromAsn1(obj);
...
```

#### <a name="apidoc.element.node-forge.pki.certificationRequestFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestFromAsn1 (obj, computeHash)](#apidoc.element.node-forge.pki.certificationRequestFromAsn1)
- description and source-code
```javascript
certificationRequestFromAsn1 = function (obj, computeHash) {
  // validate certification request and capture data
  var capture = {};
  var errors = [];
  if(!asn1.validate(obj, certificationRequestValidator, capture, errors)) {
    var error = new Error('Cannot read PKCS#10 certificate request. ' +
      'ASN.1 object is not a PKCS#10 CertificationRequest.');
    error.errors = errors;
    throw error;
  }

  // get oid
  var oid = asn1.derToOid(capture.publicKeyOid);
  if(oid !== pki.oids.rsaEncryption) {
    throw new Error('Cannot read public key. OID is not RSA.');
  }

  // create certification request
  var csr = pki.createCertificationRequest();
  csr.version = capture.csrVersion ? capture.csrVersion.charCodeAt(0) : 0;
  csr.signatureOid = forge.asn1.derToOid(capture.csrSignatureOid);
  csr.signatureParameters = _readSignatureParameters(
    csr.signatureOid, capture.csrSignatureParams, true);
  csr.siginfo.algorithmOid = forge.asn1.derToOid(capture.csrSignatureOid);
  csr.siginfo.parameters = _readSignatureParameters(
    csr.siginfo.algorithmOid, capture.csrSignatureParams, false);
  csr.signature = capture.csrSignature;

  // keep CertificationRequestInfo to preserve signature when exporting
  csr.certificationRequestInfo = capture.certificationRequestInfo;

  if(computeHash) {
    // check signature OID for supported signature types
    csr.md = null;
    if(csr.signatureOid in oids) {
      var oid = oids[csr.signatureOid];
      switch(oid) {
      case 'sha1WithRSAEncryption':
        csr.md = forge.md.sha1.create();
        break;
      case 'md5WithRSAEncryption':
        csr.md = forge.md.md5.create();
        break;
      case 'sha256WithRSAEncryption':
        csr.md = forge.md.sha256.create();
        break;
      case 'sha512WithRSAEncryption':
        csr.md = forge.md.sha512.create();
        break;
      case 'RSASSA-PSS':
        csr.md = forge.md.sha256.create();
        break;
      }
    }
    if(csr.md === null) {
      var error = new Error('Could not compute certification request digest. ' +
        'Unknown signature OID.');
      error.signatureOid = csr.signatureOid;
      throw error;
    }

    // produce DER formatted CertificationRequestInfo and digest it
    var bytes = asn1.toDer(csr.certificationRequestInfo);
    csr.md.update(bytes.getBytes());
  }

  // handle subject, build subject message digest
  var smd = forge.md.sha1.create();
  csr.subject.getField = function(sn) {
    return _getAttribute(csr.subject, sn);
  };
  csr.subject.addField = function(attr) {
    _fillMissingFields([attr]);
    csr.subject.attributes.push(attr);
  };
  csr.subject.attributes = pki.RDNAttributesAsArray(
    capture.certificationRequestInfoSubject, smd);
  csr.subject.hash = smd.digest().toHex();

  // convert RSA public key from ASN.1
  csr.publicKey = pki.publicKeyFromAsn1(capture.subjectPublicKeyInfo);

  // convert attributes from ASN.1
  csr.getAttribute = function(sn) {
    return _getAttribute(csr, sn);
  };
  csr.addAttribute = function(attr) {
    _fillMissingFields([attr]);
    csr.attributes.push(attr);
  };
  csr.attributes = pki.CRIAttributesAsArray(
    capture.certificationRequestInfoAttributes || []);

  return csr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificationRequestFromPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestFromPem (pem, computeHash, strict)](#apidoc.element.node-forge.pki.certificationRequestFromPem)
- description and source-code
```javascript
certificationRequestFromPem = function (pem, computeHash, strict) {
  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'CERTIFICATE REQUEST') {
    var error = new Error('Could not convert certification request from PEM; ' +
      'PEM header type is not "CERTIFICATE REQUEST".');
    error.headerType = msg.type;
    throw error;
  }
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert certification request from PEM; ' +
      'PEM is encrypted.');
  }

  // convert DER to ASN.1 object
  var obj = asn1.fromDer(msg.body, strict);

  return pki.certificationRequestFromAsn1(obj, computeHash);
}
```
- example usage
```shell
...
// verify certification request
var verified = csr.verify();

// convert certification request to PEM-format
var pem = forge.pki.certificationRequestToPem(csr);

// convert a Forge certification request from PEM-format
var csr = forge.pki.certificationRequestFromPem(pem);

// get an attribute
csr.getAttribute({name: 'challengePassword'});

// get extensions array
csr.getAttribute({name: 'extensionRequest'}).extensions;
...
```

#### <a name="apidoc.element.node-forge.pki.certificationRequestToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestToAsn1 (csr)](#apidoc.element.node-forge.pki.certificationRequestToAsn1)
- description and source-code
```javascript
certificationRequestToAsn1 = function (csr) {
  // prefer cached CertificationRequestInfo over generating one
  var cri = csr.certificationRequestInfo ||
    pki.getCertificationRequestInfo(csr);

  // Certificate
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // CertificationRequestInfo
    cri,
    // AlgorithmIdentifier (signature algorithm)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      // algorithm
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(csr.signatureOid).getBytes()),
      // parameters
      _signatureParametersToAsn1(csr.signatureOid, csr.signatureParameters)
    ]),
    // signature
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false,
      String.fromCharCode(0x00) + csr.signature)
  ]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.certificationRequestToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>certificationRequestToPem (csr, maxline)](#apidoc.element.node-forge.pki.certificationRequestToPem)
- description and source-code
```javascript
certificationRequestToPem = function (csr, maxline) {
  // convert to ASN.1, then DER, then PEM-encode
  var msg = {
    type: 'CERTIFICATE REQUEST',
    body: asn1.toDer(pki.certificationRequestToAsn1(csr)).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
...
// sign certification request
csr.sign(keys.privateKey);

// verify certification request
var verified = csr.verify();

// convert certification request to PEM-format
var pem = forge.pki.certificationRequestToPem(csr);

// convert a Forge certification request from PEM-format
var csr = forge.pki.certificationRequestFromPem(pem);

// get an attribute
csr.getAttribute({name: 'challengePassword'});
...
```

#### <a name="apidoc.element.node-forge.pki.createCaStore"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>createCaStore (certs)](#apidoc.element.node-forge.pki.createCaStore)
- description and source-code
```javascript
createCaStore = function (certs) {
  // create CA store
  var caStore = {
    // stored certificates
    certs: {}
  };

<span class="apidocCodeCommentSpan">  /**
   * Gets the certificate that issued the passed certificate or its
   * 'parent'.
   *
   * @param cert the certificate to get the parent for.
   *
   * @return the parent certificate or null if none was found.
   */
</span>  caStore.getIssuer = function(cert) {
    var rval = getBySubject(cert.issuer);

    // see if there are multiple matches
    /*if(forge.util.isArray(rval)) {
      // TODO: resolve multiple matches by checking
      // authorityKey/subjectKey/issuerUniqueID/other identifiers, etc.
      // FIXME: or alternatively do authority key mapping
      // if possible (X.509v1 certs can't work?)
      throw new Error('Resolving multiple issuer matches not implemented yet.');
    }*/

    return rval;
  };

  /**
   * Adds a trusted certificate to the store.
   *
   * @param cert the certificate to add as a trusted certificate (either a
   *          pki.certificate object or a PEM-formatted certificate).
   */
  caStore.addCertificate = function(cert) {
    // convert from pem if necessary
    if(typeof cert === 'string') {
      cert = forge.pki.certificateFromPem(cert);
    }

    ensureSubjectHasHash(cert.subject);

    if(!caStore.hasCertificate(cert)) {  // avoid duplicate certificates in store
      if(cert.subject.hash in caStore.certs) {
        // subject hash already exists, append to array
        var tmp = caStore.certs[cert.subject.hash];
        if(!forge.util.isArray(tmp)) {
          tmp = [tmp];
        }
        tmp.push(cert);
        caStore.certs[cert.subject.hash] = tmp;
      } else {
        caStore.certs[cert.subject.hash] = cert;
      }
    }
  };

  /**
   * Checks to see if the given certificate is in the store.
   *
   * @param cert the certificate to check (either a pki.certificate or a
   *          PEM-formatted certificate).
   *
   * @return true if the certificate is in the store, false if not.
   */
  caStore.hasCertificate = function(cert) {
    // convert from pem if necessary
    if(typeof cert === 'string') {
      cert = forge.pki.certificateFromPem(cert);
    }

    var match = getBySubject(cert.subject);
    if(!match) {
      return false;
    }
    if(!forge.util.isArray(match)) {
      match = [match];
    }
    // compare DER-encoding of certificates
    var der1 = asn1.toDer(pki.certificateToAsn1(cert)).getBytes();
    for(var i = 0; i < match.length; ++i) {
      var der2 = asn1.toDer(pki.certificateToAsn1(match[i])).getBytes();
      if(der1 === der2) {
        return true;
      }
    }
    return false;
  };

  /**
   * Lists all of the certificates kept in the store.
   *
   * @return an array of all of the pki.certificate objects in the store.
   */
  caStore.listAllCertificates = function() {
    var certList = [];

    for(var hash in caStore.certs) {
      if(caStore.certs.hasOwnProperty(hash)) {
        var value = caStore.certs[hash];
        if(!forge.util.isArray(value)) {
          certList.push(value);
        } else {
          for(var i = 0; i < value.length; ++i) {
            certList.push(value[i]);
          }
        }
      }
    }

    return certList;
  };

  /**
   * Removes a certificate from the store.
   *
   * @param cert the certificate to remove (either a pki.certificate or a
   *          PEM-formatted certificate).
   *
   * @return the certificate that was removed or null if the certificate
   *           wasn't in store.
   */
  caStore.removeCertificate = function(cert) {
    var result;

    // convert from pem if necessary
    if(typeof cert === 'string') {
      cert = forge.pki.certificateFromPem(cert);
    }
    ensureSubjectHasHash(cert.subject);
    if(!caStore.hasCertificate(cert)) {
      return null;
    }

    var match = getBySubject(cert.subject);

    if(!forge.util.isArray(match)) {
      result = caStore.certs[cert.subject.hash];
      delete caStore.certs[cert.subject.hash];
      return result;
    }

    // compare DER-encoding of certificates
    var der1 = asn1.toDer(pki.certificateToAsn1(cert)).getBy ...
```
- example usage
```shell
...
pki.getPublicKeyFingerprint(key, {
  md: forge.md.md5.create(),
  encoding: 'hex',
  delimiter: ':'
});

// creates a CA store
var caStore = pki.createCaStore([/* PEM-encoded cert */, ...]);

// add a certificate to the CA store
caStore.addCertificate(certObjectOrPemString);

// gets the issuer (its certificate) for the given certificate
var issuerCert = caStore.getIssuer(subjectCert);
...
```

#### <a name="apidoc.element.node-forge.pki.createCertificate"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>createCertificate ()](#apidoc.element.node-forge.pki.createCertificate)
- description and source-code
```javascript
createCertificate = function () {
  var cert = {};
  cert.version = 0x02;
  cert.serialNumber = '00';
  cert.signatureOid = null;
  cert.signature = null;
  cert.siginfo = {};
  cert.siginfo.algorithmOid = null;
  cert.validity = {};
  cert.validity.notBefore = new Date();
  cert.validity.notAfter = new Date();

  cert.issuer = {};
  cert.issuer.getField = function(sn) {
    return _getAttribute(cert.issuer, sn);
  };
  cert.issuer.addField = function(attr) {
    _fillMissingFields([attr]);
    cert.issuer.attributes.push(attr);
  };
  cert.issuer.attributes = [];
  cert.issuer.hash = null;

  cert.subject = {};
  cert.subject.getField = function(sn) {
    return _getAttribute(cert.subject, sn);
  };
  cert.subject.addField = function(attr) {
    _fillMissingFields([attr]);
    cert.subject.attributes.push(attr);
  };
  cert.subject.attributes = [];
  cert.subject.hash = null;

  cert.extensions = [];
  cert.publicKey = null;
  cert.md = null;

<span class="apidocCodeCommentSpan">  /**
   * Sets the subject of this certificate.
   *
   * @param attrs the array of subject attributes to use.
   * @param uniqueId an optional a unique ID to use.
   */
</span>  cert.setSubject = function(attrs, uniqueId) {
    // set new attributes, clear hash
    _fillMissingFields(attrs);
    cert.subject.attributes = attrs;
    delete cert.subject.uniqueId;
    if(uniqueId) {
      // TODO: support arbitrary bit length ids
      cert.subject.uniqueId = uniqueId;
    }
    cert.subject.hash = null;
  };

  /**
   * Sets the issuer of this certificate.
   *
   * @param attrs the array of issuer attributes to use.
   * @param uniqueId an optional a unique ID to use.
   */
  cert.setIssuer = function(attrs, uniqueId) {
    // set new attributes, clear hash
    _fillMissingFields(attrs);
    cert.issuer.attributes = attrs;
    delete cert.issuer.uniqueId;
    if(uniqueId) {
      // TODO: support arbitrary bit length ids
      cert.issuer.uniqueId = uniqueId;
    }
    cert.issuer.hash = null;
  };

  /**
   * Sets the extensions of this certificate.
   *
   * @param exts the array of extensions to use.
   */
  cert.setExtensions = function(exts) {
    for(var i = 0; i < exts.length; ++i) {
      _fillMissingExtensionFields(exts[i], {cert: cert});
    }
    // set new extensions
    cert.extensions = exts;
  };

  /**
   * Gets an extension by its name or id.
   *
   * @param options the name to use or an object with:
   *          name the name to use.
   *          id the id to use.
   *
   * @return the extension or null if not found.
   */
  cert.getExtension = function(options) {
    if(typeof options === 'string') {
      options = {name: options};
    }

    var rval = null;
    var ext;
    for(var i = 0; rval === null && i < cert.extensions.length; ++i) {
      ext = cert.extensions[i];
      if(options.id && ext.id === options.id) {
        rval = ext;
      } else if(options.name && ext.name === options.name) {
        rval = ext;
      }
    }
    return rval;
  };

  /**
   * Signs this certificate using the given private key.
   *
   * @param key the private key to sign with.
   * @param md the message digest object to use (defaults to forge.md.sha1).
   */
  cert.sign = function(key, md) {
    // TODO: get signature OID from private key
    cert.md = md || forge.md.sha1.create();
    var algorithmOid = oids[cert.md.algorithm + 'WithRSAEncryption'];
    if(!algorithmOid) {
      var error = new Error('Could not compute certificate digest. ' +
        'Unknown message digest algorithm OID.');
      error.algorithm = cert.md.algorithm;
      throw error;
    }
    cert.signatureOid = cert.siginfo.algorithmOid = algorithmOid;

    // get TBSCertificate, convert to DER
    cert.tbsCertificate = pki.getTBSCertificate(cert);
    var bytes = asn1.toDer(cert.tbsCertificate);

    // digest and sign
    cert.md.update(bytes.getBytes());
    cert.signature = key.sign(cert.md);
  };

  /**
   * Attempts verify the signature on the passed certificate using this
   * certificate's public key.
   *
   * @param child the certificate to verify.
   *
   * @return true if verified, false if not.
   */
  cert.v ...
```
- example usage
```shell
...
cert.sign(privateKey, forge.md.sha256.create());

// verifies an issued certificate using the certificates public key
var verified = issuer.verify(issued);

// generate a keypair and create an X.509v3 certificate
var keys = pki.rsa.generateKeyPair(2048);
var cert = pki.createCertificate();
cert.publicKey = keys.publicKey;
// alternatively set public key from a csr
//cert.publicKey = csr.publicKey;
cert.serialNumber = '01';
cert.validity.notBefore = new Date();
cert.validity.notAfter = new Date();
cert.validity.notAfter.setFullYear(cert.validity.notBefore.getFullYear() + 1);
...
```

#### <a name="apidoc.element.node-forge.pki.createCertificationRequest"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>createCertificationRequest ()](#apidoc.element.node-forge.pki.createCertificationRequest)
- description and source-code
```javascript
createCertificationRequest = function () {
  var csr = {};
  csr.version = 0x00;
  csr.signatureOid = null;
  csr.signature = null;
  csr.siginfo = {};
  csr.siginfo.algorithmOid = null;

  csr.subject = {};
  csr.subject.getField = function(sn) {
    return _getAttribute(csr.subject, sn);
  };
  csr.subject.addField = function(attr) {
    _fillMissingFields([attr]);
    csr.subject.attributes.push(attr);
  };
  csr.subject.attributes = [];
  csr.subject.hash = null;

  csr.publicKey = null;
  csr.attributes = [];
  csr.getAttribute = function(sn) {
    return _getAttribute(csr, sn);
  };
  csr.addAttribute = function(attr) {
    _fillMissingFields([attr]);
    csr.attributes.push(attr);
  };
  csr.md = null;

<span class="apidocCodeCommentSpan">  /**
   * Sets the subject of this certification request.
   *
   * @param attrs the array of subject attributes to use.
   */
</span>  csr.setSubject = function(attrs) {
    // set new attributes
    _fillMissingFields(attrs);
    csr.subject.attributes = attrs;
    csr.subject.hash = null;
  };

  /**
   * Sets the attributes of this certification request.
   *
   * @param attrs the array of attributes to use.
   */
  csr.setAttributes = function(attrs) {
    // set new attributes
    _fillMissingFields(attrs);
    csr.attributes = attrs;
  };

  /**
   * Signs this certification request using the given private key.
   *
   * @param key the private key to sign with.
   * @param md the message digest object to use (defaults to forge.md.sha1).
   */
  csr.sign = function(key, md) {
    // TODO: get signature OID from private key
    csr.md = md || forge.md.sha1.create();
    var algorithmOid = oids[csr.md.algorithm + 'WithRSAEncryption'];
    if(!algorithmOid) {
      var error = new Error('Could not compute certification request digest. ' +
        'Unknown message digest algorithm OID.');
      error.algorithm = csr.md.algorithm;
      throw error;
    }
    csr.signatureOid = csr.siginfo.algorithmOid = algorithmOid;

    // get CertificationRequestInfo, convert to DER
    csr.certificationRequestInfo = pki.getCertificationRequestInfo(csr);
    var bytes = asn1.toDer(csr.certificationRequestInfo);

    // digest and sign
    csr.md.update(bytes.getBytes());
    csr.signature = key.sign(csr.md);
  };

  /**
   * Attempts verify the signature on the passed certification request using
   * its public key.
   *
   * A CSR that has been exported to a file in PEM format can be verified using
   * OpenSSL using this command:
   *
   * openssl req -in <the-csr-pem-file> -verify -noout -text
   *
   * @return true if verified, false if not.
   */
  csr.verify = function() {
    var rval = false;

    var md = csr.md;
    if(md === null) {
      // check signature OID for supported signature types
      if(csr.signatureOid in oids) {
        // TODO: create DRY 'OID to md' function
        var oid = oids[csr.signatureOid];
        switch(oid) {
        case 'sha1WithRSAEncryption':
          md = forge.md.sha1.create();
          break;
        case 'md5WithRSAEncryption':
          md = forge.md.md5.create();
          break;
        case 'sha256WithRSAEncryption':
          md = forge.md.sha256.create();
          break;
        case 'sha512WithRSAEncryption':
          md = forge.md.sha512.create();
          break;
        case 'RSASSA-PSS':
          md = forge.md.sha256.create();
          break;
        }
      }
      if(md === null) {
        var error = new Error('Could not compute certification request digest. ' +
          'Unknown signature OID.');
        error.signatureOid = csr.signatureOid;
        throw error;
      }

      // produce DER formatted CertificationRequestInfo and digest it
      var cri = csr.certificationRequestInfo ||
        pki.getCertificationRequestInfo(csr);
      var bytes = asn1.toDer(cri);
      md.update(bytes.getBytes());
    }

    if(md !== null) {
      var scheme;

      switch(csr.signatureOid) {
      case oids.sha1WithRSAEncryption:
        /* use PKCS#1 v1.5 padding scheme */
        break;
      case oids['RSASSA-PSS']:
        var hash, mgf;

        /* initialize mgf */
        hash = oids[csr.signatur ...
```
- example usage
```shell
...
__Examples__

'''js
// generate a key pair
var keys = forge.pki.rsa.generateKeyPair(1024);

// create a certification request (CSR)
var csr = forge.pki.createCertificationRequest();
csr.publicKey = keys.publicKey;
csr.setSubject([{
name: 'commonName',
value: 'example.org'
}, {
name: 'countryName',
value: 'US'
...
```

#### <a name="apidoc.element.node-forge.pki.decryptPrivateKeyInfo"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>decryptPrivateKeyInfo (obj, password)](#apidoc.element.node-forge.pki.decryptPrivateKeyInfo)
- description and source-code
```javascript
decryptPrivateKeyInfo = function (obj, password) {
  var rval = null;

  // get PBE params
  var capture = {};
  var errors = [];
  if(!asn1.validate(obj, encryptedPrivateKeyValidator, capture, errors)) {
    var error = new Error('Cannot read encrypted private key. ' +
      'ASN.1 object is not a supported EncryptedPrivateKeyInfo.');
    error.errors = errors;
    throw error;
  }

  // get cipher
  var oid = asn1.derToOid(capture.encryptionOid);
  var cipher = pki.pbe.getCipher(oid, capture.encryptionParams, password);

  // get encrypted data
  var encrypted = forge.util.createBuffer(capture.encryptedData);

  cipher.update(encrypted);
  if(cipher.finish()) {
    rval = asn1.fromDer(cipher.output);
  }

  return rval;
}
```
- example usage
```shell
...
// encrypts a PrivateKeyInfo and outputs an EncryptedPrivateKeyInfo
var encryptedPrivateKeyInfo = pki.encryptPrivateKeyInfo(
  privateKeyInfo, 'password', {
    algorithm: 'aes256', // 'aes128', 'aes192', 'aes256', '3des'
  });

// decrypts an ASN.1 EncryptedPrivateKeyInfo
var privateKeyInfo = pki.decryptPrivateKeyInfo(
  encryptedPrivateKeyInfo, 'password');

// converts an EncryptedPrivateKeyInfo to PEM
var pem = pki.encryptedPrivateKeyToPem(encryptedPrivateKeyInfo);

// converts a PEM-encoded EncryptedPrivateKeyInfo to ASN.1 format
var encryptedPrivateKeyInfo = pki.encryptedPrivateKeyFromPem(pem);
...
```

#### <a name="apidoc.element.node-forge.pki.decryptRsaPrivateKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>decryptRsaPrivateKey (pem, password)](#apidoc.element.node-forge.pki.decryptRsaPrivateKey)
- description and source-code
```javascript
decryptRsaPrivateKey = function (pem, password) {
  var rval = null;

  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'ENCRYPTED PRIVATE KEY' &&
    msg.type !== 'PRIVATE KEY' &&
    msg.type !== 'RSA PRIVATE KEY') {
    var error = new Error('Could not convert private key from PEM; PEM header type ' +
      'is not "ENCRYPTED PRIVATE KEY", "PRIVATE KEY", or "RSA PRIVATE KEY".');
    error.headerType = error;
    throw error;
  }

  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    var dkLen;
    var cipherFn;
    switch(msg.dekInfo.algorithm) {
    case 'DES-CBC':
      dkLen = 8;
      cipherFn = forge.des.createDecryptionCipher;
      break;
    case 'DES-EDE3-CBC':
      dkLen = 24;
      cipherFn = forge.des.createDecryptionCipher;
      break;
    case 'AES-128-CBC':
      dkLen = 16;
      cipherFn = forge.aes.createDecryptionCipher;
      break;
    case 'AES-192-CBC':
      dkLen = 24;
      cipherFn = forge.aes.createDecryptionCipher;
      break;
    case 'AES-256-CBC':
      dkLen = 32;
      cipherFn = forge.aes.createDecryptionCipher;
      break;
    case 'RC2-40-CBC':
      dkLen = 5;
      cipherFn = function(key) {
        return forge.rc2.createDecryptionCipher(key, 40);
      };
      break;
    case 'RC2-64-CBC':
      dkLen = 8;
      cipherFn = function(key) {
        return forge.rc2.createDecryptionCipher(key, 64);
      };
      break;
    case 'RC2-128-CBC':
      dkLen = 16;
      cipherFn = function(key) {
        return forge.rc2.createDecryptionCipher(key, 128);
      };
      break;
    default:
      var error = new Error('Could not decrypt private key; unsupported ' +
        'encryption algorithm "' + msg.dekInfo.algorithm + '".');
      error.algorithm = msg.dekInfo.algorithm;
      throw error;
    }

    // use OpenSSL legacy key derivation
    var iv = forge.util.hexToBytes(msg.dekInfo.parameters);
    var dk = forge.pbe.opensslDeriveBytes(password, iv.substr(0, 8), dkLen);
    var cipher = cipherFn(dk);
    cipher.start(iv);
    cipher.update(forge.util.createBuffer(msg.body));
    if(cipher.finish()) {
      rval = cipher.output.getBytes();
    } else {
      return rval;
    }
  } else {
    rval = msg.body;
  }

  if(msg.type === 'ENCRYPTED PRIVATE KEY') {
    rval = pki.decryptPrivateKeyInfo(asn1.fromDer(rval), password);
  } else {
    // decryption already performed above
    rval = asn1.fromDer(rval);
  }

  if(rval !== null) {
    rval = pki.privateKeyFromAsn1(rval);
  }

  return rval;
}
```
- example usage
```shell
...
var pem = pki.encryptRsaPrivateKey(privateKey, 'password');

// encrypts a Forge private key and outputs it in PEM format using OpenSSL's
// proprietary legacy format + encapsulated PEM headers (DEK-Info)
var pem = pki.encryptRsaPrivateKey(privateKey, 'password', {legacy: true});

// decrypts a PEM-formatted, encrypted private key
var privateKey = pki.decryptRsaPrivateKey(pem, 'password');

// sets an RSA public key from a private key
var publicKey = pki.setRsaPublicKey(privateKey.n, privateKey.e);
'''

<a name="pkcs10" />
### PKCS#10
...
```

#### <a name="apidoc.element.node-forge.pki.distinguishedNameToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>distinguishedNameToAsn1 (dn)](#apidoc.element.node-forge.pki.distinguishedNameToAsn1)
- description and source-code
```javascript
distinguishedNameToAsn1 = function (dn) {
  return _dnToAsn1(dn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.encryptPrivateKeyInfo"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptPrivateKeyInfo (obj, password, options)](#apidoc.element.node-forge.pki.encryptPrivateKeyInfo)
- description and source-code
```javascript
encryptPrivateKeyInfo = function (obj, password, options) {
  // set default options
  options = options || {};
  options.saltSize = options.saltSize || 8;
  options.count = options.count || 2048;
  options.algorithm = options.algorithm || 'aes128';
  options.prfAlgorithm = options.prfAlgorithm || 'sha1';

  // generate PBE params
  var salt = forge.random.getBytesSync(options.saltSize);
  var count = options.count;
  var countBytes = asn1.integerToDer(count);
  var dkLen;
  var encryptionAlgorithm;
  var encryptedData;
  if(options.algorithm.indexOf('aes') === 0 || options.algorithm === 'des') {
    // do PBES2
    var ivLen, encOid, cipherFn;
    switch(options.algorithm) {
    case 'aes128':
      dkLen = 16;
      ivLen = 16;
      encOid = oids['aes128-CBC'];
      cipherFn = forge.aes.createEncryptionCipher;
      break;
    case 'aes192':
      dkLen = 24;
      ivLen = 16;
      encOid = oids['aes192-CBC'];
      cipherFn = forge.aes.createEncryptionCipher;
      break;
    case 'aes256':
      dkLen = 32;
      ivLen = 16;
      encOid = oids['aes256-CBC'];
      cipherFn = forge.aes.createEncryptionCipher;
      break;
    case 'des':
      dkLen = 8;
      ivLen = 8;
      encOid = oids['desCBC'];
      cipherFn = forge.des.createEncryptionCipher;
      break;
    default:
      var error = new Error('Cannot encrypt private key. Unknown encryption algorithm.');
      error.algorithm = options.algorithm;
      throw error;
    }

    // get PRF message digest
    var prfAlgorithm = 'hmacWith' + options.prfAlgorithm.toUpperCase();
    var md = prfAlgorithmToMessageDigest(prfAlgorithm);

    // encrypt private key using pbe SHA-1 and AES/DES
    var dk = forge.pkcs5.pbkdf2(password, salt, count, dkLen, md);
    var iv = forge.random.getBytesSync(ivLen);
    var cipher = cipherFn(dk);
    cipher.start(iv);
    cipher.update(asn1.toDer(obj));
    cipher.finish();
    encryptedData = cipher.output.getBytes();

    // get PBKDF2-params
    var params = createPbkdf2Params(salt, countBytes, dkLen, prfAlgorithm);

    encryptionAlgorithm = asn1.create(
      asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(oids['pkcs5PBES2']).getBytes()),
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
        // keyDerivationFunc
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
            asn1.oidToDer(oids['pkcs5PBKDF2']).getBytes()),
          // PBKDF2-params
          params
        ]),
        // encryptionScheme
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
          asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
            asn1.oidToDer(encOid).getBytes()),
          // iv
          asn1.create(
            asn1.Class.UNIVERSAL, asn1.Type.OCTETSTRING, false, iv)
        ])
      ])
    ]);
  } else if(options.algorithm === '3des') {
    // Do PKCS12 PBE
    dkLen = 24;

    var saltBytes = new forge.util.ByteBuffer(salt);
    var dk = pki.pbe.generatePkcs12Key(password, saltBytes, 1, count, dkLen);
    var iv = pki.pbe.generatePkcs12Key(password, saltBytes, 2, count, dkLen);
    var cipher = forge.des.createEncryptionCipher(dk);
    cipher.start(iv);
    cipher.update(asn1.toDer(obj));
    cipher.finish();
    encryptedData = cipher.output.getBytes();

    encryptionAlgorithm = asn1.create(
      asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(oids['pbeWithSHAAnd3-KeyTripleDES-CBC']).getBytes()),
      // pkcs-12PbeParams
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
        // salt
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OCTETSTRING, false, salt),
        // iteration count
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
          countBytes.getBytes())
      ])
    ]);
  } else {
    var error = new Error('Cannot encrypt private key. Unknown encryption algorithm.');
    error.algorithm = op ...
```
- example usage
```shell
...
// wrap an RSAPrivateKey ASN.1 object in a PKCS#8 ASN.1 PrivateKeyInfo
var privateKeyInfo = pki.wrapRsaPrivateKey(rsaPrivateKey);

// convert a PKCS#8 ASN.1 PrivateKeyInfo to PEM
var pem = pki.privateKeyInfoToPem(privateKeyInfo);

// encrypts a PrivateKeyInfo and outputs an EncryptedPrivateKeyInfo
var encryptedPrivateKeyInfo = pki.encryptPrivateKeyInfo(
privateKeyInfo, 'password', {
  algorithm: 'aes256', // 'aes128', 'aes192', 'aes256', '3des'
});

// decrypts an ASN.1 EncryptedPrivateKeyInfo
var privateKeyInfo = pki.decryptPrivateKeyInfo(
encryptedPrivateKeyInfo, 'password');
...
```

#### <a name="apidoc.element.node-forge.pki.encryptRsaPrivateKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptRsaPrivateKey (rsaKey, password, options)](#apidoc.element.node-forge.pki.encryptRsaPrivateKey)
- description and source-code
```javascript
encryptRsaPrivateKey = function (rsaKey, password, options) {
  // standard PKCS#8
  options = options || {};
  if(!options.legacy) {
    // encrypt PrivateKeyInfo
    var rval = pki.wrapRsaPrivateKey(pki.privateKeyToAsn1(rsaKey));
    rval = pki.encryptPrivateKeyInfo(rval, password, options);
    return pki.encryptedPrivateKeyToPem(rval);
  }

  // legacy non-PKCS#8
  var algorithm;
  var iv;
  var dkLen;
  var cipherFn;
  switch(options.algorithm) {
  case 'aes128':
    algorithm = 'AES-128-CBC';
    dkLen = 16;
    iv = forge.random.getBytesSync(16);
    cipherFn = forge.aes.createEncryptionCipher;
    break;
  case 'aes192':
    algorithm = 'AES-192-CBC';
    dkLen = 24;
    iv = forge.random.getBytesSync(16);
    cipherFn = forge.aes.createEncryptionCipher;
    break;
  case 'aes256':
    algorithm = 'AES-256-CBC';
    dkLen = 32;
    iv = forge.random.getBytesSync(16);
    cipherFn = forge.aes.createEncryptionCipher;
    break;
  case '3des':
    algorithm = 'DES-EDE3-CBC';
    dkLen = 24;
    iv = forge.random.getBytesSync(8);
    cipherFn = forge.des.createEncryptionCipher;
    break;
  case 'des':
    algorithm = 'DES-CBC';
    dkLen = 8;
    iv = forge.random.getBytesSync(8);
    cipherFn = forge.des.createEncryptionCipher;
    break;
  default:
    var error = new Error('Could not encrypt RSA private key; unsupported ' +
      'encryption algorithm "' + options.algorithm + '".');
    error.algorithm = options.algorithm;
    throw error;
  }

  // encrypt private key using OpenSSL legacy key derivation
  var dk = forge.pbe.opensslDeriveBytes(password, iv.substr(0, 8), dkLen);
  var cipher = cipherFn(dk);
  cipher.start(iv);
  cipher.update(asn1.toDer(pki.privateKeyToAsn1(rsaKey)));
  cipher.finish();

  var msg = {
    type: 'RSA PRIVATE KEY',
    procType: {
      version: '4',
      type: 'ENCRYPTED'
    },
    dekInfo: {
      algorithm: algorithm,
      parameters: forge.util.bytesToHex(iv).toUpperCase()
    },
    body: cipher.output.getBytes()
  };
  return forge.pem.encode(msg);
}
```
- example usage
```shell
...
// converts an EncryptedPrivateKeyInfo to PEM
var pem = pki.encryptedPrivateKeyToPem(encryptedPrivateKeyInfo);

// converts a PEM-encoded EncryptedPrivateKeyInfo to ASN.1 format
var encryptedPrivateKeyInfo = pki.encryptedPrivateKeyFromPem(pem);

// wraps and encrypts a Forge private key and outputs it in PEM format
var pem = pki.encryptRsaPrivateKey(privateKey, 'password');

// encrypts a Forge private key and outputs it in PEM format using OpenSSL's
// proprietary legacy format + encapsulated PEM headers (DEK-Info)
var pem = pki.encryptRsaPrivateKey(privateKey, 'password', {legacy: true});

// decrypts a PEM-formatted, encrypted private key
var privateKey = pki.decryptRsaPrivateKey(pem, 'password');
...
```

#### <a name="apidoc.element.node-forge.pki.encryptedPrivateKeyFromPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptedPrivateKeyFromPem (pem)](#apidoc.element.node-forge.pki.encryptedPrivateKeyFromPem)
- description and source-code
```javascript
encryptedPrivateKeyFromPem = function (pem) {
  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'ENCRYPTED PRIVATE KEY') {
    var error = new Error('Could not convert encrypted private key from PEM; ' +
      'PEM header type is "ENCRYPTED PRIVATE KEY".');
    error.headerType = msg.type;
    throw error;
  }
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert encrypted private key from PEM; ' +
      'PEM is encrypted.');
  }

  // convert DER to ASN.1 object
  return asn1.fromDer(msg.body);
}
```
- example usage
```shell
...
var privateKeyInfo = pki.decryptPrivateKeyInfo(
  encryptedPrivateKeyInfo, 'password');

// converts an EncryptedPrivateKeyInfo to PEM
var pem = pki.encryptedPrivateKeyToPem(encryptedPrivateKeyInfo);

// converts a PEM-encoded EncryptedPrivateKeyInfo to ASN.1 format
var encryptedPrivateKeyInfo = pki.encryptedPrivateKeyFromPem(pem);

// wraps and encrypts a Forge private key and outputs it in PEM format
var pem = pki.encryptRsaPrivateKey(privateKey, 'password');

// encrypts a Forge private key and outputs it in PEM format using OpenSSL's
// proprietary legacy format + encapsulated PEM headers (DEK-Info)
var pem = pki.encryptRsaPrivateKey(privateKey, 'password', {legacy: true});
...
```

#### <a name="apidoc.element.node-forge.pki.encryptedPrivateKeyToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>encryptedPrivateKeyToPem (epki, maxline)](#apidoc.element.node-forge.pki.encryptedPrivateKeyToPem)
- description and source-code
```javascript
encryptedPrivateKeyToPem = function (epki, maxline) {
  // convert to DER, then PEM-encode
  var msg = {
    type: 'ENCRYPTED PRIVATE KEY',
    body: asn1.toDer(epki).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
...
  });

// decrypts an ASN.1 EncryptedPrivateKeyInfo
var privateKeyInfo = pki.decryptPrivateKeyInfo(
  encryptedPrivateKeyInfo, 'password');

// converts an EncryptedPrivateKeyInfo to PEM
var pem = pki.encryptedPrivateKeyToPem(encryptedPrivateKeyInfo);

// converts a PEM-encoded EncryptedPrivateKeyInfo to ASN.1 format
var encryptedPrivateKeyInfo = pki.encryptedPrivateKeyFromPem(pem);

// wraps and encrypts a Forge private key and outputs it in PEM format
var pem = pki.encryptRsaPrivateKey(privateKey, 'password');
...
```

#### <a name="apidoc.element.node-forge.pki.getCertificationRequestInfo"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>getCertificationRequestInfo (csr)](#apidoc.element.node-forge.pki.getCertificationRequestInfo)
- description and source-code
```javascript
getCertificationRequestInfo = function (csr) {
  // CertificationRequestInfo
  var cri = asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // version
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      asn1.integerToDer(csr.version).getBytes()),
    // subject
    _dnToAsn1(csr.subject),
    // SubjectPublicKeyInfo
    pki.publicKeyToAsn1(csr.publicKey),
    // attributes
    _CRIAttributesToAsn1(csr)
  ]);

  return cri;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.getPublicKeyFingerprint"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>getPublicKeyFingerprint (key, options)](#apidoc.element.node-forge.pki.getPublicKeyFingerprint)
- description and source-code
```javascript
getPublicKeyFingerprint = function (key, options) {
  options = options || {};
  var md = options.md || forge.md.sha1.create();
  var type = options.type || 'RSAPublicKey';

  var bytes;
  switch(type) {
  case 'RSAPublicKey':
    bytes = asn1.toDer(pki.publicKeyToRSAPublicKey(key)).getBytes();
    break;
  case 'SubjectPublicKeyInfo':
    bytes = asn1.toDer(pki.publicKeyToAsn1(key)).getBytes();
    break;
  default:
    throw new Error('Unknown fingerprint type "' + options.type + '".');
  }

  // hash public key bytes
  md.start();
  md.update(bytes);
  var digest = md.digest();
  if(options.encoding === 'hex') {
    var hex = digest.toHex();
    if(options.delimiter) {
      return hex.match(/.{2}/g).join(options.delimiter);
    }
    return hex;
  } else if(options.encoding === 'binary') {
    return digest.getBytes();
  } else if(options.encoding) {
    throw new Error('Unknown encoding "' + options.encoding + '".');
  }
  return digest;
}
```
- example usage
```shell
...
// encodes a public RSA key as an OpenSSH file
forge.ssh.publicKeyToOpenSSH(key, comment);

// encodes a private RSA key as an OpenSSH file
forge.ssh.privateKeyToOpenSSH(privateKey, passphrase);

// gets the SSH public key fingerprint in a byte buffer
forge.ssh.getPublicKeyFingerprint(key);

// gets a hex-encoded, colon-delimited SSH public key fingerprint
forge.ssh.getPublicKeyFingerprint(key, {encoding: 'hex', delimiter: ':'});
'''

<a name="xhr" />
### XHR
...
```

#### <a name="apidoc.element.node-forge.pki.getTBSCertificate"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>getTBSCertificate (cert)](#apidoc.element.node-forge.pki.getTBSCertificate)
- description and source-code
```javascript
getTBSCertificate = function (cert) {
  // TBSCertificate
  var tbs = asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // version
    asn1.create(asn1.Class.CONTEXT_SPECIFIC, 0, true, [
      // integer
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
        asn1.integerToDer(cert.version).getBytes())
    ]),
    // serialNumber
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      forge.util.hexToBytes(cert.serialNumber)),
    // signature
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      // algorithm
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(cert.siginfo.algorithmOid).getBytes()),
      // parameters
      _signatureParametersToAsn1(
        cert.siginfo.algorithmOid, cert.siginfo.parameters)
    ]),
    // issuer
    _dnToAsn1(cert.issuer),
    // validity
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      // notBefore
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.UTCTIME, false,
        asn1.dateToUtcTime(cert.validity.notBefore)),
      // notAfter
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.UTCTIME, false,
        asn1.dateToUtcTime(cert.validity.notAfter))
    ]),
    // subject
    _dnToAsn1(cert.subject),
    // SubjectPublicKeyInfo
    pki.publicKeyToAsn1(cert.publicKey)
  ]);

  if(cert.issuer.uniqueId) {
    // issuerUniqueID (optional)
    tbs.value.push(
      asn1.create(asn1.Class.CONTEXT_SPECIFIC, 1, true, [
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false,
          // TODO: support arbitrary bit length ids
          String.fromCharCode(0x00) +
          cert.issuer.uniqueId
        )
      ])
    );
  }
  if(cert.subject.uniqueId) {
    // subjectUniqueID (optional)
    tbs.value.push(
      asn1.create(asn1.Class.CONTEXT_SPECIFIC, 2, true, [
        asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false,
          // TODO: support arbitrary bit length ids
          String.fromCharCode(0x00) +
          cert.subject.uniqueId
        )
      ])
    );
  }

  if(cert.extensions.length > 0) {
    // extensions (optional)
    tbs.value.push(pki.certificateExtensionsToAsn1(cert.extensions));
  }

  return tbs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.pemToDer"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>pemToDer (pem)](#apidoc.element.node-forge.pki.pemToDer)
- description and source-code
```javascript
pemToDer = function (pem) {
  var msg = forge.pem.decode(pem)[0];
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert PEM to DER; PEM is encrypted.');
  }
  return forge.util.createBuffer(msg.body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.privateKeyFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyFromAsn1 (obj)](#apidoc.element.node-forge.pki.privateKeyFromAsn1)
- description and source-code
```javascript
privateKeyFromAsn1 = function (obj) {
  // get PrivateKeyInfo
  var capture = {};
  var errors = [];
  if(asn1.validate(obj, privateKeyValidator, capture, errors)) {
    obj = asn1.fromDer(forge.util.createBuffer(capture.privateKey));
  }

  // get RSAPrivateKey
  capture = {};
  errors = [];
  if(!asn1.validate(obj, rsaPrivateKeyValidator, capture, errors)) {
    var error = new Error('Cannot read private key. ' +
      'ASN.1 object does not contain an RSAPrivateKey.');
    error.errors = errors;
    throw error;
  }

  // Note: Version is currently ignored.
  // capture.privateKeyVersion
  // FIXME: inefficient, get a BigInteger that uses byte strings
  var n, e, d, p, q, dP, dQ, qInv;
  n = forge.util.createBuffer(capture.privateKeyModulus).toHex();
  e = forge.util.createBuffer(capture.privateKeyPublicExponent).toHex();
  d = forge.util.createBuffer(capture.privateKeyPrivateExponent).toHex();
  p = forge.util.createBuffer(capture.privateKeyPrime1).toHex();
  q = forge.util.createBuffer(capture.privateKeyPrime2).toHex();
  dP = forge.util.createBuffer(capture.privateKeyExponent1).toHex();
  dQ = forge.util.createBuffer(capture.privateKeyExponent2).toHex();
  qInv = forge.util.createBuffer(capture.privateKeyCoefficient).toHex();

  // set private key
  return pki.setRsaPrivateKey(
    new BigInteger(n, 16),
    new BigInteger(e, 16),
    new BigInteger(d, 16),
    new BigInteger(p, 16),
    new BigInteger(q, 16),
    new BigInteger(dP, 16),
    new BigInteger(dQ, 16),
    new BigInteger(qInv, 16));
}
```
- example usage
```shell
...
// convert a PEM-formatted private key to a Forge private key
var privateKey = pki.privateKeyFromPem(pem);

// convert a Forge private key to PEM-format
var pem = pki.privateKeyToPem(privateKey);

// convert an ASN.1 PrivateKeyInfo or RSAPrivateKey to a Forge private key
var privateKey = pki.privateKeyFromAsn1(rsaPrivateKey);

// convert a Forge private key to an ASN.1 RSAPrivateKey
var rsaPrivateKey = pki.privateKeyToAsn1(privateKey);

// wrap an RSAPrivateKey ASN.1 object in a PKCS#8 ASN.1 PrivateKeyInfo
var privateKeyInfo = pki.wrapRsaPrivateKey(rsaPrivateKey);
...
```

#### <a name="apidoc.element.node-forge.pki.privateKeyFromPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyFromPem (pem)](#apidoc.element.node-forge.pki.privateKeyFromPem)
- description and source-code
```javascript
privateKeyFromPem = function (pem) {
  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'PRIVATE KEY' && msg.type !== 'RSA PRIVATE KEY') {
    var error = new Error('Could not convert private key from PEM; PEM ' +
      'header type is not "PRIVATE KEY" or "RSA PRIVATE KEY".');
    error.headerType = msg.type;
    throw error;
  }
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert private key from PEM; PEM is encrypted.');
  }

  // convert DER to ASN.1 object
  var obj = asn1.fromDer(msg.body);

  return pki.privateKeyFromAsn1(obj);
}
```
- example usage
```shell
...

__Examples__

'''js
var pki = forge.pki;

// convert a PEM-formatted private key to a Forge private key
var privateKey = pki.privateKeyFromPem(pem);

// convert a Forge private key to PEM-format
var pem = pki.privateKeyToPem(privateKey);

// convert an ASN.1 PrivateKeyInfo or RSAPrivateKey to a Forge private key
var privateKey = pki.privateKeyFromAsn1(rsaPrivateKey);
...
```

#### <a name="apidoc.element.node-forge.pki.privateKeyInfoToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyInfoToPem (pki, maxline)](#apidoc.element.node-forge.pki.privateKeyInfoToPem)
- description and source-code
```javascript
privateKeyInfoToPem = function (pki, maxline) {
  // convert to DER, then PEM-encode
  var msg = {
    type: 'PRIVATE KEY',
    body: asn1.toDer(pki).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
...
// convert a Forge private key to an ASN.1 RSAPrivateKey
var rsaPrivateKey = pki.privateKeyToAsn1(privateKey);

// wrap an RSAPrivateKey ASN.1 object in a PKCS#8 ASN.1 PrivateKeyInfo
var privateKeyInfo = pki.wrapRsaPrivateKey(rsaPrivateKey);

// convert a PKCS#8 ASN.1 PrivateKeyInfo to PEM
var pem = pki.privateKeyInfoToPem(privateKeyInfo);

// encrypts a PrivateKeyInfo and outputs an EncryptedPrivateKeyInfo
var encryptedPrivateKeyInfo = pki.encryptPrivateKeyInfo(
privateKeyInfo, 'password', {
  algorithm: 'aes256', // 'aes128', 'aes192', 'aes256', '3des'
});
...
```

#### <a name="apidoc.element.node-forge.pki.privateKeyToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyToAsn1 (key)](#apidoc.element.node-forge.pki.privateKeyToAsn1)
- description and source-code
```javascript
privateKeyToAsn1 = function (key) {
  // RSAPrivateKey
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // version (0 = only 2 primes, 1 multiple primes)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      asn1.integerToDer(0).getBytes()),
    // modulus (n)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.n)),
    // publicExponent (e)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.e)),
    // privateExponent (d)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.d)),
    // privateKeyPrime1 (p)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.p)),
    // privateKeyPrime2 (q)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.q)),
    // privateKeyExponent1 (dP)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.dP)),
    // privateKeyExponent2 (dQ)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.dQ)),
    // coefficient (qInv)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.qInv))
  ]);
}
```
- example usage
```shell
...
// convert a Forge private key to PEM-format
var pem = pki.privateKeyToPem(privateKey);

// convert an ASN.1 PrivateKeyInfo or RSAPrivateKey to a Forge private key
var privateKey = pki.privateKeyFromAsn1(rsaPrivateKey);

// convert a Forge private key to an ASN.1 RSAPrivateKey
var rsaPrivateKey = pki.privateKeyToAsn1(privateKey);

// wrap an RSAPrivateKey ASN.1 object in a PKCS#8 ASN.1 PrivateKeyInfo
var privateKeyInfo = pki.wrapRsaPrivateKey(rsaPrivateKey);

// convert a PKCS#8 ASN.1 PrivateKeyInfo to PEM
var pem = pki.privateKeyInfoToPem(privateKeyInfo);
...
```

#### <a name="apidoc.element.node-forge.pki.privateKeyToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyToPem (key, maxline)](#apidoc.element.node-forge.pki.privateKeyToPem)
- description and source-code
```javascript
privateKeyToPem = function (key, maxline) {
  // convert to ASN.1, then DER, then PEM-encode
  var msg = {
    type: 'RSA PRIVATE KEY',
    body: asn1.toDer(pki.privateKeyToAsn1(key)).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
...
'''js
var pki = forge.pki;

// convert a PEM-formatted private key to a Forge private key
var privateKey = pki.privateKeyFromPem(pem);

// convert a Forge private key to PEM-format
var pem = pki.privateKeyToPem(privateKey);

// convert an ASN.1 PrivateKeyInfo or RSAPrivateKey to a Forge private key
var privateKey = pki.privateKeyFromAsn1(rsaPrivateKey);

// convert a Forge private key to an ASN.1 RSAPrivateKey
var rsaPrivateKey = pki.privateKeyToAsn1(privateKey);
...
```

#### <a name="apidoc.element.node-forge.pki.privateKeyToRSAPrivateKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>privateKeyToRSAPrivateKey (key)](#apidoc.element.node-forge.pki.privateKeyToRSAPrivateKey)
- description and source-code
```javascript
privateKeyToRSAPrivateKey = function (key) {
  // RSAPrivateKey
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // version (0 = only 2 primes, 1 multiple primes)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      asn1.integerToDer(0).getBytes()),
    // modulus (n)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.n)),
    // publicExponent (e)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.e)),
    // privateExponent (d)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.d)),
    // privateKeyPrime1 (p)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.p)),
    // privateKeyPrime2 (q)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.q)),
    // privateKeyExponent1 (dP)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.dP)),
    // privateKeyExponent2 (dQ)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.dQ)),
    // coefficient (qInv)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.qInv))
  ]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.publicKeyFromAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyFromAsn1 (obj)](#apidoc.element.node-forge.pki.publicKeyFromAsn1)
- description and source-code
```javascript
publicKeyFromAsn1 = function (obj) {
  // get SubjectPublicKeyInfo
  var capture = {};
  var errors = [];
  if(asn1.validate(obj, publicKeyValidator, capture, errors)) {
    // get oid
    var oid = asn1.derToOid(capture.publicKeyOid);
    if(oid !== pki.oids.rsaEncryption) {
      var error = new Error('Cannot read public key. Unknown OID.');
      error.oid = oid;
      throw error;
    }
    obj = capture.rsaPublicKey;
  }

  // get RSA params
  errors = [];
  if(!asn1.validate(obj, rsaPublicKeyValidator, capture, errors)) {
    var error = new Error('Cannot read public key. ' +
      'ASN.1 object does not contain an RSAPublicKey.');
    error.errors = errors;
    throw error;
  }

  // FIXME: inefficient, get a BigInteger that uses byte strings
  var n = forge.util.createBuffer(capture.publicKeyModulus).toHex();
  var e = forge.util.createBuffer(capture.publicKeyExponent).toHex();

  // set public key
  return pki.setRsaPublicKey(
    new BigInteger(n, 16),
    new BigInteger(e, 16));
}
```
- example usage
```shell
...
// convert a PEM-formatted public key to a Forge public key
var publicKey = pki.publicKeyFromPem(pem);

// convert a Forge public key to PEM-format
var pem = pki.publicKeyToPem(publicKey);

// convert an ASN.1 SubjectPublicKeyInfo to a Forge public key
var publicKey = pki.publicKeyFromAsn1(subjectPublicKeyInfo);

// convert a Forge public key to an ASN.1 SubjectPublicKeyInfo
var subjectPublicKeyInfo = pki.publicKeyToAsn1(publicKey);

// gets a SHA-1 RSAPublicKey fingerprint a byte buffer
pki.getPublicKeyFingerprint(key);
...
```

#### <a name="apidoc.element.node-forge.pki.publicKeyFromPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyFromPem (pem)](#apidoc.element.node-forge.pki.publicKeyFromPem)
- description and source-code
```javascript
publicKeyFromPem = function (pem) {
  var msg = forge.pem.decode(pem)[0];

  if(msg.type !== 'PUBLIC KEY' && msg.type !== 'RSA PUBLIC KEY') {
    var error = new Error('Could not convert public key from PEM; PEM header ' +
      'type is not "PUBLIC KEY" or "RSA PUBLIC KEY".');
    error.headerType = msg.type;
    throw error;
  }
  if(msg.procType && msg.procType.type === 'ENCRYPTED') {
    throw new Error('Could not convert public key from PEM; PEM is encrypted.');
  }

  // convert DER to ASN.1 object
  var obj = asn1.fromDer(msg.body);

  return pki.publicKeyFromAsn1(obj);
}
```
- example usage
```shell
...

__Examples__

'''js
var pki = forge.pki;

// convert a PEM-formatted public key to a Forge public key
var publicKey = pki.publicKeyFromPem(pem);

// convert a Forge public key to PEM-format
var pem = pki.publicKeyToPem(publicKey);

// convert an ASN.1 SubjectPublicKeyInfo to a Forge public key
var publicKey = pki.publicKeyFromAsn1(subjectPublicKeyInfo);
...
```

#### <a name="apidoc.element.node-forge.pki.publicKeyToAsn1"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToAsn1 (key)](#apidoc.element.node-forge.pki.publicKeyToAsn1)
- description and source-code
```javascript
publicKeyToAsn1 = function (key) {
  // SubjectPublicKeyInfo
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // AlgorithmIdentifier
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      // algorithm
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(pki.oids.rsaEncryption).getBytes()),
      // parameters (null)
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.NULL, false, '')
    ]),
    // subjectPublicKey
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false, [
      pki.publicKeyToRSAPublicKey(key)
    ])
  ]);
}
```
- example usage
```shell
...
// convert a Forge public key to PEM-format
var pem = pki.publicKeyToPem(publicKey);

// convert an ASN.1 SubjectPublicKeyInfo to a Forge public key
var publicKey = pki.publicKeyFromAsn1(subjectPublicKeyInfo);

// convert a Forge public key to an ASN.1 SubjectPublicKeyInfo
var subjectPublicKeyInfo = pki.publicKeyToAsn1(publicKey);

// gets a SHA-1 RSAPublicKey fingerprint a byte buffer
pki.getPublicKeyFingerprint(key);

// gets a SHA-1 SubjectPublicKeyInfo fingerprint a byte buffer
pki.getPublicKeyFingerprint(key, {type: 'SubjectPublicKeyInfo'});
...
```

#### <a name="apidoc.element.node-forge.pki.publicKeyToPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToPem (key, maxline)](#apidoc.element.node-forge.pki.publicKeyToPem)
- description and source-code
```javascript
publicKeyToPem = function (key, maxline) {
  // convert to ASN.1, then DER, then PEM-encode
  var msg = {
    type: 'PUBLIC KEY',
    body: asn1.toDer(pki.publicKeyToAsn1(key)).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
...
'''js
var pki = forge.pki;

// convert a PEM-formatted public key to a Forge public key
var publicKey = pki.publicKeyFromPem(pem);

// convert a Forge public key to PEM-format
var pem = pki.publicKeyToPem(publicKey);

// convert an ASN.1 SubjectPublicKeyInfo to a Forge public key
var publicKey = pki.publicKeyFromAsn1(subjectPublicKeyInfo);

// convert a Forge public key to an ASN.1 SubjectPublicKeyInfo
var subjectPublicKeyInfo = pki.publicKeyToAsn1(publicKey);
...
```

#### <a name="apidoc.element.node-forge.pki.publicKeyToRSAPublicKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToRSAPublicKey (key)](#apidoc.element.node-forge.pki.publicKeyToRSAPublicKey)
- description and source-code
```javascript
publicKeyToRSAPublicKey = function (key) {
  // RSAPublicKey
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // modulus (n)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.n)),
    // publicExponent (e)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      _bnToBytes(key.e))
  ]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.publicKeyToRSAPublicKeyPem"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToRSAPublicKeyPem (key, maxline)](#apidoc.element.node-forge.pki.publicKeyToRSAPublicKeyPem)
- description and source-code
```javascript
publicKeyToRSAPublicKeyPem = function (key, maxline) {
  // convert to ASN.1, then DER, then PEM-encode
  var msg = {
    type: 'RSA PUBLIC KEY',
    body: asn1.toDer(pki.publicKeyToRSAPublicKey(key)).getBytes()
  };
  return forge.pem.encode(msg, {maxline: maxline});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.publicKeyToSubjectPublicKeyInfo"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>publicKeyToSubjectPublicKeyInfo (key)](#apidoc.element.node-forge.pki.publicKeyToSubjectPublicKeyInfo)
- description and source-code
```javascript
publicKeyToSubjectPublicKeyInfo = function (key) {
  // SubjectPublicKeyInfo
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // AlgorithmIdentifier
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      // algorithm
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(pki.oids.rsaEncryption).getBytes()),
      // parameters (null)
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.NULL, false, '')
    ]),
    // subjectPublicKey
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.BITSTRING, false, [
      pki.publicKeyToRSAPublicKey(key)
    ])
  ]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.setRsaPrivateKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>setRsaPrivateKey ( n, e, d, p, q, dP, dQ, qInv)](#apidoc.element.node-forge.pki.setRsaPrivateKey)
- description and source-code
```javascript
setRsaPrivateKey = function ( n, e, d, p, q, dP, dQ, qInv) {
  var key = {
    n: n,
    e: e,
    d: d,
    p: p,
    q: q,
    dP: dP,
    dQ: dQ,
    qInv: qInv
  };

<span class="apidocCodeCommentSpan">  /**
   * Decrypts the given data with this private key. The decryption scheme
   * must match the one used to encrypt the data.
   *
   * @param data the byte string to decrypt.
   * @param scheme the decryption scheme to use:
   *          'RSAES-PKCS1-V1_5' (default),
   *          'RSA-OAEP',
   *          'RAW', 'NONE', or null to perform raw RSA decryption.
   * @param schemeOptions any scheme-specific options.
   *
   * @return the decrypted byte string.
   */
</span>  key.decrypt = function(data, scheme, schemeOptions) {
    if(typeof scheme === 'string') {
      scheme = scheme.toUpperCase();
    } else if(scheme === undefined) {
      scheme = 'RSAES-PKCS1-V1_5';
    }

    // do rsa decryption w/o any decoding
    var d = pki.rsa.decrypt(data, key, false, false);

    if(scheme === 'RSAES-PKCS1-V1_5') {
      scheme = { decode: _decodePkcs1_v1_5 };
    } else if(scheme === 'RSA-OAEP' || scheme === 'RSAES-OAEP') {
      scheme = {
        decode: function(d, key) {
          return forge.pkcs1.decode_rsa_oaep(key, d, schemeOptions);
        }
      };
    } else if(['RAW', 'NONE', 'NULL', null].indexOf(scheme) !== -1) {
      scheme = { decode: function(d) { return d; } };
    } else {
      throw new Error('Unsupported encryption scheme: "' + scheme + '".');
    }

    // decode according to scheme
    return scheme.decode(d, key, false);
  };

  /**
   * Signs the given digest, producing a signature.
   *
   * PKCS#1 supports multiple (currently two) signature schemes:
   * RSASSA-PKCS1-V1_5 and RSASSA-PSS.
   *
   * By default this implementation uses the "old scheme", i.e.
   * RSASSA-PKCS1-V1_5. In order to generate a PSS signature, provide
   * an instance of Forge PSS object as the scheme parameter.
   *
   * @param md the message digest object with the hash to sign.
   * @param scheme the signature scheme to use:
   *          'RSASSA-PKCS1-V1_5' or undefined for RSASSA PKCS#1 v1.5,
   *          a Forge PSS object for RSASSA-PSS,
   *          'NONE' or null for none, DigestInfo will not be used but
   *            PKCS#1 v1.5 padding will still be used.
   *
   * @return the signature as a byte string.
   */
  key.sign = function(md, scheme) {
    /* Note: The internal implementation of RSA operations is being
      transitioned away from a PKCS#1 v1.5 hard-coded scheme. Some legacy
      code like the use of an encoding block identifier 'bt' will eventually
      be removed. */

    // private key operation
    var bt = false;

    if(typeof scheme === 'string') {
      scheme = scheme.toUpperCase();
    }

    if(scheme === undefined || scheme === 'RSASSA-PKCS1-V1_5') {
      scheme = { encode: emsaPkcs1v15encode };
      bt = 0x01;
    } else if(scheme === 'NONE' || scheme === 'NULL' || scheme === null) {
      scheme = { encode: function() { return md; } };
      bt = 0x01;
    }

    // encode and then encrypt
    var d = scheme.encode(md, key.n.bitLength());
    return pki.rsa.encrypt(d, key, bt);
  };

  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.pki.setRsaPublicKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>setRsaPublicKey (n, e)](#apidoc.element.node-forge.pki.setRsaPublicKey)
- description and source-code
```javascript
setRsaPublicKey = function (n, e) {
  var key = {
    n: n,
    e: e
  };

<span class="apidocCodeCommentSpan">  /**
   * Encrypts the given data with this public key. Newer applications
   * should use the 'RSA-OAEP' decryption scheme, 'RSAES-PKCS1-V1_5' is for
   * legacy applications.
   *
   * @param data the byte string to encrypt.
   * @param scheme the encryption scheme to use:
   *          'RSAES-PKCS1-V1_5' (default),
   *          'RSA-OAEP',
   *          'RAW', 'NONE', or null to perform raw RSA encryption,
   *          an object with an 'encode' property set to a function
   *          with the signature 'function(data, key)' that returns
   *          a binary-encoded string representing the encoded data.
   * @param schemeOptions any scheme-specific options.
   *
   * @return the encrypted byte string.
   */
</span>  key.encrypt = function(data, scheme, schemeOptions) {
    if(typeof scheme === 'string') {
      scheme = scheme.toUpperCase();
    } else if(scheme === undefined) {
      scheme = 'RSAES-PKCS1-V1_5';
    }

    if(scheme === 'RSAES-PKCS1-V1_5') {
      scheme = {
        encode: function(m, key, pub) {
          return _encodePkcs1_v1_5(m, key, 0x02).getBytes();
        }
      };
    } else if(scheme === 'RSA-OAEP' || scheme === 'RSAES-OAEP') {
      scheme = {
        encode: function(m, key) {
          return forge.pkcs1.encode_rsa_oaep(key, m, schemeOptions);
        }
      };
    } else if(['RAW', 'NONE', 'NULL', null].indexOf(scheme) !== -1) {
      scheme = { encode: function(e) { return e; } };
    } else if(typeof scheme === 'string') {
      throw new Error('Unsupported encryption scheme: "' + scheme + '".');
    }

    // do scheme-based encoding then rsa encryption
    var e = scheme.encode(data, key, true);
    return pki.rsa.encrypt(e, key, true);
  };

  /**
   * Verifies the given signature against the given digest.
   *
   * PKCS#1 supports multiple (currently two) signature schemes:
   * RSASSA-PKCS1-V1_5 and RSASSA-PSS.
   *
   * By default this implementation uses the "old scheme", i.e.
   * RSASSA-PKCS1-V1_5, in which case once RSA-decrypted, the
   * signature is an OCTET STRING that holds a DigestInfo.
   *
   * DigestInfo ::= SEQUENCE {
   *   digestAlgorithm DigestAlgorithmIdentifier,
   *   digest Digest
   * }
   * DigestAlgorithmIdentifier ::= AlgorithmIdentifier
   * Digest ::= OCTET STRING
   *
   * To perform PSS signature verification, provide an instance
   * of Forge PSS object as the scheme parameter.
   *
   * @param digest the message digest hash to compare against the signature,
   *          as a binary-encoded string.
   * @param signature the signature to verify, as a binary-encoded string.
   * @param scheme signature verification scheme to use:
   *          'RSASSA-PKCS1-V1_5' or undefined for RSASSA PKCS#1 v1.5,
   *          a Forge PSS object for RSASSA-PSS,
   *          'NONE' or null for none, DigestInfo will not be expected, but
   *            PKCS#1 v1.5 padding will still be used.
   *
   * @return true if the signature was verified, false if not.
   */
   key.verify = function(digest, signature, scheme) {
     if(typeof scheme === 'string') {
       scheme = scheme.toUpperCase();
     } else if(scheme === undefined) {
       scheme = 'RSASSA-PKCS1-V1_5';
     }

     if(scheme === 'RSASSA-PKCS1-V1_5') {
       scheme = {
         verify: function(digest, d) {
           // remove padding
           d = _decodePkcs1_v1_5(d, key, true);
           // d is ASN.1 BER-encoded DigestInfo
           var obj = asn1.fromDer(d);
           // compare the given digest to the decrypted one
           return digest === obj.value[1].value;
         }
       };
     } else if(scheme === 'NONE' || scheme === 'NULL' || scheme === null) {
       scheme = {
         verify: function(digest, d) {
           // remove padding
           d = _decodePkcs1_v1_5(d, key, true);
           return digest === d;
         }
       };
     }

     // do rsa decryption w/o any decoding, then verify -- which does decoding
     var d = pki.rsa.decrypt(signature, key, true, false);
     return scheme.verify(digest, d, key.n.bitL ...
```
- example usage
```shell
...
// proprietary legacy format + encapsulated PEM headers (DEK-Info)
var pem = pki.encryptRsaPrivateKey(privateKey, 'password', {legacy: true});

// decrypts a PEM-formatted, encrypted private key
var privateKey = pki.decryptRsaPrivateKey(pem, 'password');

// sets an RSA public key from a private key
var publicKey = pki.setRsaPublicKey(privateKey.n, privateKey.e);
'''

<a name="pkcs10" />
### PKCS#10

Provides certification requests or certificate signing requests (CSR) from
[PKCS#10][].
...
```

#### <a name="apidoc.element.node-forge.pki.verifyCertificateChain"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>verifyCertificateChain (caStore, chain, verify)](#apidoc.element.node-forge.pki.verifyCertificateChain)
- description and source-code
```javascript
verifyCertificateChain = function (caStore, chain, verify) {
  /* From: RFC3280 - Internet X.509 Public Key Infrastructure Certificate
    Section 6: Certification Path Validation
    See inline parentheticals related to this particular implementation.

    The primary goal of path validation is to verify the binding between
    a subject distinguished name or a subject alternative name and subject
    public key, as represented in the end entity certificate, based on the
    public key of the trust anchor. This requires obtaining a sequence of
    certificates that support that binding. That sequence should be provided
    in the passed 'chain'. The trust anchor should be in the given CA
    store. The 'end entity' certificate is the certificate provided by the
    end point (typically a server) and is the first in the chain.

    To meet this goal, the path validation process verifies, among other
    things, that a prospective certification path (a sequence of n
    certificates or a 'chain') satisfies the following conditions:

    (a) for all x in {1, ..., n-1}, the subject of certificate x is
          the issuer of certificate x+1;

    (b) certificate 1 is issued by the trust anchor;

    (c) certificate n is the certificate to be validated; and

    (d) for all x in {1, ..., n}, the certificate was valid at the
          time in question.

    Note that here 'n' is index 0 in the chain and 1 is the last certificate
    in the chain and it must be signed by a certificate in the connection's
    CA store.

    The path validation process also determines the set of certificate
    policies that are valid for this path, based on the certificate policies
    extension, policy mapping extension, policy constraints extension, and
    inhibit any-policy extension.

    Note: Policy mapping extension not supported (Not Required).

    Note: If the certificate has an unsupported critical extension, then it
    must be rejected.

    Note: A certificate is self-issued if the DNs that appear in the subject
    and issuer fields are identical and are not empty.

    The path validation algorithm assumes the following seven inputs are
    provided to the path processing logic. What this specific implementation
    will use is provided parenthetically:

    (a) a prospective certification path of length n (the 'chain')
    (b) the current date/time: ('now').
    (c) user-initial-policy-set: A set of certificate policy identifiers
          naming the policies that are acceptable to the certificate user.
          The user-initial-policy-set contains the special value any-policy
          if the user is not concerned about certificate policy
          (Not implemented. Any policy is accepted).
    (d) trust anchor information, describing a CA that serves as a trust
          anchor for the certification path. The trust anchor information
          includes:

      (1)  the trusted issuer name,
      (2)  the trusted public key algorithm,
      (3)  the trusted public key, and
      (4)  optionally, the trusted public key parameters associated
             with the public key.

      (Trust anchors are provided via certificates in the CA store).

      The trust anchor information may be provided to the path processing
      procedure in the form of a self-signed certificate. The trusted anchor
      information is trusted because it was delivered to the path processing
      procedure by some trustworthy out-of-band procedure. If the trusted
      public key algorithm requires parameters, then the parameters are
      provided along with the trusted public key (No parameters used in this
      implementation).

    (e) initial-policy-mapping-inhibit, which indicates if policy mapping is
          allowed in the certification path.
          (Not implemented, no policy checking)

    (f) initial-explicit-policy, which indicates if the path must be valid
          for at least one of the certificate policies in the user-initial-
          policy-set.
          (Not implemented, no policy checking)

    (g) initial-any-policy-inhibit, which indicates whet ...
```
- example usage
```shell
...
// add a certificate to the CA store
caStore.addCertificate(certObjectOrPemString);

// gets the issuer (its certificate) for the given certificate
var issuerCert = caStore.getIssuer(subjectCert);

// verifies a certificate chain against a CA store
pki.verifyCertificateChain(caStore, chain, customVerifyCallback);

// signs a certificate using the given private key
cert.sign(privateKey);

// signs a certificate using SHA-256 instead of SHA-1
cert.sign(privateKey, forge.md.sha256.create());
...
```

#### <a name="apidoc.element.node-forge.pki.wrapRsaPrivateKey"></a>[function <span class="apidocSignatureSpan">node-forge.pki.</span>wrapRsaPrivateKey (rsaKey)](#apidoc.element.node-forge.pki.wrapRsaPrivateKey)
- description and source-code
```javascript
wrapRsaPrivateKey = function (rsaKey) {
  // PrivateKeyInfo
  return asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
    // version (0)
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.INTEGER, false,
      asn1.integerToDer(0).getBytes()),
    // privateKeyAlgorithm
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.SEQUENCE, true, [
      asn1.create(
        asn1.Class.UNIVERSAL, asn1.Type.OID, false,
        asn1.oidToDer(pki.oids.rsaEncryption).getBytes()),
      asn1.create(asn1.Class.UNIVERSAL, asn1.Type.NULL, false, '')
    ]),
    // PrivateKey
    asn1.create(asn1.Class.UNIVERSAL, asn1.Type.OCTETSTRING, false,
      asn1.toDer(rsaKey).getBytes())
    ]);
}
```
- example usage
```shell
...
// convert an ASN.1 PrivateKeyInfo or RSAPrivateKey to a Forge private key
var privateKey = pki.privateKeyFromAsn1(rsaPrivateKey);

// convert a Forge private key to an ASN.1 RSAPrivateKey
var rsaPrivateKey = pki.privateKeyToAsn1(privateKey);

// wrap an RSAPrivateKey ASN.1 object in a PKCS#8 ASN.1 PrivateKeyInfo
var privateKeyInfo = pki.wrapRsaPrivateKey(rsaPrivateKey);

// convert a PKCS#8 ASN.1 PrivateKeyInfo to PEM
var pem = pki.privateKeyInfoToPem(privateKeyInfo);

// encrypts a PrivateKeyInfo and outputs an EncryptedPrivateKeyInfo
var encryptedPrivateKeyInfo = pki.encryptPrivateKeyInfo(
privateKeyInfo, 'password', {
...
```



# <a name="apidoc.module.node-forge.prime"></a>[module node-forge.prime](#apidoc.module.node-forge.prime)

#### <a name="apidoc.element.node-forge.prime.generateProbablePrime"></a>[function <span class="apidocSignatureSpan">node-forge.prime.</span>generateProbablePrime (bits, options, callback)](#apidoc.element.node-forge.prime.generateProbablePrime)
- description and source-code
```javascript
generateProbablePrime = function (bits, options, callback) {
  if(typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};

  // default to PRIMEINC algorithm
  var algorithm = options.algorithm || 'PRIMEINC';
  if(typeof algorithm === 'string') {
    algorithm = {name: algorithm};
  }
  algorithm.options = algorithm.options || {};

  // create prng with api that matches BigInteger secure random
  var prng = options.prng || forge.random;
  var rng = {
    // x is an array to fill with bytes
    nextBytes: function(x) {
      var b = prng.getBytesSync(x.length);
      for(var i = 0; i < x.length; ++i) {
        x[i] = b.charCodeAt(i);
      }
    }
  };

  if(algorithm.name === 'PRIMEINC') {
    return primeincFindPrime(bits, rng, algorithm.options, callback);
  }

  throw new Error('Invalid prime generation algorithm: ' + algorithm.name);
}
```
- example usage
```shell
...
Provides an API for generating large, random, probable primes.

__Examples__

'''js
// generate a random prime on the main JS thread
var bits = 1024;
forge.prime.generateProbablePrime(bits, function(err, num) {
  console.log('random prime', num.toString(16));
});

// generate a random prime using Web Workers (if available, otherwise
// falls back to the main thread)
var bits = 1024;
var options = {
...
```



# <a name="apidoc.module.node-forge.prng"></a>[module node-forge.prng](#apidoc.module.node-forge.prng)

#### <a name="apidoc.element.node-forge.prng.create"></a>[function <span class="apidocSignatureSpan">node-forge.prng.</span>create (plugin)](#apidoc.element.node-forge.prng.create)
- description and source-code
```javascript
create = function (plugin) {
  var ctx = {
    plugin: plugin,
    key: null,
    seed: null,
    time: null,
    // number of reseeds so far
    reseeds: 0,
    // amount of data generated so far
    generated: 0
  };

  // create 32 entropy pools (each is a message digest)
  var md = plugin.md;
  var pools = new Array(32);
  for(var i = 0; i < 32; ++i) {
    pools[i] = md.create();
  }
  ctx.pools = pools;

  // entropy pools are written to cyclically, starting at index 0
  ctx.pool = 0;

<span class="apidocCodeCommentSpan">  /**
   * Generates random bytes. The bytes may be generated synchronously or
   * asynchronously. Web workers must use the asynchronous interface or
   * else the behavior is undefined.
   *
   * @param count the number of random bytes to generate.
   * @param [callback(err, bytes)] called once the operation completes.
   *
   * @return count random bytes as a string.
   */
</span>  ctx.generate = function(count, callback) {
    // do synchronously
    if(!callback) {
      return ctx.generateSync(count);
    }

    // simple generator using counter-based CBC
    var cipher = ctx.plugin.cipher;
    var increment = ctx.plugin.increment;
    var formatKey = ctx.plugin.formatKey;
    var formatSeed = ctx.plugin.formatSeed;
    var b = forge.util.createBuffer();

    // reset key for every request
    ctx.key = null;

    generate();

    function generate(err) {
      if(err) {
        return callback(err);
      }

      // sufficient bytes generated
      if(b.length() >= count) {
        return callback(null, b.getBytes(count));
      }

      // if amount of data generated is greater than 1 MiB, trigger reseed
      if(ctx.generated > 0xfffff) {
        ctx.key = null;
      }

      if(ctx.key === null) {
        // prevent stack overflow
        return forge.util.nextTick(function() {
          _reseed(generate);
        });
      }

      // generate the random bytes
      var bytes = cipher(ctx.key, ctx.seed);
      ctx.generated += bytes.length;
      b.putBytes(bytes);

      // generate bytes for a new key and seed
      ctx.key = formatKey(cipher(ctx.key, increment(ctx.seed)));
      ctx.seed = formatSeed(cipher(ctx.key, ctx.seed));

      forge.util.setImmediate(generate);
    }
  };

  /**
   * Generates random bytes synchronously.
   *
   * @param count the number of random bytes to generate.
   *
   * @return count random bytes as a string.
   */
  ctx.generateSync = function(count) {
    // simple generator using counter-based CBC
    var cipher = ctx.plugin.cipher;
    var increment = ctx.plugin.increment;
    var formatKey = ctx.plugin.formatKey;
    var formatSeed = ctx.plugin.formatSeed;

    // reset key for every request
    ctx.key = null;

    var b = forge.util.createBuffer();
    while(b.length() < count) {
      // if amount of data generated is greater than 1 MiB, trigger reseed
      if(ctx.generated > 0xfffff) {
        ctx.key = null;
      }

      if(ctx.key === null) {
        _reseedSync();
      }

      // generate the random bytes
      var bytes = cipher(ctx.key, ctx.seed);
      ctx.generated += bytes.length;
      b.putBytes(bytes);

      // generate bytes for a new key and seed
      ctx.key = formatKey(cipher(ctx.key, increment(ctx.seed)));
      ctx.seed = formatSeed(cipher(ctx.key, ctx.seed));
    }

    return b.getBytes(count);
  };

  /**
   * Private function that asynchronously reseeds a generator.
   *
   * @param callback(err) called once the operation completes.
   */
  function _reseed(callback) {
    if(ctx.pools[0].messageLength >= 32) {
      _seed();
      return callback();
    }
    // not enough seed data...
    var needed = (32 - ctx.pools[0].messageLength) << 5;
    ctx.seedFile(needed, function(err, bytes) {
      if(err) {
        return callback(err);
      }
      ctx.collect(bytes);
      _seed();
      callback();
    });
  }

  /**
   * Private function that synchronously reseeds a generator.
   */
  function _reseedSync() {
    if(ctx.pools[0].messageLength >= 32) {
      return _seed();
    }
    // not enough seed data...
    var needed = (32 - ctx.pools[0].messageLength) << 5; ...
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.pss"></a>[module node-forge.pss](#apidoc.module.node-forge.pss)

#### <a name="apidoc.element.node-forge.pss.create"></a>[function <span class="apidocSignatureSpan">node-forge.pss.</span>create (options)](#apidoc.element.node-forge.pss.create)
- description and source-code
```javascript
create = function (options) {
  // backwards compatibility w/legacy args: hash, mgf, sLen
  if(arguments.length === 3) {
    options = {
      md: arguments[0],
      mgf: arguments[1],
      saltLength: arguments[2]
    };
  }

  var hash = options.md;
  var mgf = options.mgf;
  var hLen = hash.digestLength;

  var salt_ = options.salt || null;
  if(typeof salt_ === 'string') {
    // assume binary-encoded string
    salt_ = forge.util.createBuffer(salt_);
  }

  var sLen;
  if('saltLength' in options) {
    sLen = options.saltLength;
  } else if(salt_ !== null) {
    sLen = salt_.length();
  } else {
    throw new Error('Salt length not specified or specific salt not given.');
  }

  if(salt_ !== null && salt_.length() !== sLen) {
    throw new Error('Given salt length does not match length of given salt.');
  }

  var prng = options.prng || forge.random;

  var pssobj = {};

<span class="apidocCodeCommentSpan">  /**
   * Encodes a PSS signature.
   *
   * This function implements EMSA-PSS-ENCODE as per RFC 3447, section 9.1.1.
   *
   * @param md the message digest object with the hash to sign.
   * @param modsBits the length of the RSA modulus in bits.
   *
   * @return the encoded message as a binary-encoded string of length
   *           ceil((modBits - 1) / 8).
   */
</span>  pssobj.encode = function(md, modBits) {
    var i;
    var emBits = modBits - 1;
    var emLen = Math.ceil(emBits / 8);

    /* 2. Let mHash = Hash(M), an octet string of length hLen. */
    var mHash = md.digest().getBytes();

    /* 3. If emLen < hLen + sLen + 2, output "encoding error" and stop. */
    if(emLen < hLen + sLen + 2) {
      throw new Error('Message is too long to encrypt.');
    }

    /* 4. Generate a random octet string salt of length sLen; if sLen = 0,
     *    then salt is the empty string. */
    var salt;
    if(salt_ === null) {
      salt = prng.getBytesSync(sLen);
    } else {
      salt = salt_.bytes();
    }

    /* 5. Let M' = (0x)00 00 00 00 00 00 00 00 || mHash || salt; */
    var m_ = new forge.util.ByteBuffer();
    m_.fillWithByte(0, 8);
    m_.putBytes(mHash);
    m_.putBytes(salt);

    /* 6. Let H = Hash(M'), an octet string of length hLen. */
    hash.start();
    hash.update(m_.getBytes());
    var h = hash.digest().getBytes();

    /* 7. Generate an octet string PS consisting of emLen - sLen - hLen - 2
     *    zero octets.  The length of PS may be 0. */
    var ps = new forge.util.ByteBuffer();
    ps.fillWithByte(0, emLen - sLen - hLen - 2);

    /* 8. Let DB = PS || 0x01 || salt; DB is an octet string of length
     *    emLen - hLen - 1. */
    ps.putByte(0x01);
    ps.putBytes(salt);
    var db = ps.getBytes();

    /* 9. Let dbMask = MGF(H, emLen - hLen - 1). */
    var maskLen = emLen - hLen - 1;
    var dbMask = mgf.generate(h, maskLen);

    /* 10. Let maskedDB = DB \xor dbMask. */
    var maskedDB = '';
    for(i = 0; i < maskLen; i++) {
      maskedDB += String.fromCharCode(db.charCodeAt(i) ^ dbMask.charCodeAt(i));
    }

    /* 11. Set the leftmost 8emLen - emBits bits of the leftmost octet in
     *     maskedDB to zero. */
    var mask = (0xFF00 >> (8 * emLen - emBits)) & 0xFF;
    maskedDB = String.fromCharCode(maskedDB.charCodeAt(0) & ~mask) +
      maskedDB.substr(1);

    /* 12. Let EM = maskedDB || H || 0xbc.
     * 13. Output EM. */
    return maskedDB + h + String.fromCharCode(0xbc);
  };

  /**
   * Verifies a PSS signature.
   *
   * This function implements EMSA-PSS-VERIFY as per RFC 3447, section 9.1.2.
   *
   * @param mHash the message digest hash, as a binary-encoded string, to
   *         compare against the signature.
   * @param em the encoded message, as a binary-encoded string
   *          (RSA decryption result).
   * @param modsBits the length of the RSA modulus in bits.
   *
   * @return true if the signature was verified, false if not.
   */
  pssobj.verify = function(mHash, em, modBits) {
    var i;
    var emBits = modBits - 1;
    var emLen = Math.ceil(emBits / 8);

    /* c. Convert the message representative m to an encoded message EM
     *    of length emLen = ceil((modBits - 1) / 8) octets, where modBits ...
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.random"></a>[module node-forge.random](#apidoc.module.node-forge.random)

#### <a name="apidoc.element.node-forge.random.collect"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>collect (bytes)](#apidoc.element.node-forge.random.collect)
- description and source-code
```javascript
collect = function (bytes) {
  // iterate over pools distributing entropy cyclically
  var count = bytes.length;
  for(var i = 0; i < count; ++i) {
    ctx.pools[ctx.pool].update(bytes.substr(i, 1));
    ctx.pool = (ctx.pool === 31) ? 0 : ctx.pool + 1;
  }
}
```
- example usage
```shell
...

// get some random bytes asynchronously
forge.random.getBytes(32, function(err, bytes) {
  console.log(forge.util.bytesToHex(bytes));
});

// collect some entropy if you'd like
forge.random.collect(someRandomBytes);
jQuery().mousemove(function(e) {
  forge.random.collectInt(e.clientX, 16);
  forge.random.collectInt(e.clientY, 16);
});

// specify a seed file for use with the synchronous API if you'd like
forge.random.seedFileSync = function(needed) {
...
```

#### <a name="apidoc.element.node-forge.random.collectInt"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>collectInt (i, n)](#apidoc.element.node-forge.random.collectInt)
- description and source-code
```javascript
collectInt = function (i, n) {
  var bytes = '';
  for(var x = 0; x < n; x += 8) {
    bytes += String.fromCharCode((i >> x) & 0xFF);
  }
  ctx.collect(bytes);
}
```
- example usage
```shell
...
forge.random.getBytes(32, function(err, bytes) {
console.log(forge.util.bytesToHex(bytes));
});

// collect some entropy if you'd like
forge.random.collect(someRandomBytes);
jQuery().mousemove(function(e) {
forge.random.collectInt(e.clientX, 16);
forge.random.collectInt(e.clientY, 16);
});

// specify a seed file for use with the synchronous API if you'd like
forge.random.seedFileSync = function(needed) {
// get 'needed' number of random bytes from somewhere
return fetchedRandomBytes;
...
```

#### <a name="apidoc.element.node-forge.random.createInstance"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>createInstance ()](#apidoc.element.node-forge.random.createInstance)
- description and source-code
```javascript
function spawnPrng() {
  var ctx = forge.prng.create(prng_aes);

<span class="apidocCodeCommentSpan">  /**
   * Gets random bytes. If a native secure crypto API is unavailable, this
   * method tries to make the bytes more unpredictable by drawing from data that
   * can be collected from the user of the browser, eg: mouse movement.
   *
   * If a callback is given, this method will be called asynchronously.
   *
   * @param count the number of random bytes to get.
   * @param [callback(err, bytes)] called once the operation completes.
   *
   * @return the random bytes in a string.
   */
</span>  ctx.getBytes = function(count, callback) {
    return ctx.generate(count, callback);
  };

  /**
   * Gets random bytes asynchronously. If a native secure crypto API is
   * unavailable, this method tries to make the bytes more unpredictable by
   * drawing from data that can be collected from the user of the browser,
   * eg: mouse movement.
   *
   * @param count the number of random bytes to get.
   *
   * @return the random bytes in a string.
   */
  ctx.getBytesSync = function(count) {
    return ctx.generate(count);
  };

  return ctx;
}
```
- example usage
```shell
...
});

// register the main thread to send entropy or a Web Worker to receive
// entropy on demand from the main thread
forge.random.registerWorker(self);

// generate a new instance of a PRNG with no collected entropy
var myPrng = forge.random.createInstance();
'''

<a name="task" />
### Tasks

Provides queuing and synchronizing tasks in a web application.
...
```

#### <a name="apidoc.element.node-forge.random.generate"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>generate (count, callback)](#apidoc.element.node-forge.random.generate)
- description and source-code
```javascript
generate = function (count, callback) {
  // do synchronously
  if(!callback) {
    return ctx.generateSync(count);
  }

  // simple generator using counter-based CBC
  var cipher = ctx.plugin.cipher;
  var increment = ctx.plugin.increment;
  var formatKey = ctx.plugin.formatKey;
  var formatSeed = ctx.plugin.formatSeed;
  var b = forge.util.createBuffer();

  // reset key for every request
  ctx.key = null;

  generate();

  function generate(err) {
    if(err) {
      return callback(err);
    }

    // sufficient bytes generated
    if(b.length() >= count) {
      return callback(null, b.getBytes(count));
    }

    // if amount of data generated is greater than 1 MiB, trigger reseed
    if(ctx.generated > 0xfffff) {
      ctx.key = null;
    }

    if(ctx.key === null) {
      // prevent stack overflow
      return forge.util.nextTick(function() {
        _reseed(generate);
      });
    }

    // generate the random bytes
    var bytes = cipher(ctx.key, ctx.seed);
    ctx.generated += bytes.length;
    b.putBytes(bytes);

    // generate bytes for a new key and seed
    ctx.key = formatKey(cipher(ctx.key, increment(ctx.seed)));
    ctx.seed = formatSeed(cipher(ctx.key, ctx.seed));

    forge.util.setImmediate(generate);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.random.generateSync"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>generateSync (count)](#apidoc.element.node-forge.random.generateSync)
- description and source-code
```javascript
generateSync = function (count) {
  // simple generator using counter-based CBC
  var cipher = ctx.plugin.cipher;
  var increment = ctx.plugin.increment;
  var formatKey = ctx.plugin.formatKey;
  var formatSeed = ctx.plugin.formatSeed;

  // reset key for every request
  ctx.key = null;

  var b = forge.util.createBuffer();
  while(b.length() < count) {
    // if amount of data generated is greater than 1 MiB, trigger reseed
    if(ctx.generated > 0xfffff) {
      ctx.key = null;
    }

    if(ctx.key === null) {
      _reseedSync();
    }

    // generate the random bytes
    var bytes = cipher(ctx.key, ctx.seed);
    ctx.generated += bytes.length;
    b.putBytes(bytes);

    // generate bytes for a new key and seed
    ctx.key = formatKey(cipher(ctx.key, increment(ctx.seed)));
    ctx.seed = formatSeed(cipher(ctx.key, ctx.seed));
  }

  return b.getBytes(count);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.random.getBytes"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>getBytes (count, callback)](#apidoc.element.node-forge.random.getBytes)
- description and source-code
```javascript
getBytes = function (count, callback) {
  return ctx.generate(count, callback);
}
```
- example usage
```shell
...
},
/* the private key for the client-side cert if provided */
getPrivateKey: function(connection, cert) {
  return myClientPrivateKey;
},
tlsDataReady: function(connection) {
  // TLS data (encrypted) is ready to be sent to the server
  sendToServerSomehow(connection.tlsData.getBytes());
  // if you were communicating with the server below, you'd do:
  // server.process(connection.tlsData.getBytes());
},
dataReady: function(connection) {
  // clear data from the server is ready
  console.log('the server sent: ' +
    forge.util.decodeUtf8(connection.data.getBytes()));
...
```

#### <a name="apidoc.element.node-forge.random.getBytesSync"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>getBytesSync (count)](#apidoc.element.node-forge.random.getBytesSync)
- description and source-code
```javascript
getBytesSync = function (count) {
  return ctx.generate(count);
}
```
- example usage
```shell
...
[DES][] is used. Use a [3DES][] algorithm to enforce Triple-DES.

__Examples__

'''js
// generate a random key and IV
// Note: a key size of 16 bytes will use AES-128, 24 => AES-192, 32 => AES-256
var key = forge.random.getBytesSync(16);
var iv = forge.random.getBytesSync(16);

/* alternatively, generate a password-based 16-byte key
var salt = forge.random.getBytesSync(128);
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/
...
```

#### <a name="apidoc.element.node-forge.random.registerWorker"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>registerWorker (worker)](#apidoc.element.node-forge.random.registerWorker)
- description and source-code
```javascript
registerWorker = function (worker) {
  // worker receives random bytes
  if(worker === self) {
    ctx.seedFile = function(needed, callback) {
      function listener(e) {
        var data = e.data;
        if(data.forge && data.forge.prng) {
          self.removeEventListener('message', listener);
          callback(data.forge.prng.err, data.forge.prng.bytes);
        }
      }
      self.addEventListener('message', listener);
      self.postMessage({forge: {prng: {needed: needed}}});
    };
  } else {
    // main thread sends random bytes upon request
    var listener = function(e) {
      var data = e.data;
      if(data.forge && data.forge.prng) {
        ctx.seedFile(data.forge.prng.needed, function(err, bytes) {
          worker.postMessage({forge: {prng: {err: err, bytes: bytes}}});
        });
      }
    };
    // TODO: do we need to remove the event listener when the worker dies?
    worker.addEventListener('message', listener);
  }
}
```
- example usage
```shell
...
forge.random.seedFile = function(needed, callback) {
  // get the 'needed' number of random bytes from somewhere
  callback(null, fetchedRandomBytes);
});

// register the main thread to send entropy or a Web Worker to receive
// entropy on demand from the main thread
forge.random.registerWorker(self);

// generate a new instance of a PRNG with no collected entropy
var myPrng = forge.random.createInstance();
'''

<a name="task" />
### Tasks
...
```

#### <a name="apidoc.element.node-forge.random.seedFile"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>seedFile (needed, callback)](#apidoc.element.node-forge.random.seedFile)
- description and source-code
```javascript
seedFile = function (needed, callback) {
  _crypto.randomBytes(needed, function(err, bytes) {
    if(err) {
      return callback(err);
    }
    callback(null, bytes.toString());
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.random.seedFileSync"></a>[function <span class="apidocSignatureSpan">node-forge.random.</span>seedFileSync (needed)](#apidoc.element.node-forge.random.seedFileSync)
- description and source-code
```javascript
seedFileSync = function (needed) {
  return _crypto.randomBytes(needed).toString();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.random.plugin"></a>[module node-forge.random.plugin](#apidoc.module.node-forge.random.plugin)

#### <a name="apidoc.element.node-forge.random.plugin.cipher"></a>[function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>cipher (key, seed)](#apidoc.element.node-forge.random.plugin.cipher)
- description and source-code
```javascript
cipher = function (key, seed) {
  forge.aes._updateBlock(key, seed, _prng_aes_output, false);
  _prng_aes_buffer.putInt32(_prng_aes_output[0]);
  _prng_aes_buffer.putInt32(_prng_aes_output[1]);
  _prng_aes_buffer.putInt32(_prng_aes_output[2]);
  _prng_aes_buffer.putInt32(_prng_aes_output[3]);
  return _prng_aes_buffer.getBytes();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.random.plugin.formatKey"></a>[function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>formatKey (key)](#apidoc.element.node-forge.random.plugin.formatKey)
- description and source-code
```javascript
formatKey = function (key) {
  // convert the key into 32-bit integers
  var tmp = forge.util.createBuffer(key);
  key = new Array(4);
  key[0] = tmp.getInt32();
  key[1] = tmp.getInt32();
  key[2] = tmp.getInt32();
  key[3] = tmp.getInt32();

  // return the expanded key
  return forge.aes._expandKey(key, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.random.plugin.formatSeed"></a>[function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>formatSeed (seed)](#apidoc.element.node-forge.random.plugin.formatSeed)
- description and source-code
```javascript
formatSeed = function (seed) {
  // convert seed into 32-bit integers
  var tmp = forge.util.createBuffer(seed);
  seed = new Array(4);
  seed[0] = tmp.getInt32();
  seed[1] = tmp.getInt32();
  seed[2] = tmp.getInt32();
  seed[3] = tmp.getInt32();
  return seed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.random.plugin.increment"></a>[function <span class="apidocSignatureSpan">node-forge.random.plugin.</span>increment (seed)](#apidoc.element.node-forge.random.plugin.increment)
- description and source-code
```javascript
increment = function (seed) {
  // FIXME: do we care about carry or signed issues?
  ++seed[3];
  return seed;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.rc2"></a>[module node-forge.rc2](#apidoc.module.node-forge.rc2)

#### <a name="apidoc.element.node-forge.rc2.createDecryptionCipher"></a>[function <span class="apidocSignatureSpan">node-forge.rc2.</span>createDecryptionCipher (key, bits)](#apidoc.element.node-forge.rc2.createDecryptionCipher)
- description and source-code
```javascript
createDecryptionCipher = function (key, bits) {
  return createCipher(key, bits, false);
}
```
- example usage
```shell
...
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes
var cipher = forge.rc2.createDecryptionCipher(key);
cipher.start(iv);
cipher.update(encrypted);
cipher.finish();
// outputs decrypted hex
console.log(cipher.output.toHex());
'''
...
```

#### <a name="apidoc.element.node-forge.rc2.createEncryptionCipher"></a>[function <span class="apidocSignatureSpan">node-forge.rc2.</span>createEncryptionCipher (key, bits)](#apidoc.element.node-forge.rc2.createEncryptionCipher)
- description and source-code
```javascript
createEncryptionCipher = function (key, bits) {
  return createCipher(key, bits, true);
}
```
- example usage
```shell
...

'''js
// generate a random key and IV
var key = forge.random.getBytesSync(16);
var iv = forge.random.getBytesSync(8);

// encrypt some bytes
var cipher = forge.rc2.createEncryptionCipher(key);
cipher.start(iv);
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());
...
```

#### <a name="apidoc.element.node-forge.rc2.expandKey"></a>[function <span class="apidocSignatureSpan">node-forge.rc2.</span>expandKey (key, effKeyBits)](#apidoc.element.node-forge.rc2.expandKey)
- description and source-code
```javascript
expandKey = function (key, effKeyBits) {
  if(typeof key === 'string') {
    key = forge.util.createBuffer(key);
  }
  effKeyBits = effKeyBits || 128;

<span class="apidocCodeCommentSpan">  /* introduce variables that match the names used in RFC #2268 */
</span>  var L = key;
  var T = key.length();
  var T1 = effKeyBits;
  var T8 = Math.ceil(T1 / 8);
  var TM = 0xff >> (T1 & 0x07);
  var i;

  for(i = T; i < 128; i++) {
    L.putByte(piTable[(L.at(i - 1) + L.at(i - T)) & 0xff]);
  }

  L.setAt(128 - T8, piTable[L.at(128 - T8) & TM]);

  for(i = 127 - T8; i >= 0; i--) {
    L.setAt(i, piTable[L.at(i + 1) ^ L.at(i + T8)]);
  }

  return L;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.rc2.startDecrypting"></a>[function <span class="apidocSignatureSpan">node-forge.rc2.</span>startDecrypting (key, iv, output)](#apidoc.element.node-forge.rc2.startDecrypting)
- description and source-code
```javascript
startDecrypting = function (key, iv, output) {
  var cipher = forge.rc2.createDecryptionCipher(key, 128);
  cipher.start(iv, output);
  return cipher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.rc2.startEncrypting"></a>[function <span class="apidocSignatureSpan">node-forge.rc2.</span>startEncrypting (key, iv, output)](#apidoc.element.node-forge.rc2.startEncrypting)
- description and source-code
```javascript
startEncrypting = function (key, iv, output) {
  var cipher = forge.rc2.createEncryptionCipher(key, 128);
  cipher.start(iv, output);
  return cipher;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.rsa"></a>[module node-forge.rsa](#apidoc.module.node-forge.rsa)

#### <a name="apidoc.element.node-forge.rsa.createKeyPairGenerationState"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>createKeyPairGenerationState (bits, e, options)](#apidoc.element.node-forge.rsa.createKeyPairGenerationState)
- description and source-code
```javascript
createKeyPairGenerationState = function (bits, e, options) {
  // TODO: migrate step-based prime generation code to forge.prime

  // set default bits
  if(typeof(bits) === 'string') {
    bits = parseInt(bits, 10);
  }
  bits = bits || 2048;

  // create prng with api that matches BigInteger secure random
  options = options || {};
  var prng = options.prng || forge.random;
  var rng = {
    // x is an array to fill with bytes
    nextBytes: function(x) {
      var b = prng.getBytesSync(x.length);
      for(var i = 0; i < x.length; ++i) {
        x[i] = b.charCodeAt(i);
      }
    }
  };

  var algorithm = options.algorithm || 'PRIMEINC';

  // create PRIMEINC algorithm state
  var rval;
  if(algorithm === 'PRIMEINC') {
    rval = {
      algorithm: algorithm,
      state: 0,
      bits: bits,
      rng: rng,
      eInt: e || 65537,
      e: new BigInteger(null),
      p: null,
      q: null,
      qBits: bits >> 1,
      pBits: bits - (bits >> 1),
      pqState: 0,
      num: null,
      keys: null
    };
    rval.e.fromInt(rval.eInt);
  } else {
    throw new Error('Invalid key generation algorithm: ' + algorithm);
  }

  return rval;
}
```
- example usage
```shell
...
// native APIs if available.
rsa.generateKeyPair({bits: 2048, workers: 2}, function(err, keypair) {
// keypair.privateKey, keypair.publicKey
});

// generate an RSA key pair in steps that attempt to run for a specified period
// of time on the main JS thread
var state = rsa.createKeyPairGenerationState(2048, 0x10001);
var step = function() {
// run for 100 ms
if(!rsa.stepKeyPairGenerationState(state, 100)) {
  setTimeout(step, 1);
}
else {
  // done, turn off progress indicator, use state.keys
...
```

#### <a name="apidoc.element.node-forge.rsa.decrypt"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>decrypt (ed, key, pub, ml)](#apidoc.element.node-forge.rsa.decrypt)
- description and source-code
```javascript
decrypt = function (ed, key, pub, ml) {
  // get the length of the modulus in bytes
  var k = Math.ceil(key.n.bitLength() / 8);

  // error if the length of the encrypted data ED is not k
  if(ed.length !== k) {
    var error = new Error('Encrypted message length is invalid.');
    error.length = ed.length;
    error.expected = k;
    throw error;
  }

  // convert encrypted data into a big integer
  // FIXME: hex conversion inefficient, get BigInteger w/byte strings
  var y = new BigInteger(forge.util.createBuffer(ed).toHex(), 16);

  // y must be less than the modulus or it wasn't the result of
  // a previous mod operation (encryption) using that modulus
  if(y.compareTo(key.n) >= 0) {
    throw new Error('Encrypted message is invalid.');
  }

  // do RSA decryption
  var x = _modPow(y, key, pub);

  // create the encryption block, if x is shorter in bytes than k, then
  // prepend zero bytes to fill up eb
  // FIXME: hex conversion inefficient, get BigInteger w/byte strings
  var xhex = x.toString(16);
  var eb = forge.util.createBuffer();
  var zeros = k - Math.ceil(xhex.length / 2);
  while(zeros > 0) {
    eb.putByte(0x00);
    --zeros;
  }
  eb.putBytes(forge.util.hexToBytes(xhex));

  if(ml !== false) {
    // legacy, default to PKCS#1 v1.5 padding
    return _decodePkcs1_v1_5(eb.getBytes(), key, pub);
  }

  // return message
  return eb.getBytes();
}
```
- example usage
```shell
...
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');

// decrypt data with a private key using RSAES PKCS#1 v1.5
var decrypted = privateKey.decrypt(encrypted, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.rsa.encrypt"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>encrypt (m, key, bt)](#apidoc.element.node-forge.rsa.encrypt)
- description and source-code
```javascript
encrypt = function (m, key, bt) {
  var pub = bt;
  var eb;

  // get the length of the modulus in bytes
  var k = Math.ceil(key.n.bitLength() / 8);

  if(bt !== false && bt !== true) {
    // legacy, default to PKCS#1 v1.5 padding
    pub = (bt === 0x02);
    eb = _encodePkcs1_v1_5(m, key, bt);
  } else {
    eb = forge.util.createBuffer();
    eb.putBytes(m);
  }

  // load encryption block as big integer 'x'
  // FIXME: hex conversion inefficient, get BigInteger w/byte strings
  var x = new BigInteger(eb.toHex(), 16);

  // do RSA encryption
  var y = _modPow(x, key, pub);

  // convert y into the encrypted data byte string, if y is shorter in
  // bytes than k, then prepend zero bytes to fill up ed
  // FIXME: hex conversion inefficient, get BigInteger w/byte strings
  var yhex = y.toString(16);
  var ed = forge.util.createBuffer();
  var zeros = k - Math.ceil(yhex.length / 2);
  while(zeros > 0) {
    ed.putByte(0x00);
    --zeros;
  }
  ed.putBytes(forge.util.hexToBytes(yhex));
  return ed.getBytes();
}
```
- example usage
```shell
...
  // optionally pass 'prng' with a custom PRNG implementation
});
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
publicKey.verify(md.digest().getBytes(), signature, pss);

// encrypt data with a public key (defaults to RSAES PKCS#1 v1.5)
var encrypted = publicKey.encrypt(bytes);

// decrypt data with a private key (defaults to RSAES PKCS#1 v1.5)
var decrypted = privateKey.decrypt(encrypted);

// encrypt data with a public key using RSAES PKCS#1 v1.5
var encrypted = publicKey.encrypt(bytes, 'RSAES-PKCS1-V1_5');
...
```

#### <a name="apidoc.element.node-forge.rsa.generateKeyPair"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>generateKeyPair (bits, e, options, callback)](#apidoc.element.node-forge.rsa.generateKeyPair)
- description and source-code
```javascript
generateKeyPair = function (bits, e, options, callback) {
  // (bits), (options), (callback)
  if(arguments.length === 1) {
    if(typeof bits === 'object') {
      options = bits;
      bits = undefined;
    } else if(typeof bits === 'function') {
      callback = bits;
      bits = undefined;
    }
  } else if(arguments.length === 2) {
    // (bits, e), (bits, options), (bits, callback), (options, callback)
    if(typeof bits === 'number') {
      if(typeof e === 'function') {
        callback = e;
        e = undefined;
      } else if(typeof e !== 'number') {
        options = e;
        e = undefined;
      }
    } else {
      options = bits;
      callback = e;
      bits = undefined;
      e = undefined;
    }
  } else if(arguments.length === 3) {
    // (bits, e, options), (bits, e, callback), (bits, options, callback)
    if(typeof e === 'number') {
      if(typeof options === 'function') {
        callback = options;
        options = undefined;
      }
    } else {
      callback = options;
      options = e;
      e = undefined;
    }
  }
  options = options || {};
  if(bits === undefined) {
    bits = options.bits || 2048;
  }
  if(e === undefined) {
    e = options.e || 0x10001;
  }

  // if native code is permitted and a callback is given, use native
  // key generation code if available and if parameters are acceptable
  if(!forge.options.usePureJavaScript && callback &&
    bits >= 256 && bits <= 16384 && (e === 0x10001 || e === 3)) {
    if(_detectSubtleCrypto('generateKey') && _detectSubtleCrypto('exportKey')) {
      // use standard native generateKey
      return window.crypto.subtle.generateKey({
        name: 'RSASSA-PKCS1-v1_5',
        modulusLength: bits,
        publicExponent: _intToUint8Array(e),
        hash: {name: 'SHA-256'}
      }, true /* key can be exported*/, ['sign', 'verify'])
      .then(function(pair) {
        return window.crypto.subtle.exportKey('pkcs8', pair.privateKey);
      // avoiding catch(function(err) {...}) to support IE <= 8
      }).then(undefined, function(err) {
        callback(err);
      }).then(function(pkcs8) {
        if(pkcs8) {
          var privateKey = pki.privateKeyFromAsn1(
            asn1.fromDer(forge.util.createBuffer(pkcs8)));
          callback(null, {
            privateKey: privateKey,
            publicKey: pki.setRsaPublicKey(privateKey.n, privateKey.e)
          });
        }
      });
    }
    if(_detectSubtleMsCrypto('generateKey') &&
      _detectSubtleMsCrypto('exportKey')) {
      var genOp = window.msCrypto.subtle.generateKey({
        name: 'RSASSA-PKCS1-v1_5',
        modulusLength: bits,
        publicExponent: _intToUint8Array(e),
        hash: {name: 'SHA-256'}
      }, true /* key can be exported*/, ['sign', 'verify']);
      genOp.oncomplete = function(e) {
        var pair = e.target.result;
        var exportOp = window.msCrypto.subtle.exportKey(
          'pkcs8', pair.privateKey);
        exportOp.oncomplete = function(e) {
          var pkcs8 = e.target.result;
          var privateKey = pki.privateKeyFromAsn1(
            asn1.fromDer(forge.util.createBuffer(pkcs8)));
          callback(null, {
            privateKey: privateKey,
            publicKey: pki.setRsaPublicKey(privateKey.n, privateKey.e)
          });
        };
        exportOp.onerror = function(err) {
          callback(err);
        };
      };
      genOp.onerror = function(err) {
        callback(err);
      };
      return;
    }
  }

  // use JavaScript implementation
  var state = pki.rsa.createKeyPairGenerationState(bits, e, options);
  if(!callback) {
    pki.rsa.stepKeyPairGenerationState(state, 0);
    return state.keys;
  }
  _generateKeyPair(state, options, callback);
}
```
- example usage
```shell
...

'''js
var rsa = forge.pki.rsa;

// generate an RSA key pair synchronously
// *NOT RECOMMENDED* -- can be significantly slower than async and will not
// use native APIs if available.
var keypair = rsa.generateKeyPair({bits: 2048, e: 0x10001});

// generate an RSA key pair asynchronously (uses web workers if available)
// use workers: -1 to run a fast core estimator to optimize # of workers
// *RECOMMENDED* - can be significantly faster than sync -- and will use
// native APIs if available.
rsa.generateKeyPair({bits: 2048, workers: 2}, function(err, keypair) {
// keypair.privateKey, keypair.publicKey
...
```

#### <a name="apidoc.element.node-forge.rsa.setPrivateKey"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>setPrivateKey ( n, e, d, p, q, dP, dQ, qInv)](#apidoc.element.node-forge.rsa.setPrivateKey)
- description and source-code
```javascript
setPrivateKey = function ( n, e, d, p, q, dP, dQ, qInv) {
  var key = {
    n: n,
    e: e,
    d: d,
    p: p,
    q: q,
    dP: dP,
    dQ: dQ,
    qInv: qInv
  };

<span class="apidocCodeCommentSpan">  /**
   * Decrypts the given data with this private key. The decryption scheme
   * must match the one used to encrypt the data.
   *
   * @param data the byte string to decrypt.
   * @param scheme the decryption scheme to use:
   *          'RSAES-PKCS1-V1_5' (default),
   *          'RSA-OAEP',
   *          'RAW', 'NONE', or null to perform raw RSA decryption.
   * @param schemeOptions any scheme-specific options.
   *
   * @return the decrypted byte string.
   */
</span>  key.decrypt = function(data, scheme, schemeOptions) {
    if(typeof scheme === 'string') {
      scheme = scheme.toUpperCase();
    } else if(scheme === undefined) {
      scheme = 'RSAES-PKCS1-V1_5';
    }

    // do rsa decryption w/o any decoding
    var d = pki.rsa.decrypt(data, key, false, false);

    if(scheme === 'RSAES-PKCS1-V1_5') {
      scheme = { decode: _decodePkcs1_v1_5 };
    } else if(scheme === 'RSA-OAEP' || scheme === 'RSAES-OAEP') {
      scheme = {
        decode: function(d, key) {
          return forge.pkcs1.decode_rsa_oaep(key, d, schemeOptions);
        }
      };
    } else if(['RAW', 'NONE', 'NULL', null].indexOf(scheme) !== -1) {
      scheme = { decode: function(d) { return d; } };
    } else {
      throw new Error('Unsupported encryption scheme: "' + scheme + '".');
    }

    // decode according to scheme
    return scheme.decode(d, key, false);
  };

  /**
   * Signs the given digest, producing a signature.
   *
   * PKCS#1 supports multiple (currently two) signature schemes:
   * RSASSA-PKCS1-V1_5 and RSASSA-PSS.
   *
   * By default this implementation uses the "old scheme", i.e.
   * RSASSA-PKCS1-V1_5. In order to generate a PSS signature, provide
   * an instance of Forge PSS object as the scheme parameter.
   *
   * @param md the message digest object with the hash to sign.
   * @param scheme the signature scheme to use:
   *          'RSASSA-PKCS1-V1_5' or undefined for RSASSA PKCS#1 v1.5,
   *          a Forge PSS object for RSASSA-PSS,
   *          'NONE' or null for none, DigestInfo will not be used but
   *            PKCS#1 v1.5 padding will still be used.
   *
   * @return the signature as a byte string.
   */
  key.sign = function(md, scheme) {
    /* Note: The internal implementation of RSA operations is being
      transitioned away from a PKCS#1 v1.5 hard-coded scheme. Some legacy
      code like the use of an encoding block identifier 'bt' will eventually
      be removed. */

    // private key operation
    var bt = false;

    if(typeof scheme === 'string') {
      scheme = scheme.toUpperCase();
    }

    if(scheme === undefined || scheme === 'RSASSA-PKCS1-V1_5') {
      scheme = { encode: emsaPkcs1v15encode };
      bt = 0x01;
    } else if(scheme === 'NONE' || scheme === 'NULL' || scheme === null) {
      scheme = { encode: function() { return md; } };
      bt = 0x01;
    }

    // encode and then encrypt
    var d = scheme.encode(md, key.n.bitLength());
    return pki.rsa.encrypt(d, key, bt);
  };

  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.rsa.setPublicKey"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>setPublicKey (n, e)](#apidoc.element.node-forge.rsa.setPublicKey)
- description and source-code
```javascript
setPublicKey = function (n, e) {
  var key = {
    n: n,
    e: e
  };

<span class="apidocCodeCommentSpan">  /**
   * Encrypts the given data with this public key. Newer applications
   * should use the 'RSA-OAEP' decryption scheme, 'RSAES-PKCS1-V1_5' is for
   * legacy applications.
   *
   * @param data the byte string to encrypt.
   * @param scheme the encryption scheme to use:
   *          'RSAES-PKCS1-V1_5' (default),
   *          'RSA-OAEP',
   *          'RAW', 'NONE', or null to perform raw RSA encryption,
   *          an object with an 'encode' property set to a function
   *          with the signature 'function(data, key)' that returns
   *          a binary-encoded string representing the encoded data.
   * @param schemeOptions any scheme-specific options.
   *
   * @return the encrypted byte string.
   */
</span>  key.encrypt = function(data, scheme, schemeOptions) {
    if(typeof scheme === 'string') {
      scheme = scheme.toUpperCase();
    } else if(scheme === undefined) {
      scheme = 'RSAES-PKCS1-V1_5';
    }

    if(scheme === 'RSAES-PKCS1-V1_5') {
      scheme = {
        encode: function(m, key, pub) {
          return _encodePkcs1_v1_5(m, key, 0x02).getBytes();
        }
      };
    } else if(scheme === 'RSA-OAEP' || scheme === 'RSAES-OAEP') {
      scheme = {
        encode: function(m, key) {
          return forge.pkcs1.encode_rsa_oaep(key, m, schemeOptions);
        }
      };
    } else if(['RAW', 'NONE', 'NULL', null].indexOf(scheme) !== -1) {
      scheme = { encode: function(e) { return e; } };
    } else if(typeof scheme === 'string') {
      throw new Error('Unsupported encryption scheme: "' + scheme + '".');
    }

    // do scheme-based encoding then rsa encryption
    var e = scheme.encode(data, key, true);
    return pki.rsa.encrypt(e, key, true);
  };

  /**
   * Verifies the given signature against the given digest.
   *
   * PKCS#1 supports multiple (currently two) signature schemes:
   * RSASSA-PKCS1-V1_5 and RSASSA-PSS.
   *
   * By default this implementation uses the "old scheme", i.e.
   * RSASSA-PKCS1-V1_5, in which case once RSA-decrypted, the
   * signature is an OCTET STRING that holds a DigestInfo.
   *
   * DigestInfo ::= SEQUENCE {
   *   digestAlgorithm DigestAlgorithmIdentifier,
   *   digest Digest
   * }
   * DigestAlgorithmIdentifier ::= AlgorithmIdentifier
   * Digest ::= OCTET STRING
   *
   * To perform PSS signature verification, provide an instance
   * of Forge PSS object as the scheme parameter.
   *
   * @param digest the message digest hash to compare against the signature,
   *          as a binary-encoded string.
   * @param signature the signature to verify, as a binary-encoded string.
   * @param scheme signature verification scheme to use:
   *          'RSASSA-PKCS1-V1_5' or undefined for RSASSA PKCS#1 v1.5,
   *          a Forge PSS object for RSASSA-PSS,
   *          'NONE' or null for none, DigestInfo will not be expected, but
   *            PKCS#1 v1.5 padding will still be used.
   *
   * @return true if the signature was verified, false if not.
   */
   key.verify = function(digest, signature, scheme) {
     if(typeof scheme === 'string') {
       scheme = scheme.toUpperCase();
     } else if(scheme === undefined) {
       scheme = 'RSASSA-PKCS1-V1_5';
     }

     if(scheme === 'RSASSA-PKCS1-V1_5') {
       scheme = {
         verify: function(digest, d) {
           // remove padding
           d = _decodePkcs1_v1_5(d, key, true);
           // d is ASN.1 BER-encoded DigestInfo
           var obj = asn1.fromDer(d);
           // compare the given digest to the decrypted one
           return digest === obj.value[1].value;
         }
       };
     } else if(scheme === 'NONE' || scheme === 'NULL' || scheme === null) {
       scheme = {
         verify: function(digest, d) {
           // remove padding
           d = _decodePkcs1_v1_5(d, key, true);
           return digest === d;
         }
       };
     }

     // do rsa decryption w/o any decoding, then verify -- which does decoding
     var d = pki.rsa.decrypt(signature, key, true, false);
     return scheme.verify(digest, d, key.n.bitL ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.rsa.stepKeyPairGenerationState"></a>[function <span class="apidocSignatureSpan">node-forge.rsa.</span>stepKeyPairGenerationState (state, n)](#apidoc.element.node-forge.rsa.stepKeyPairGenerationState)
- description and source-code
```javascript
stepKeyPairGenerationState = function (state, n) {
  // set default algorithm if not set
  if(!('algorithm' in state)) {
    state.algorithm = 'PRIMEINC';
  }

  // TODO: migrate step-based prime generation code to forge.prime
  // TODO: abstract as PRIMEINC algorithm

  // do key generation (based on Tom Wu's rsa.js, see jsbn.js license)
  // with some minor optimizations and designed to run in steps

  // local state vars
  var THIRTY = new BigInteger(null);
  THIRTY.fromInt(30);
  var deltaIdx = 0;
  var op_or = function(x, y) { return x|y; };

  // keep stepping until time limit is reached or done
  var t1 = +new Date();
  var t2;
  var total = 0;
  while(state.keys === null && (n <= 0 || total < n)) {
    // generate p or q
    if(state.state === 0) {
<span class="apidocCodeCommentSpan">      /* Note: All primes are of the form:

        30k+i, for i < 30 and gcd(30, i)=1, where there are 8 values for i

        When we generate a random number, we always align it at 30k + 1. Each
        time the number is determined not to be prime we add to get to the
        next 'i', eg: if the number was at 30k + 1 we add 6. */
</span>      var bits = (state.p === null) ? state.pBits : state.qBits;
      var bits1 = bits - 1;

      // get a random number
      if(state.pqState === 0) {
        state.num = new BigInteger(bits, state.rng);
        // force MSB set
        if(!state.num.testBit(bits1)) {
          state.num.bitwiseTo(
            BigInteger.ONE.shiftLeft(bits1), op_or, state.num);
        }
        // align number on 30k+1 boundary
        state.num.dAddOffset(31 - state.num.mod(THIRTY).byteValue(), 0);
        deltaIdx = 0;

        ++state.pqState;
      } else if(state.pqState === 1) {
        // try to make the number a prime
        if(state.num.bitLength() > bits) {
          // overflow, try again
          state.pqState = 0;
          // do primality test
        } else if(state.num.isProbablePrime(
          _getMillerRabinTests(state.num.bitLength()))) {
          ++state.pqState;
        } else {
          // get next potential prime
          state.num.dAddOffset(GCD_30_DELTA[deltaIdx++ % 8], 0);
        }
      } else if(state.pqState === 2) {
        // ensure number is coprime with e
        state.pqState =
          (state.num.subtract(BigInteger.ONE).gcd(state.e)
          .compareTo(BigInteger.ONE) === 0) ? 3 : 0;
      } else if(state.pqState === 3) {
        // store p or q
        state.pqState = 0;
        if(state.p === null) {
          state.p = state.num;
        } else {
          state.q = state.num;
        }

        // advance state if both p and q are ready
        if(state.p !== null && state.q !== null) {
          ++state.state;
        }
        state.num = null;
      }
    } else if(state.state === 1) {
      // ensure p is larger than q (swap them if not)
      if(state.p.compareTo(state.q) < 0) {
        state.num = state.p;
        state.p = state.q;
        state.q = state.num;
      }
      ++state.state;
    } else if(state.state === 2) {
      // compute phi: (p - 1)(q - 1) (Euler's totient function)
      state.p1 = state.p.subtract(BigInteger.ONE);
      state.q1 = state.q.subtract(BigInteger.ONE);
      state.phi = state.p1.multiply(state.q1);
      ++state.state;
    } else if(state.state === 3) {
      // ensure e and phi are coprime
      if(state.phi.gcd(state.e).compareTo(BigInteger.ONE) === 0) {
        // phi and e are coprime, advance
        ++state.state;
      } else {
        // phi and e aren't coprime, so generate a new p and q
        state.p = null;
        state.q = null;
        state.state = 0;
      }
    } else if(state.state === 4) {
      // create n, ensure n is has the right number of bits
      state.n = state.p.multiply(state.q);

      // ensure n is right number of bits
      if(state.n.bitLength() === state.bits) {
        // success, advance
        ++state.state;
      } else {
        // failed, get new q
        state.q = null;
        state.state = 0;
      }
    } else if(state.state === 5) {
      // set keys
      var d = state.e.modInverse(state.phi);
      state.keys = {
        privateKey: pki.r ...
```
- example usage
```shell
...
});

// generate an RSA key pair in steps that attempt to run for a specified period
// of time on the main JS thread
var state = rsa.createKeyPairGenerationState(2048, 0x10001);
var step = function() {
  // run for 100 ms
  if(!rsa.stepKeyPairGenerationState(state, 100)) {
    setTimeout(step, 1);
  }
  else {
    // done, turn off progress indicator, use state.keys
  }
};
// turn on progress indicator, schedule generation to run
...
```



# <a name="apidoc.module.node-forge.sha1"></a>[module node-forge.sha1](#apidoc.module.node-forge.sha1)

#### <a name="apidoc.element.node-forge.sha1.create"></a>[function <span class="apidocSignatureSpan">node-forge.sha1.</span>create ()](#apidoc.element.node-forge.sha1.create)
- description and source-code
```javascript
create = function () {
  // do initialization as necessary
  if(!_initialized) {
    _init();
  }

  // SHA-1 state contains five 32-bit integers
  var _state = null;

  // input buffer
  var _input = forge.util.createBuffer();

  // used for word storage
  var _w = new Array(80);

  // message digest object
  var md = {
    algorithm: 'sha1',
    blockLength: 64,
    digestLength: 20,
    // 56-bit length of message so far (does not including padding)
    messageLength: 0,
    // true message length
    fullMessageLength: null,
    // size of message length in bytes
    messageLengthSize: 8
  };

<span class="apidocCodeCommentSpan">  /**
   * Starts the digest.
   *
   * @return this digest object.
   */
</span>  md.start = function() {
    // up to 56-bit message length for convenience
    md.messageLength = 0;

    // full message length (set md.messageLength64 for backwards-compatibility)
    md.fullMessageLength = md.messageLength64 = [];
    var int32s = md.messageLengthSize / 4;
    for(var i = 0; i < int32s; ++i) {
      md.fullMessageLength.push(0);
    }
    _input = forge.util.createBuffer();
    _state = {
      h0: 0x67452301,
      h1: 0xEFCDAB89,
      h2: 0x98BADCFE,
      h3: 0x10325476,
      h4: 0xC3D2E1F0
    };
    return md;
  };
  // start digest automatically for first time
  md.start();

  /**
   * Updates the digest with the given message input. The given input can
   * treated as raw input (no encoding will be applied) or an encoding of
   * 'utf8' maybe given to encode the input using UTF-8.
   *
   * @param msg the message input to update with.
   * @param encoding the encoding to use (default: 'raw', other: 'utf8').
   *
   * @return this digest object.
   */
  md.update = function(msg, encoding) {
    if(encoding === 'utf8') {
      msg = forge.util.encodeUtf8(msg);
    }

    // update message length
    var len = msg.length;
    md.messageLength += len;
    len = [(len / 0x100000000) >>> 0, len >>> 0];
    for(var i = md.fullMessageLength.length - 1; i >= 0; --i) {
      md.fullMessageLength[i] += len[1];
      len[1] = len[0] + ((md.fullMessageLength[i] / 0x100000000) >>> 0);
      md.fullMessageLength[i] = md.fullMessageLength[i] >>> 0;
      len[0] = ((len[1] / 0x100000000) >>> 0);
    }

    // add bytes to input buffer
    _input.putBytes(msg);

    // process bytes
    _update(_state, _w, _input);

    // compact input buffer every 2K or if empty
    if(_input.read > 2048 || _input.length() === 0) {
      _input.compact();
    }

    return md;
  };

   /**
    * Produces the digest.
    *
    * @return a byte buffer containing the digest value.
    */
   md.digest = function() {
    /* Note: Here we copy the remaining bytes in the input buffer and
    add the appropriate SHA-1 padding. Then we do the final update
    on a copy of the state so that if the user wants to get
    intermediate digests they can do so. */

    /* Determine the number of bytes that must be added to the message
    to ensure its length is congruent to 448 mod 512. In other words,
    the data to be digested must be a multiple of 512 bits (or 128 bytes).
    This data includes the message, some padding, and the length of the
    message. Since the length of the message will be encoded as 8 bytes (64
    bits), that means that the last segment of the data must have 56 bytes
    (448 bits) of message and padding. Therefore, the length of the message
    plus the padding must be congruent to 448 mod 512 because
    512 - 128 = 448.

    In order to fill up the message length it must be filled with
    padding that begins with 1 bit followed by all 0 bits. Padding
    must *always* be present, so if the message length is already
    congruent to 448 mod 512, then 512 padding bits must be added. */

    var finalBlock = forge.util.createBuffer();
    finalBlock.putBytes(_input.bytes());

    // compute remaining size to be digested (include message length size)
    var remaining = (
      md.fullMessageLength[md.fullMessageLength.length - 1] +
      md.messageLengthSize);

    // add padding for overflow blockSize - overflow
    // _padding starts with 1 byte with ...
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.sha256"></a>[module node-forge.sha256](#apidoc.module.node-forge.sha256)

#### <a name="apidoc.element.node-forge.sha256.create"></a>[function <span class="apidocSignatureSpan">node-forge.sha256.</span>create ()](#apidoc.element.node-forge.sha256.create)
- description and source-code
```javascript
create = function () {
  // do initialization as necessary
  if(!_initialized) {
    _init();
  }

  // SHA-256 state contains eight 32-bit integers
  var _state = null;

  // input buffer
  var _input = forge.util.createBuffer();

  // used for word storage
  var _w = new Array(64);

  // message digest object
  var md = {
    algorithm: 'sha256',
    blockLength: 64,
    digestLength: 32,
    // 56-bit length of message so far (does not including padding)
    messageLength: 0,
    // true message length
    fullMessageLength: null,
    // size of message length in bytes
    messageLengthSize: 8
  };

<span class="apidocCodeCommentSpan">  /**
   * Starts the digest.
   *
   * @return this digest object.
   */
</span>  md.start = function() {
    // up to 56-bit message length for convenience
    md.messageLength = 0;

    // full message length (set md.messageLength64 for backwards-compatibility)
    md.fullMessageLength = md.messageLength64 = [];
    var int32s = md.messageLengthSize / 4;
    for(var i = 0; i < int32s; ++i) {
      md.fullMessageLength.push(0);
    }
    _input = forge.util.createBuffer();
    _state = {
      h0: 0x6A09E667,
      h1: 0xBB67AE85,
      h2: 0x3C6EF372,
      h3: 0xA54FF53A,
      h4: 0x510E527F,
      h5: 0x9B05688C,
      h6: 0x1F83D9AB,
      h7: 0x5BE0CD19
    };
    return md;
  };
  // start digest automatically for first time
  md.start();

  /**
   * Updates the digest with the given message input. The given input can
   * treated as raw input (no encoding will be applied) or an encoding of
   * 'utf8' maybe given to encode the input using UTF-8.
   *
   * @param msg the message input to update with.
   * @param encoding the encoding to use (default: 'raw', other: 'utf8').
   *
   * @return this digest object.
   */
  md.update = function(msg, encoding) {
    if(encoding === 'utf8') {
      msg = forge.util.encodeUtf8(msg);
    }

    // update message length
    var len = msg.length;
    md.messageLength += len;
    len = [(len / 0x100000000) >>> 0, len >>> 0];
    for(var i = md.fullMessageLength.length - 1; i >= 0; --i) {
      md.fullMessageLength[i] += len[1];
      len[1] = len[0] + ((md.fullMessageLength[i] / 0x100000000) >>> 0);
      md.fullMessageLength[i] = md.fullMessageLength[i] >>> 0;
      len[0] = ((len[1] / 0x100000000) >>> 0);
    }

    // add bytes to input buffer
    _input.putBytes(msg);

    // process bytes
    _update(_state, _w, _input);

    // compact input buffer every 2K or if empty
    if(_input.read > 2048 || _input.length() === 0) {
      _input.compact();
    }

    return md;
  };

  /**
   * Produces the digest.
   *
   * @return a byte buffer containing the digest value.
   */
  md.digest = function() {
    /* Note: Here we copy the remaining bytes in the input buffer and
    add the appropriate SHA-256 padding. Then we do the final update
    on a copy of the state so that if the user wants to get
    intermediate digests they can do so. */

    /* Determine the number of bytes that must be added to the message
    to ensure its length is congruent to 448 mod 512. In other words,
    the data to be digested must be a multiple of 512 bits (or 128 bytes).
    This data includes the message, some padding, and the length of the
    message. Since the length of the message will be encoded as 8 bytes (64
    bits), that means that the last segment of the data must have 56 bytes
    (448 bits) of message and padding. Therefore, the length of the message
    plus the padding must be congruent to 448 mod 512 because
    512 - 128 = 448.

    In order to fill up the message length it must be filled with
    padding that begins with 1 bit followed by all 0 bits. Padding
    must *always* be present, so if the message length is already
    congruent to 448 mod 512, then 512 padding bits must be added. */

    var finalBlock = forge.util.createBuffer();
    finalBlock.putBytes(_input.bytes());

    // compute remaining size to be digested (include message length size)
    var remaining = (
      md.fullMessageLength[md.fullMessageLength.length - 1] +
      md.messageLengthSize);

    // add padding for ov ...
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.sha384"></a>[module node-forge.sha384](#apidoc.module.node-forge.sha384)

#### <a name="apidoc.element.node-forge.sha384.create"></a>[function <span class="apidocSignatureSpan">node-forge.sha384.</span>create ()](#apidoc.element.node-forge.sha384.create)
- description and source-code
```javascript
create = function () {
  return sha512.create('SHA-384');
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.sha512"></a>[module node-forge.sha512](#apidoc.module.node-forge.sha512)

#### <a name="apidoc.element.node-forge.sha512.create"></a>[function <span class="apidocSignatureSpan">node-forge.sha512.</span>create (algorithm)](#apidoc.element.node-forge.sha512.create)
- description and source-code
```javascript
create = function (algorithm) {
  // do initialization as necessary
  if(!_initialized) {
    _init();
  }

  if(typeof algorithm === 'undefined') {
    algorithm = 'SHA-512';
  }

  if(!(algorithm in _states)) {
    throw new Error('Invalid SHA-512 algorithm: ' + algorithm);
  }

  // SHA-512 state contains eight 64-bit integers (each as two 32-bit ints)
  var _state = _states[algorithm];
  var _h = null;

  // input buffer
  var _input = forge.util.createBuffer();

  // used for 64-bit word storage
  var _w = new Array(80);
  for(var wi = 0; wi < 80; ++wi) {
    _w[wi] = new Array(2);
  }

  // determine digest length by algorithm name (default)
  var digestLength = 64;
  switch (algorithm) {
    case 'SHA-384':
      digestLength = 48;
      break;
    case 'SHA-512/256':
      digestLength = 32;
      break;
    case 'SHA-512/224':
      digestLength = 28;
      break;
  }

  // message digest object
  var md = {
    // SHA-512 => sha512
    algorithm: algorithm.replace('-', '').toLowerCase(),
    blockLength: 128,
    digestLength: digestLength,
    // 56-bit length of message so far (does not including padding)
    messageLength: 0,
    // true message length
    fullMessageLength: null,
    // size of message length in bytes
    messageLengthSize: 16
  };

<span class="apidocCodeCommentSpan">  /**
   * Starts the digest.
   *
   * @return this digest object.
   */
</span>  md.start = function() {
    // up to 56-bit message length for convenience
    md.messageLength = 0;

    // full message length (set md.messageLength128 for backwards-compatibility)
    md.fullMessageLength = md.messageLength128 = [];
    var int32s = md.messageLengthSize / 4;
    for(var i = 0; i < int32s; ++i) {
      md.fullMessageLength.push(0);
    }
    _input = forge.util.createBuffer();
    _h = new Array(_state.length);
    for(var i = 0; i < _state.length; ++i) {
      _h[i] = _state[i].slice(0);
    }
    return md;
  };
  // start digest automatically for first time
  md.start();

  /**
   * Updates the digest with the given message input. The given input can
   * treated as raw input (no encoding will be applied) or an encoding of
   * 'utf8' maybe given to encode the input using UTF-8.
   *
   * @param msg the message input to update with.
   * @param encoding the encoding to use (default: 'raw', other: 'utf8').
   *
   * @return this digest object.
   */
  md.update = function(msg, encoding) {
    if(encoding === 'utf8') {
      msg = forge.util.encodeUtf8(msg);
    }

    // update message length
    var len = msg.length;
    md.messageLength += len;
    len = [(len / 0x100000000) >>> 0, len >>> 0];
    for(var i = md.fullMessageLength.length - 1; i >= 0; --i) {
      md.fullMessageLength[i] += len[1];
      len[1] = len[0] + ((md.fullMessageLength[i] / 0x100000000) >>> 0);
      md.fullMessageLength[i] = md.fullMessageLength[i] >>> 0;
      len[0] = ((len[1] / 0x100000000) >>> 0);
    }

    // add bytes to input buffer
    _input.putBytes(msg);

    // process bytes
    _update(_h, _w, _input);

    // compact input buffer every 2K or if empty
    if(_input.read > 2048 || _input.length() === 0) {
      _input.compact();
    }

    return md;
  };

  /**
   * Produces the digest.
   *
   * @return a byte buffer containing the digest value.
   */
  md.digest = function() {
    /* Note: Here we copy the remaining bytes in the input buffer and
    add the appropriate SHA-512 padding. Then we do the final update
    on a copy of the state so that if the user wants to get
    intermediate digests they can do so. */

    /* Determine the number of bytes that must be added to the message
    to ensure its length is congruent to 896 mod 1024. In other words,
    the data to be digested must be a multiple of 1024 bits (or 128 bytes).
    This data includes the message, some padding, and the length of the
    message. Since the length of the message will be encoded as 16 bytes (128
    bits), that means that the last segment of the data must have 112 bytes
    (896 bits) of message and padding. Therefore, the length of the message
    plus the padding must be congruent to 896 mod 1024 bec ...
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.sha512.sha224"></a>[module node-forge.sha512.sha224](#apidoc.module.node-forge.sha512.sha224)

#### <a name="apidoc.element.node-forge.sha512.sha224.create"></a>[function <span class="apidocSignatureSpan">node-forge.sha512.sha224.</span>create ()](#apidoc.element.node-forge.sha512.sha224.create)
- description and source-code
```javascript
create = function () {
  return sha512.create('SHA-512/224');
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.sha512.sha256"></a>[module node-forge.sha512.sha256](#apidoc.module.node-forge.sha512.sha256)

#### <a name="apidoc.element.node-forge.sha512.sha256.create"></a>[function <span class="apidocSignatureSpan">node-forge.sha512.sha256.</span>create ()](#apidoc.element.node-forge.sha512.sha256.create)
- description and source-code
```javascript
create = function () {
  return sha512.create('SHA-512/256');
}
```
- example usage
```shell
...
// 3DES key and IV sizes
var keySize = 24;
var ivSize = 8;

// get derived bytes
// Notes:
// 1. If using an alternative hash (eg: "-md sha1") pass
//   "forge.md.sha1.create()" as the final parameter.
// 2. If using "-nosalt", set salt to null.
var salt = forge.random.getBytesSync(8);
// var md = forge.md.sha1.create(); // "-md sha1"
var derivedBytes = forge.pbe.opensslDeriveBytes(
  password, salt, keySize + ivSize/*, md*/);
var buffer = forge.util.createBuffer(derivedBytes);
var key = buffer.getBytes(keySize);
...
```



# <a name="apidoc.module.node-forge.ssh"></a>[module node-forge.ssh](#apidoc.module.node-forge.ssh)

#### <a name="apidoc.element.node-forge.ssh.getPublicKeyFingerprint"></a>[function <span class="apidocSignatureSpan">node-forge.ssh.</span>getPublicKeyFingerprint (key, options)](#apidoc.element.node-forge.ssh.getPublicKeyFingerprint)
- description and source-code
```javascript
getPublicKeyFingerprint = function (key, options) {
  options = options || {};
  var md = options.md || forge.md.md5.create();

  var type = 'ssh-rsa';
  var buffer = forge.util.createBuffer();
  _addStringToBuffer(buffer, type);
  _addBigIntegerToBuffer(buffer, key.e);
  _addBigIntegerToBuffer(buffer, key.n);

  // hash public key bytes
  md.start();
  md.update(buffer.getBytes());
  var digest = md.digest();
  if(options.encoding === 'hex') {
    var hex = digest.toHex();
    if(options.delimiter) {
      return hex.match(/.{2}/g).join(options.delimiter);
    }
    return hex;
  } else if(options.encoding === 'binary') {
    return digest.getBytes();
  } else if(options.encoding) {
    throw new Error('Unknown encoding "' + options.encoding + '".');
  }
  return digest;
}
```
- example usage
```shell
...
// encodes a public RSA key as an OpenSSH file
forge.ssh.publicKeyToOpenSSH(key, comment);

// encodes a private RSA key as an OpenSSH file
forge.ssh.privateKeyToOpenSSH(privateKey, passphrase);

// gets the SSH public key fingerprint in a byte buffer
forge.ssh.getPublicKeyFingerprint(key);

// gets a hex-encoded, colon-delimited SSH public key fingerprint
forge.ssh.getPublicKeyFingerprint(key, {encoding: 'hex', delimiter: ':'});
'''

<a name="xhr" />
### XHR
...
```

#### <a name="apidoc.element.node-forge.ssh.privateKeyToOpenSSH"></a>[function <span class="apidocSignatureSpan">node-forge.ssh.</span>privateKeyToOpenSSH (privateKey, passphrase)](#apidoc.element.node-forge.ssh.privateKeyToOpenSSH)
- description and source-code
```javascript
privateKeyToOpenSSH = function (privateKey, passphrase) {
  if(!passphrase) {
    return forge.pki.privateKeyToPem(privateKey);
  }
  // OpenSSH private key is just a legacy format, it seems
  return forge.pki.encryptRsaPrivateKey(privateKey, passphrase,
    {legacy: true, algorithm: 'aes128'});
}
```
- example usage
```shell
...
// encodes (and optionally encrypts) a private RSA key as a Putty PPK file
forge.ssh.privateKeyToPutty(privateKey, passphrase, comment);

// encodes a public RSA key as an OpenSSH file
forge.ssh.publicKeyToOpenSSH(key, comment);

// encodes a private RSA key as an OpenSSH file
forge.ssh.privateKeyToOpenSSH(privateKey, passphrase);

// gets the SSH public key fingerprint in a byte buffer
forge.ssh.getPublicKeyFingerprint(key);

// gets a hex-encoded, colon-delimited SSH public key fingerprint
forge.ssh.getPublicKeyFingerprint(key, {encoding: 'hex', delimiter: ':'});
'''
...
```

#### <a name="apidoc.element.node-forge.ssh.privateKeyToPutty"></a>[function <span class="apidocSignatureSpan">node-forge.ssh.</span>privateKeyToPutty (privateKey, passphrase, comment)](#apidoc.element.node-forge.ssh.privateKeyToPutty)
- description and source-code
```javascript
privateKeyToPutty = function (privateKey, passphrase, comment) {
  comment = comment || '';
  passphrase = passphrase || '';
  var algorithm = 'ssh-rsa';
  var encryptionAlgorithm = (passphrase === '') ? 'none' : 'aes256-cbc';

  var ppk = 'PuTTY-User-Key-File-2: ' + algorithm + '\r\n';
  ppk += 'Encryption: ' + encryptionAlgorithm + '\r\n';
  ppk += 'Comment: ' + comment + '\r\n';

  // public key into buffer for ppk
  var pubbuffer = forge.util.createBuffer();
  _addStringToBuffer(pubbuffer, algorithm);
  _addBigIntegerToBuffer(pubbuffer, privateKey.e);
  _addBigIntegerToBuffer(pubbuffer, privateKey.n);

  // write public key
  var pub = forge.util.encode64(pubbuffer.bytes(), 64);
  var length = Math.floor(pub.length / 66) + 1; // 66 = 64 + \r\n
  ppk += 'Public-Lines: ' + length + '\r\n';
  ppk += pub;

  // private key into a buffer
  var privbuffer = forge.util.createBuffer();
  _addBigIntegerToBuffer(privbuffer, privateKey.d);
  _addBigIntegerToBuffer(privbuffer, privateKey.p);
  _addBigIntegerToBuffer(privbuffer, privateKey.q);
  _addBigIntegerToBuffer(privbuffer, privateKey.qInv);

  // optionally encrypt the private key
  var priv;
  if(!passphrase) {
    // use the unencrypted buffer
    priv = forge.util.encode64(privbuffer.bytes(), 64);
  } else {
    // encrypt RSA key using passphrase
    var encLen = privbuffer.length() + 16 - 1;
    encLen -= encLen % 16;

    // pad private key with sha1-d data -- needs to be a multiple of 16
    var padding = _sha1(privbuffer.bytes());

    padding.truncate(padding.length() - encLen + privbuffer.length());
    privbuffer.putBuffer(padding);

    var aeskey = forge.util.createBuffer();
    aeskey.putBuffer(_sha1('\x00\x00\x00\x00', passphrase));
    aeskey.putBuffer(_sha1('\x00\x00\x00\x01', passphrase));

    // encrypt some bytes using CBC mode
    // key is 40 bytes, so truncate *by* 8 bytes
    var cipher = forge.aes.createEncryptionCipher(aeskey.truncate(8), 'CBC');
    cipher.start(forge.util.createBuffer().fillWithByte(0, 16));
    cipher.update(privbuffer.copy());
    cipher.finish();
    var encrypted = cipher.output;

    // Note: this appears to differ from Putty -- is forge wrong, or putty?
    // due to padding we finish as an exact multiple of 16
    encrypted.truncate(16); // all padding

    priv = forge.util.encode64(encrypted.bytes(), 64);
  }

  // output private key
  length = Math.floor(priv.length / 66) + 1; // 64 + \r\n
  ppk += '\r\nPrivate-Lines: ' + length + '\r\n';
  ppk += priv;

  // MAC
  var mackey = _sha1('putty-private-key-file-mac-key', passphrase);

  var macbuffer = forge.util.createBuffer();
  _addStringToBuffer(macbuffer, algorithm);
  _addStringToBuffer(macbuffer, encryptionAlgorithm);
  _addStringToBuffer(macbuffer, comment);
  macbuffer.putInt32(pubbuffer.length());
  macbuffer.putBuffer(pubbuffer);
  macbuffer.putInt32(privbuffer.length());
  macbuffer.putBuffer(privbuffer);

  var hmac = forge.hmac.create();
  hmac.start('sha1', mackey);
  hmac.update(macbuffer.bytes());

  ppk += '\r\nPrivate-MAC: ' + hmac.digest().toHex() + '\r\n';

  return ppk;
}
```
- example usage
```shell
...

Provides some SSH utility functions.

__Examples__

'''js
// encodes (and optionally encrypts) a private RSA key as a Putty PPK file
forge.ssh.privateKeyToPutty(privateKey, passphrase, comment);

// encodes a public RSA key as an OpenSSH file
forge.ssh.publicKeyToOpenSSH(key, comment);

// encodes a private RSA key as an OpenSSH file
forge.ssh.privateKeyToOpenSSH(privateKey, passphrase);
...
```

#### <a name="apidoc.element.node-forge.ssh.publicKeyToOpenSSH"></a>[function <span class="apidocSignatureSpan">node-forge.ssh.</span>publicKeyToOpenSSH (key, comment)](#apidoc.element.node-forge.ssh.publicKeyToOpenSSH)
- description and source-code
```javascript
publicKeyToOpenSSH = function (key, comment) {
  var type = 'ssh-rsa';
  comment = comment || '';

  var buffer = forge.util.createBuffer();
  _addStringToBuffer(buffer, type);
  _addBigIntegerToBuffer(buffer, key.e);
  _addBigIntegerToBuffer(buffer, key.n);

  return type + ' ' + forge.util.encode64(buffer.bytes()) + ' ' + comment;
}
```
- example usage
```shell
...
__Examples__

'''js
// encodes (and optionally encrypts) a private RSA key as a Putty PPK file
forge.ssh.privateKeyToPutty(privateKey, passphrase, comment);

// encodes a public RSA key as an OpenSSH file
forge.ssh.publicKeyToOpenSSH(key, comment);

// encodes a private RSA key as an OpenSSH file
forge.ssh.privateKeyToOpenSSH(privateKey, passphrase);

// gets the SSH public key fingerprint in a byte buffer
forge.ssh.getPublicKeyFingerprint(key);
...
```



# <a name="apidoc.module.node-forge.task"></a>[module node-forge.task](#apidoc.module.node-forge.task)

#### <a name="apidoc.element.node-forge.task.cancel"></a>[function <span class="apidocSignatureSpan">node-forge.task.</span>cancel (type)](#apidoc.element.node-forge.task.cancel)
- description and source-code
```javascript
cancel = function (type) {
  // find the task queue
  if(type in sTaskQueues) {
    // empty all but the current task from the queue
    sTaskQueues[type] = [sTaskQueues[type][0]];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.task.createCondition"></a>[function <span class="apidocSignatureSpan">node-forge.task.</span>createCondition ()](#apidoc.element.node-forge.task.createCondition)
- description and source-code
```javascript
createCondition = function () {
  var cond = {
    // all tasks that are blocked
    tasks: {}
  };

<span class="apidocCodeCommentSpan">  /**
   * Causes the given task to block until notify is called. If the task
   * is already waiting on this condition then this is a no-op.
   *
   * @param task the task to cause to wait.
   */
</span>  cond.wait = function(task) {
    // only block once
    if(!(task.id in cond.tasks)) {
       task.block();
       cond.tasks[task.id] = task;
    }
  };

  /**
   * Notifies all waiting tasks to wake up.
   */
  cond.notify = function() {
    // since unblock() will run the next task from here, make sure to
    // clear the condition's blocked task list before unblocking
    var tmp = cond.tasks;
    cond.tasks = {};
    for(var id in tmp) {
      tmp[id].unblock();
    }
  };

  return cond;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.task.start"></a>[function <span class="apidocSignatureSpan">node-forge.task.</span>start (options)](#apidoc.element.node-forge.task.start)
- description and source-code
```javascript
start = function (options) {
  // create a new task
  var task = new Task({
    run: options.run,
    name: options.name || sNoTaskName
  });
  task.type = options.type;
  task.successCallback = options.success || null;
  task.failureCallback = options.failure || null;

  // append the task onto the appropriate queue
  if(!(task.type in sTaskQueues)) {
    if(sVL >= 1) {
      forge.log.verbose(cat, '[%s][%s] create queue [%s]',
        task.id, task.name, task.type);
    }
    // create the queue with the new task
    sTaskQueues[task.type] = [task];
    start(task);
  } else {
    // push the task onto the queue, it will be run after a task
    // with the same type completes
    sTaskQueues[options.type].push(task);
  }
}
```
- example usage
```shell
...
var key = forge.pkcs5.pbkdf2('password', salt, numIterations, 16);
*/

// encrypt some bytes using CBC mode
// (other modes include: ECB, CFB, OFB, CTR, and GCM)
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
...
```



# <a name="apidoc.module.node-forge.tls"></a>[module node-forge.tls](#apidoc.module.node-forge.tls)

#### <a name="apidoc.element.node-forge.tls.createConnection"></a>[function <span class="apidocSignatureSpan">node-forge.tls.</span>createConnection (options)](#apidoc.element.node-forge.tls.createConnection)
- description and source-code
```javascript
createConnection = function (options) {
  var caStore = null;
  if(options.caStore) {
    // if CA store is an array, convert it to a CA store object
    if(forge.util.isArray(options.caStore)) {
      caStore = forge.pki.createCaStore(options.caStore);
    } else {
      caStore = options.caStore;
    }
  } else {
    // create empty CA store
    caStore = forge.pki.createCaStore();
  }

  // setup default cipher suites
  var cipherSuites = options.cipherSuites || null;
  if(cipherSuites === null) {
    cipherSuites = [];
    for(var key in tls.CipherSuites) {
      cipherSuites.push(tls.CipherSuites[key]);
    }
  }

  // set default entity
  var entity = (options.server || false) ?
    tls.ConnectionEnd.server : tls.ConnectionEnd.client;

  // create session cache if requested
  var sessionCache = options.sessionCache ?
    tls.createSessionCache(options.sessionCache) : null;

  // create TLS connection
  var c = {
    version: {major: tls.Version.major, minor: tls.Version.minor},
    entity: entity,
    sessionId: options.sessionId,
    caStore: caStore,
    sessionCache: sessionCache,
    cipherSuites: cipherSuites,
    connected: options.connected,
    virtualHost: options.virtualHost || null,
    verifyClient: options.verifyClient || false,
    verify: options.verify || function(cn, vfd, dpth, cts) {return vfd;},
    getCertificate: options.getCertificate || null,
    getPrivateKey: options.getPrivateKey || null,
    getSignature: options.getSignature || null,
    input: forge.util.createBuffer(),
    tlsData: forge.util.createBuffer(),
    data: forge.util.createBuffer(),
    tlsDataReady: options.tlsDataReady,
    dataReady: options.dataReady,
    heartbeatReceived: options.heartbeatReceived,
    closed: options.closed,
    error: function(c, ex) {
      // set origin if not set
      ex.origin = ex.origin ||
        ((c.entity === tls.ConnectionEnd.client) ? 'client' : 'server');

      // send TLS alert
      if(ex.send) {
        tls.queue(c, tls.createAlert(c, ex.alert));
        tls.flush(c);
      }

      // error is fatal by default
      var fatal = (ex.fatal !== false);
      if(fatal) {
        // set fail flag
        c.fail = true;
      }

      // call error handler first
      options.error(c, ex);

      if(fatal) {
        // fatal error, close connection, do not clear fail
        c.close(false);
      }
    },
    deflate: options.deflate || null,
    inflate: options.inflate || null
  };

<span class="apidocCodeCommentSpan">  /**
   * Resets a closed TLS connection for reuse. Called in c.close().
   *
   * @param clearFail true to clear the fail flag (default: true).
   */
</span>  c.reset = function(clearFail) {
    c.version = {major: tls.Version.major, minor: tls.Version.minor};
    c.record = null;
    c.session = null;
    c.peerCertificate = null;
    c.state = {
      pending: null,
      current: null
    };
    c.expect = (c.entity === tls.ConnectionEnd.client) ? SHE : CHE;
    c.fragmented = null;
    c.records = [];
    c.open = false;
    c.handshakes = 0;
    c.handshaking = false;
    c.isConnected = false;
    c.fail = !(clearFail || typeof(clearFail) === 'undefined');
    c.input.clear();
    c.tlsData.clear();
    c.data.clear();
    c.state.current = tls.createConnectionState(c);
  };

  // do initial reset of connection
  c.reset();

  /**
   * Updates the current TLS engine state based on the given record.
   *
   * @param c the TLS connection.
   * @param record the TLS record to act on.
   */
  var _update = function(c, record) {
    // get record handler (align type in table by subtracting lowest)
    var aligned = record.type - tls.ContentType.change_cipher_spec;
    var handlers = ctTable[c.entity][c.expect];
    if(aligned in handlers) {
      handlers[aligned](c, record);
    } else {
      // unexpected record
      tls.handleUnexpected(c, record);
    }
  };

  /**
   * Reads the record header and initializes the next record on the given
   * connection.
   *
   * @param c the TLS connection with the next record.
   *
   * @return 0 if the input data could be processed, otherwise the
   *         number of bytes required fo ...
```
- example usage
```shell
...

Provides a native javascript client and server-side [TLS][] implementation.

__Examples__

'''js
// create TLS client
var client = forge.tls.createConnection({
server: false,
caStore: /* Array of PEM-formatted certs or a CA store object */,
sessionCache: {},
// supported cipher suites in order of preference
cipherSuites: [
  forge.tls.CipherSuites.TLS_RSA_WITH_AES_128_CBC_SHA,
  forge.tls.CipherSuites.TLS_RSA_WITH_AES_256_CBC_SHA],
...
```

#### <a name="apidoc.element.node-forge.tls.createSessionCache"></a>[function <span class="apidocSignatureSpan">node-forge.tls.</span>createSessionCache (cache, capacity)](#apidoc.element.node-forge.tls.createSessionCache)
- description and source-code
```javascript
createSessionCache = function (cache, capacity) {
  var rval = null;

  // assume input is already a session cache object
  if(cache && cache.getSession && cache.setSession && cache.order) {
    rval = cache;
  } else {
    // create cache
    rval = {};
    rval.cache = cache || {};
    rval.capacity = Math.max(capacity || 100, 1);
    rval.order = [];

    // store order for sessions, delete session overflow
    for(var key in cache) {
      if(rval.order.length <= capacity) {
        rval.order.push(key);
      } else {
        delete cache[key];
      }
    }

    // get a session from a session ID (or get any session)
    rval.getSession = function(sessionId) {
      var session = null;
      var key = null;

      // if session ID provided, use it
      if(sessionId) {
        key = forge.util.bytesToHex(sessionId);
      } else if(rval.order.length > 0) {
        // get first session from cache
        key = rval.order[0];
      }

      if(key !== null && key in rval.cache) {
        // get cached session and remove from cache
        session = rval.cache[key];
        delete rval.cache[key];
        for(var i in rval.order) {
          if(rval.order[i] === key) {
            rval.order.splice(i, 1);
            break;
          }
        }
      }

      return session;
    };

    // set a session in the cache
    rval.setSession = function(sessionId, session) {
      // remove session from cache if at capacity
      if(rval.order.length === rval.capacity) {
        var key = rval.order.shift();
        delete rval.cache[key];
      }
      // add session to cache
      var key = forge.util.bytesToHex(sessionId);
      rval.order.push(key);
      rval.cache[key] = session;
    };
  }

  return rval;
}
```
- example usage
```shell
...
 * The cache is an object mapping session IDs to internal opaque state.
 * An application might need to change the cache used by a particular
 * tlsSocket between connections if it accesses multiple TLS hosts.
 *
 * @param cache the session cache to use.
 */
tlsSocket.setSessionCache = function(cache) {
  c.sessionCache = tls.createSessionCache(cache);
};

/**
 * Connects this socket.
 *
 * @param options:
 *           host: the host to connect to.
...
```

#### <a name="apidoc.element.node-forge.tls.hmac_sha1"></a>[function <span class="apidocSignatureSpan">node-forge.tls.</span>hmac_sha1 (key, seqNum, record)](#apidoc.element.node-forge.tls.hmac_sha1)
- description and source-code
```javascript
hmac_sha1 = function (key, seqNum, record) {
<span class="apidocCodeCommentSpan">  /* MAC is computed like so:
  HMAC_hash(
    key, seqNum +
      TLSCompressed.type +
      TLSCompressed.version +
      TLSCompressed.length +
      TLSCompressed.fragment)
  */
</span>  var hmac = forge.hmac.create();
  hmac.start('SHA1', key);
  var b = forge.util.createBuffer();
  b.putInt32(seqNum[0]);
  b.putInt32(seqNum[1]);
  b.putByte(record.type);
  b.putByte(record.version.major);
  b.putByte(record.version.minor);
  b.putInt16(record.length);
  b.putBytes(record.fragment.bytes());
  hmac.update(b.getBytes());
  return hmac.digest().getBytes();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.tls.prf_tls1"></a>[function <span class="apidocSignatureSpan">node-forge.tls.</span>prf_tls1 (secret, label, seed, length)](#apidoc.element.node-forge.tls.prf_tls1)
- description and source-code
```javascript
prf_tls1 = function (secret, label, seed, length) {
  var rval = forge.util.createBuffer();

<span class="apidocCodeCommentSpan">  /* For TLS 1.0, the secret is split in half, into two secrets of equal
    length. If the secret has an odd length then the last byte of the first
    half will be the same as the first byte of the second. The length of the
    two secrets is half of the secret rounded up. */
</span>  var idx = (secret.length >> 1);
  var slen = idx + (secret.length & 1);
  var s1 = secret.substr(0, slen);
  var s2 = secret.substr(idx, slen);
  var ai = forge.util.createBuffer();
  var hmac = forge.hmac.create();
  seed = label + seed;

  // determine the number of iterations that must be performed to generate
  // enough output bytes, md5 creates 16 byte hashes, sha1 creates 20
  var md5itr = Math.ceil(length / 16);
  var sha1itr = Math.ceil(length / 20);

  // do md5 iterations
  hmac.start('MD5', s1);
  var md5bytes = forge.util.createBuffer();
  ai.putBytes(seed);
  for(var i = 0; i < md5itr; ++i) {
    // HMAC_hash(secret, A(i-1))
    hmac.start(null, null);
    hmac.update(ai.getBytes());
    ai.putBuffer(hmac.digest());

    // HMAC_hash(secret, A(i) + seed)
    hmac.start(null, null);
    hmac.update(ai.bytes() + seed);
    md5bytes.putBuffer(hmac.digest());
  }

  // do sha1 iterations
  hmac.start('SHA1', s2);
  var sha1bytes = forge.util.createBuffer();
  ai.clear();
  ai.putBytes(seed);
  for(var i = 0; i < sha1itr; ++i) {
    // HMAC_hash(secret, A(i-1))
    hmac.start(null, null);
    hmac.update(ai.getBytes());
    ai.putBuffer(hmac.digest());

    // HMAC_hash(secret, A(i) + seed)
    hmac.start(null, null);
    hmac.update(ai.bytes() + seed);
    sha1bytes.putBuffer(hmac.digest());
  }

  // XOR the md5 bytes with the sha1 bytes
  rval.putBytes(forge.util.xorBytes(
    md5bytes.getBytes(), sha1bytes.getBytes(), length));

  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.tls.wrapSocket"></a>[function <span class="apidocSignatureSpan">node-forge.tls.</span>wrapSocket (options)](#apidoc.element.node-forge.tls.wrapSocket)
- description and source-code
```javascript
wrapSocket = function (options) {
  // get raw socket
  var socket = options.socket;

  // create TLS socket
  var tlsSocket = {
    id: socket.id,
    // set handlers
    connected: socket.connected || function(e) {},
    closed: socket.closed || function(e) {},
    data: socket.data || function(e) {},
    error: socket.error || function(e) {}
  };

  // create TLS connection
  var c = forge.tls.createConnection({
    server: false,
    sessionId: options.sessionId || null,
    caStore: options.caStore || [],
    sessionCache: options.sessionCache || null,
    cipherSuites: options.cipherSuites || null,
    virtualHost: options.virtualHost,
    verify: options.verify,
    getCertificate: options.getCertificate,
    getPrivateKey: options.getPrivateKey,
    getSignature: options.getSignature,
    deflate: options.deflate,
    inflate: options.inflate,
    connected: function(c) {
      // first handshake complete, call handler
      if(c.handshakes === 1) {
        tlsSocket.connected({
          id: socket.id,
          type: 'connect',
          bytesAvailable: c.data.length()
        });
      }
    },
    tlsDataReady: function(c) {
      // send TLS data over socket
      return socket.send(c.tlsData.getBytes());
    },
    dataReady: function(c) {
      // indicate application data is ready
      tlsSocket.data({
        id: socket.id,
        type: 'socketData',
        bytesAvailable: c.data.length()
      });
    },
    closed: function(c) {
      // close socket
      socket.close();
    },
    error: function(c, e) {
      // send error, close socket
      tlsSocket.error({
        id: socket.id,
        type: 'tlsError',
        message: e.message,
        bytesAvailable: 0,
        error: e
      });
      socket.close();
    }
  });

  // handle doing handshake after connecting
  socket.connected = function(e) {
    c.handshake(options.sessionId);
  };

  // handle closing TLS connection
  socket.closed = function(e) {
    if(c.open && c.handshaking) {
      // error
      tlsSocket.error({
        id: socket.id,
        type: 'ioError',
        message: 'Connection closed during handshake.',
        bytesAvailable: 0
      });
    }
    c.close();

    // call socket handler
    tlsSocket.closed({
      id: socket.id,
      type: 'close',
      bytesAvailable: 0
    });
  };

  // handle error on socket
  socket.error = function(e) {
    // error
    tlsSocket.error({
      id: socket.id,
      type: e.type,
      message: e.message,
      bytesAvailable: 0
    });
    c.close();
  };

  // handle receiving raw TLS data from socket
  var _requiredBytes = 0;
  socket.data = function(e) {
    // drop data if connection not open
    if(!c.open) {
      socket.receive(e.bytesAvailable);
    } else {
      // only receive if there are enough bytes available to
      // process a record
      if(e.bytesAvailable >= _requiredBytes) {
        var count = Math.max(e.bytesAvailable, _requiredBytes);
        var data = socket.receive(count);
        if(data !== null) {
          _requiredBytes = c.process(data);
        }
      }
    }
  };

<span class="apidocCodeCommentSpan">  /**
   * Destroys this socket.
   */
</span>  tlsSocket.destroy = function() {
    socket.destroy();
  };

  /**
   * Sets this socket's TLS session cache. This should be called before
   * the socket is connected or after it is closed.
   *
   * The cache is an object mapping session IDs to internal opaque state.
   * An application might need to change the cache used by a particular
   * tlsSocket between connections if it accesses multiple TLS hosts.
   *
   * @param cache the session cache to use.
   */
  tlsSocket.setSessionCache = function(cache) {
    c.sessionCache = tls.createSessionCache(cache);
  };

  /**
   * Connects this socket.
   *
   * @param options:
   *           host: the host to connect to.
   *           port: the port to connect to.
   *           policyPort: the policy port to use (if non-default), 0 to
   *              use the flash default.
   *           policyUrl: the policy file URL to use (instead of port).
   */
  tlsSocket.connect = function(options) {
    socket ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.util"></a>[module node-forge.util](#apidoc.module.node-forge.util)

#### <a name="apidoc.element.node-forge.util.ByteBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>ByteBuffer (b)](#apidoc.element.node-forge.util.ByteBuffer)
- description and source-code
```javascript
function ByteStringBuffer(b) {
  // TODO: update to match DataBuffer API

  // the data in this buffer
  this.data = '';
  // the pointer for reading from this buffer
  this.read = 0;

  if(typeof b === 'string') {
    this.data = b;
  } else if(util.isArrayBuffer(b) || util.isArrayBufferView(b)) {
    // convert native buffer to forge buffer
    // FIXME: support native buffers internally instead
    var arr = new Uint8Array(b);
    try {
      this.data = String.fromCharCode.apply(null, arr);
    } catch(e) {
      for(var i = 0; i < arr.length; ++i) {
        this.putByte(arr[i]);
      }
    }
  } else if(b instanceof ByteStringBuffer ||
    (typeof b === 'object' && typeof b.data === 'string' &&
    typeof b.read === 'number')) {
    // copy existing buffer
    this.data = b.data;
    this.read = b.read;
  }

  // used for v8 optimization
  this._constructedStringLength = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteStringBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>ByteStringBuffer (b)](#apidoc.element.node-forge.util.ByteStringBuffer)
- description and source-code
```javascript
function ByteStringBuffer(b) {
  // TODO: update to match DataBuffer API

  // the data in this buffer
  this.data = '';
  // the pointer for reading from this buffer
  this.read = 0;

  if(typeof b === 'string') {
    this.data = b;
  } else if(util.isArrayBuffer(b) || util.isArrayBufferView(b)) {
    // convert native buffer to forge buffer
    // FIXME: support native buffers internally instead
    var arr = new Uint8Array(b);
    try {
      this.data = String.fromCharCode.apply(null, arr);
    } catch(e) {
      for(var i = 0; i < arr.length; ++i) {
        this.putByte(arr[i]);
      }
    }
  } else if(b instanceof ByteStringBuffer ||
    (typeof b === 'object' && typeof b.data === 'string' &&
    typeof b.read === 'number')) {
    // copy existing buffer
    this.data = b.data;
    this.read = b.read;
  }

  // used for v8 optimization
  this._constructedStringLength = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>DataBuffer (b, options)](#apidoc.element.node-forge.util.DataBuffer)
- description and source-code
```javascript
function DataBuffer(b, options) {
  // default options
  options = options || {};

  // pointers for read from/write to buffer
  this.read = options.readOffset || 0;
  this.growSize = options.growSize || 1024;

  var isArrayBuffer = util.isArrayBuffer(b);
  var isArrayBufferView = util.isArrayBufferView(b);
  if(isArrayBuffer || isArrayBufferView) {
    // use ArrayBuffer directly
    if(isArrayBuffer) {
      this.data = new DataView(b);
    } else {
      // TODO: adjust read/write offset based on the type of view
      // or specify that this must be done in the options ... that the
      // offsets are byte-based
      this.data = new DataView(b.buffer, b.byteOffset, b.byteLength);
    }
    this.write = ('writeOffset' in options ?
      options.writeOffset : this.data.byteLength);
    return;
  }

  // initialize to empty array buffer and add any given bytes using putBytes
  this.data = new DataView(new ArrayBuffer(0));
  this.write = 0;

  if(b !== null && b !== undefined) {
    this.putBytes(b);
  }

  if('writeOffset' in options) {
    this.write = options.writeOffset;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.bytesFromIP"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesFromIP (ip)](#apidoc.element.node-forge.util.bytesFromIP)
- description and source-code
```javascript
bytesFromIP = function (ip) {
  if(ip.indexOf('.') !== -1) {
    return util.bytesFromIPv4(ip);
  }
  if(ip.indexOf(':') !== -1) {
    return util.bytesFromIPv6(ip);
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.bytesFromIPv4"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesFromIPv4 (ip)](#apidoc.element.node-forge.util.bytesFromIPv4)
- description and source-code
```javascript
bytesFromIPv4 = function (ip) {
  ip = ip.split('.');
  if(ip.length !== 4) {
    return null;
  }
  var b = util.createBuffer();
  for(var i = 0; i < ip.length; ++i) {
    var num = parseInt(ip[i], 10);
    if(isNaN(num)) {
      return null;
    }
    b.putByte(num);
  }
  return b.getBytes();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.bytesFromIPv6"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesFromIPv6 (ip)](#apidoc.element.node-forge.util.bytesFromIPv6)
- description and source-code
```javascript
bytesFromIPv6 = function (ip) {
  var blanks = 0;
  ip = ip.split(':').filter(function(e) {
    if(e.length === 0) ++blanks;
    return true;
  });
  var zeros = (8 - ip.length + blanks) * 2;
  var b = util.createBuffer();
  for(var i = 0; i < 8; ++i) {
    if(!ip[i] || ip[i].length === 0) {
      b.fillWithByte(0, zeros);
      zeros = 0;
      continue;
    }
    var bytes = util.hexToBytes(ip[i]);
    if(bytes.length < 2) {
      b.putByte(0);
    }
    b.putBytes(bytes);
  }
  return b.getBytes();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.bytesToHex"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToHex (bytes)](#apidoc.element.node-forge.util.bytesToHex)
- description and source-code
```javascript
bytesToHex = function (bytes) {
  // TODO: deprecate: "Deprecated. Use util.binary.hex.encode instead."
  return util.createBuffer(bytes).toHex();
}
```
- example usage
```shell
...
be used automatically.

__Examples__

'''js
// get some random bytes synchronously
var bytes = forge.random.getBytesSync(32);
console.log(forge.util.bytesToHex(bytes));

// get some random bytes asynchronously
forge.random.getBytes(32, function(err, bytes) {
  console.log(forge.util.bytesToHex(bytes));
});

// collect some entropy if you'd like
...
```

#### <a name="apidoc.element.node-forge.util.bytesToIP"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToIP (bytes)](#apidoc.element.node-forge.util.bytesToIP)
- description and source-code
```javascript
bytesToIP = function (bytes) {
  if(bytes.length === 4) {
    return util.bytesToIPv4(bytes);
  }
  if(bytes.length === 16) {
    return util.bytesToIPv6(bytes);
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.bytesToIPv4"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToIPv4 (bytes)](#apidoc.element.node-forge.util.bytesToIPv4)
- description and source-code
```javascript
bytesToIPv4 = function (bytes) {
  if(bytes.length !== 4) {
    return null;
  }
  var ip = [];
  for(var i = 0; i < bytes.length; ++i) {
    ip.push(bytes.charCodeAt(i));
  }
  return ip.join('.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.bytesToIPv6"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>bytesToIPv6 (bytes)](#apidoc.element.node-forge.util.bytesToIPv6)
- description and source-code
```javascript
bytesToIPv6 = function (bytes) {
  if(bytes.length !== 16) {
    return null;
  }
  var ip = [];
  var zeroGroups = [];
  var zeroMaxGroup = 0;
  for(var i = 0; i < bytes.length; i += 2) {
    var hex = util.bytesToHex(bytes[i] + bytes[i + 1]);
    // canonicalize zero representation
    while(hex[0] === '0' && hex !== '0') {
      hex = hex.substr(1);
    }
    if(hex === '0') {
      var last = zeroGroups[zeroGroups.length - 1];
      var idx = ip.length;
      if(!last || idx !== last.end + 1) {
        zeroGroups.push({start: idx, end: idx});
      } else {
        last.end = idx;
        if((last.end - last.start) >
          (zeroGroups[zeroMaxGroup].end - zeroGroups[zeroMaxGroup].start)) {
          zeroMaxGroup = zeroGroups.length - 1;
        }
      }
    }
    ip.push(hex);
  }
  if(zeroGroups.length > 0) {
    var group = zeroGroups[zeroMaxGroup];
    // only shorten group of length > 0
    if(group.end - group.start > 0) {
      ip.splice(group.start, group.end - group.start + 1, '');
      if(group.start === 0) {
        ip.unshift('');
      }
      if(group.end === 7) {
        ip.push('');
      }
    }
  }
  return ip.join(':');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.clearItems"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>clearItems (api, id, location)](#apidoc.element.node-forge.util.clearItems)
- description and source-code
```javascript
clearItems = function (api, id, location) {
  _callStorageFunction(_clearItems, arguments, location);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.createBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>createBuffer (input, encoding)](#apidoc.element.node-forge.util.createBuffer)
- description and source-code
```javascript
createBuffer = function (input, encoding) {
  // TODO: deprecate, use new ByteBuffer() instead
  encoding = encoding || 'raw';
  if(input !== undefined && encoding === 'utf8') {
    input = util.encodeUtf8(input);
  }
  return new util.ByteBuffer(input);
}
```
- example usage
```shell
...
},
connected: function(connection) {
  console.log('connected');
  // send message to server
  connection.prepare(forge.util.encodeUtf8('Hi server!'));
  /* NOTE: experimental, start heartbeat retransmission timer
  myHeartbeatTimer = setInterval(function() {
    connection.prepareHeartbeatRequest(forge.util.createBuffer('1234'));
  }, 5*60*1000);*/
},
/* provide a client-side cert if you want
getCertificate: function(connection, hint) {
  return myClientCertificate;
},
/* the private key for the client-side cert if provided */
...
```

#### <a name="apidoc.element.node-forge.util.decode64"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>decode64 (input)](#apidoc.element.node-forge.util.decode64)
- description and source-code
```javascript
decode64 = function (input) {
  // TODO: deprecate: "Deprecated. Use util.binary.base64.decode instead."

  // remove all non-base64 characters
  input = input.replace(/[^A-Za-z0-9\+\/\=]/g, '');

  var output = '';
  var enc1, enc2, enc3, enc4;
  var i = 0;

  while(i < input.length) {
    enc1 = _base64Idx[input.charCodeAt(i++) - 43];
    enc2 = _base64Idx[input.charCodeAt(i++) - 43];
    enc3 = _base64Idx[input.charCodeAt(i++) - 43];
    enc4 = _base64Idx[input.charCodeAt(i++) - 43];

    output += String.fromCharCode((enc1 << 2) | (enc2 >> 4));
    if(enc3 !== 64) {
      // decoded at least 2 bytes
      output += String.fromCharCode(((enc2 & 15) << 4) | (enc3 >> 2));
      if(enc4 !== 64) {
        // decoded 3 bytes
        output += String.fromCharCode(((enc3 & 3) << 6) | enc4);
      }
    }
  }

  return output;
}
```
- example usage
```shell
...
a PKCS#12 container, try using the TripleDES algorithm. It can be passed
to 'forge.pkcs12.toPkcs12Asn1' using the '{algorithm: '3des'}' option.

__Examples__

'''js
// decode p12 from base64
var p12Der = forge.util.decode64(p12b64);
// get p12 as ASN.1 object
var p12Asn1 = forge.asn1.fromDer(p12Der);
// decrypt p12 using the password 'password'
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, 'password');
// decrypt p12 using non-strict parsing mode (resolves some ASN.1 parse errors)
var p12 = forge.pkcs12.pkcs12FromAsn1(p12Asn1, false, 'password');
// decrypt p12 using literally no password (eg: Mac OS X/apple push)
...
```

#### <a name="apidoc.element.node-forge.util.decodeUtf8"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>decodeUtf8 (str)](#apidoc.element.node-forge.util.decodeUtf8)
- description and source-code
```javascript
decodeUtf8 = function (str) {
  return decodeURIComponent(escape(str));
}
```
- example usage
```shell
...
  sendToServerSomehow(connection.tlsData.getBytes());
  // if you were communicating with the server below, you'd do:
  // server.process(connection.tlsData.getBytes());
},
dataReady: function(connection) {
  // clear data from the server is ready
  console.log('the server sent: ' +
    forge.util.decodeUtf8(connection.data.getBytes()));
  // close connection
  connection.close();
},
/* NOTE: experimental
heartbeatReceived: function(connection, payload) {
  // restart retransmission timer, look at payload
  clearInterval(myHeartbeatTimer);
...
```

#### <a name="apidoc.element.node-forge.util.deflate"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>deflate (api, bytes, raw)](#apidoc.element.node-forge.util.deflate)
- description and source-code
```javascript
deflate = function (api, bytes, raw) {
  bytes = util.decode64(api.deflate(util.encode64(bytes)).rval);

  // strip zlib header and trailer if necessary
  if(raw) {
    // zlib header is 2 bytes (CMF,FLG) where FLG indicates that
    // there is a 4-byte DICT (alder-32) block before the data if
    // its 5th bit is set
    var start = 2;
    var flg = bytes.charCodeAt(1);
    if(flg & 0x20) {
      start = 6;
    }
    // zlib trailer is 4 bytes of adler-32
    bytes = bytes.substring(start, bytes.length - 4);
  }

  return bytes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.deletePath"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>deletePath (object, keys)](#apidoc.element.node-forge.util.deletePath)
- description and source-code
```javascript
deletePath = function (object, keys) {
  // need to start at an object
  if(typeof(object) === 'object' && object !== null) {
    var i = 0;
    var len = keys.length;
    while(i < len) {
      var next = keys[i++];
      if(i == len) {
        // last
        delete object[next];
      } else {
        // more
        if(!(next in object) ||
          (typeof(object[next]) !== 'object') ||
          (object[next] === null)) {
           break;
        }
        object = object[next];
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.encode64"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>encode64 (input, maxline)](#apidoc.element.node-forge.util.encode64)
- description and source-code
```javascript
encode64 = function (input, maxline) {
  // TODO: deprecate: "Deprecated. Use util.binary.base64.encode instead."
  var line = '';
  var output = '';
  var chr1, chr2, chr3;
  var i = 0;
  while(i < input.length) {
    chr1 = input.charCodeAt(i++);
    chr2 = input.charCodeAt(i++);
    chr3 = input.charCodeAt(i++);

    // encode 4 character group
    line += _base64.charAt(chr1 >> 2);
    line += _base64.charAt(((chr1 & 3) << 4) | (chr2 >> 4));
    if(isNaN(chr2)) {
      line += '==';
    } else {
      line += _base64.charAt(((chr2 & 15) << 2) | (chr3 >> 6));
      line += isNaN(chr3) ? '=' : _base64.charAt(chr3 & 63);
    }

    if(maxline && line.length > maxline) {
      output += line.substr(0, maxline) + '\r\n';
      line = line.substr(maxline);
    }
  }
  output += line;
  return output;
}
```
- example usage
```shell
...
// (requires the use of Triple DES instead of AES)
var p12Asn1 = forge.pkcs12.toPkcs12Asn1(
  privateKey, certificateChain, 'password',
  {algorithm: '3des'});

// base64-encode p12
var p12Der = forge.asn1.toDer(p12Asn1).getBytes();
var p12b64 = forge.util.encode64(p12Der);

// create download link for p12
var a = document.createElement('a');
a.download = 'example.p12';
a.setAttribute('href', 'data:application/x-pkcs12;base64,' + p12b64);
a.appendChild(document.createTextNode('Download'));
'''
...
```

#### <a name="apidoc.element.node-forge.util.encodeUtf8"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>encodeUtf8 (str)](#apidoc.element.node-forge.util.encodeUtf8)
- description and source-code
```javascript
encodeUtf8 = function (str) {
  return unescape(encodeURIComponent(str));
}
```
- example usage
```shell
...
    }
  }
  return verified;
},
connected: function(connection) {
  console.log('connected');
  // send message to server
  connection.prepare(forge.util.encodeUtf8('Hi server!'));
  /* NOTE: experimental, start heartbeat retransmission timer
  myHeartbeatTimer = setInterval(function() {
    connection.prepareHeartbeatRequest(forge.util.createBuffer('1234'));
  }, 5*60*1000);*/
},
/* provide a client-side cert if you want
getCertificate: function(connection, hint) {
...
```

#### <a name="apidoc.element.node-forge.util.estimateCores"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>estimateCores (options, callback)](#apidoc.element.node-forge.util.estimateCores)
- description and source-code
```javascript
estimateCores = function (options, callback) {
  if(typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  if('cores' in util && !options.update) {
    return callback(null, util.cores);
  }
  if(typeof navigator !== 'undefined' &&
    'hardwareConcurrency' in navigator &&
    navigator.hardwareConcurrency > 0) {
    util.cores = navigator.hardwareConcurrency;
    return callback(null, util.cores);
  }
  if(typeof Worker === 'undefined') {
    // workers not available
    util.cores = 1;
    return callback(null, util.cores);
  }
  if(typeof Blob === 'undefined') {
    // can't estimate, default to 2
    util.cores = 2;
    return callback(null, util.cores);
  }

  // create worker concurrency estimation code as blob
  var blobUrl = URL.createObjectURL(new Blob(['(',
    function() {
      self.addEventListener('message', function(e) {
        // run worker for 4 ms
        var st = Date.now();
        var et = st + 4;
        while(Date.now() < et);
        self.postMessage({st: st, et: et});
      });
    }.toString(),
  ')()'], {type: 'application/javascript'}));

  // take 5 samples using 16 workers
  sample([], 5, 16);

  function sample(max, samples, numWorkers) {
    if(samples === 0) {
      // get overlap average
      var avg = Math.floor(max.reduce(function(avg, x) {
        return avg + x;
      }, 0) / max.length);
      util.cores = Math.max(1, avg);
      URL.revokeObjectURL(blobUrl);
      return callback(null, util.cores);
    }
    map(numWorkers, function(err, results) {
      max.push(reduce(numWorkers, results));
      sample(max, samples - 1, numWorkers);
    });
  }

  function map(numWorkers, callback) {
    var workers = [];
    var results = [];
    for(var i = 0; i < numWorkers; ++i) {
      var worker = new Worker(blobUrl);
      worker.addEventListener('message', function(e) {
        results.push(e.data);
        if(results.length === numWorkers) {
          for(var i = 0; i < numWorkers; ++i) {
            workers[i].terminate();
          }
          callback(null, results);
        }
      });
      workers.push(worker);
    }
    for(var i = 0; i < numWorkers; ++i) {
      workers[i].postMessage(i);
    }
  }

  function reduce(numWorkers, results) {
    // find overlapping time windows
    var overlaps = [];
    for(var n = 0; n < numWorkers; ++n) {
      var r1 = results[n];
      var overlap = overlaps[n] = [];
      for(var i = 0; i < numWorkers; ++i) {
        if(n === i) {
          continue;
        }
        var r2 = results[i];
        if((r1.st > r2.st && r1.st < r2.et) ||
          (r2.st > r1.st && r2.st < r1.et)) {
          overlap.push(i);
        }
      }
    }
    // get maximum overlaps ... don't include overlapping worker itself
    // as the main JS process was also being scheduled during the work and
    // would have to be subtracted from the estimate anyway
    return overlaps.reduce(function(max, overlap) {
      return Math.max(max, overlap.length);
    }, 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.fillString"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>fillString (c, n)](#apidoc.element.node-forge.util.fillString)
- description and source-code
```javascript
fillString = function (c, n) {
  var s = '';
  while(n > 0) {
    if(n & 1) {
      s += c;
    }
    n >>>= 1;
    if(n > 0) {
      c += c;
    }
  }
  return s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.format"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>format (format)](#apidoc.element.node-forge.util.format)
- description and source-code
```javascript
format = function (format) {
  var re = /%./g;
  // current match
  var match;
  // current part
  var part;
  // current arg index
  var argi = 0;
  // collected parts to recombine later
  var parts = [];
  // last index found
  var last = 0;
  // loop while matches remain
  while((match = re.exec(format))) {
    part = format.substring(last, re.lastIndex - 2);
    // don't add empty strings (ie, parts between %s%s)
    if(part.length > 0) {
      parts.push(part);
    }
    last = re.lastIndex;
    // switch on % code
    var code = match[0][1];
    switch(code) {
    case 's':
    case 'o':
      // check if enough arguments were given
      if(argi < arguments.length) {
        parts.push(arguments[argi++ + 1]);
      } else {
        parts.push('<?>');
      }
      break;
    // FIXME: do proper formating for numbers, etc
    //case 'f':
    //case 'd':
    case '%':
      parts.push('%');
      break;
    default:
      parts.push('<%' + code + '?>');
    }
  }
  // add trailing part of format string
  parts.push(format.substring(last));
  return parts.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.formatNumber"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>formatNumber (number, decimals, dec_point, thousands_sep)](#apidoc.element.node-forge.util.formatNumber)
- description and source-code
```javascript
formatNumber = function (number, decimals, dec_point, thousands_sep) {
  // http://kevin.vanzonneveld.net
  // +   original by: Jonas Raoni Soares Silva (http://www.jsfromhell.com)
  // +   improved by: Kevin van Zonneveld (http://kevin.vanzonneveld.net)
  // +     bugfix by: Michael White (http://crestidg.com)
  // +     bugfix by: Benjamin Lupton
  // +     bugfix by: Allan Jensen (http://www.winternet.no)
  // +    revised by: Jonas Raoni Soares Silva (http://www.jsfromhell.com)
  // *     example 1: number_format(1234.5678, 2, '.', '');
  // *     returns 1: 1234.57

  var n = number, c = isNaN(decimals = Math.abs(decimals)) ? 2 : decimals;
  var d = dec_point === undefined ? ',' : dec_point;
  var t = thousands_sep === undefined ?
   '.' : thousands_sep, s = n < 0 ? '-' : '';
  var i = parseInt((n = Math.abs(+n || 0).toFixed(c)), 10) + '';
  var j = (i.length > 3) ? i.length % 3 : 0;
  return s + (j ? i.substr(0, j) + t : '') +
    i.substr(j).replace(/(\d{3})(?=\d)/g, '$1' + t) +
    (c ? d + Math.abs(n - i).toFixed(c).slice(2) : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.formatSize"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>formatSize (size)](#apidoc.element.node-forge.util.formatSize)
- description and source-code
```javascript
formatSize = function (size) {
  if(size >= 1073741824) {
    size = util.formatNumber(size / 1073741824, 2, '.', '') + ' GiB';
  } else if(size >= 1048576) {
    size = util.formatNumber(size / 1048576, 2, '.', '') + ' MiB';
  } else if(size >= 1024) {
    size = util.formatNumber(size / 1024, 0) + ' KiB';
  } else {
    size = util.formatNumber(size, 0) + ' bytes';
  }
  return size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.getItem"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>getItem (api, id, key, location)](#apidoc.element.node-forge.util.getItem)
- description and source-code
```javascript
getItem = function (api, id, key, location) {
  return _callStorageFunction(_getItem, arguments, location);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.getPath"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>getPath (object, keys, _default)](#apidoc.element.node-forge.util.getPath)
- description and source-code
```javascript
getPath = function (object, keys, _default) {
  var i = 0;
  var len = keys.length;
  var hasNext = true;
  while(hasNext && i < len &&
    typeof(object) === 'object' && object !== null) {
    var next = keys[i++];
    hasNext = next in object;
    if(hasNext) {
      object = object[next];
    }
  }
  return (hasNext ? object : _default);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.getQueryVariables"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>getQueryVariables (query)](#apidoc.element.node-forge.util.getQueryVariables)
- description and source-code
```javascript
getQueryVariables = function (query) {
  var parse = function(q) {
    var rval = {};
    var kvpairs = q.split('&');
    for(var i = 0; i < kvpairs.length; i++) {
      var pos = kvpairs[i].indexOf('=');
      var key;
      var val;
      if(pos > 0) {
        key = kvpairs[i].substring(0, pos);
        val = kvpairs[i].substring(pos + 1);
      } else {
        key = kvpairs[i];
        val = null;
      }
      if(!(key in rval)) {
        rval[key] = [];
      }
      // disallow overriding object prototype keys
      if(!(key in Object.prototype) && val !== null) {
        rval[key].push(unescape(val));
      }
    }
    return rval;
  };

   var rval;
   if(typeof(query) === 'undefined') {
     // set cached variables if needed
     if(_queryVariables === null) {
       if(typeof(window) !== 'undefined' && window.location && window.location.search) {
          // parse window search query
          _queryVariables = parse(window.location.search.substring(1));
       } else {
          // no query variables available
          _queryVariables = {};
       }
     }
     rval = _queryVariables;
   } else {
     // parse given query
     rval = parse(query);
   }
   return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.hexToBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>hexToBytes (hex)](#apidoc.element.node-forge.util.hexToBytes)
- description and source-code
```javascript
hexToBytes = function (hex) {
  // TODO: deprecate: "Deprecated. Use util.binary.hex.decode instead."
  var rval = '';
  var i = 0;
  if(hex.length & 1 == 1) {
    // odd number of characters, convert first character alone
    i = 1;
    rval += String.fromCharCode(parseInt(hex[0], 16));
  }
  // convert 2 characters (1 byte) at a time
  for(; i < hex.length; i += 2) {
    rval += String.fromCharCode(parseInt(hex.substr(i, 2), 16));
  }
  return rval;
}
```
- example usage
```shell
...
var str = forge.util.decode64(encoded);

// encode/decode UTF-8
var encoded = forge.util.encodeUtf8(str);
var str = forge.util.decodeUtf8(encoded);

// bytes to/from hex
var bytes = forge.util.hexToBytes(hex);
var hex = forge.util.bytesToHex(bytes);

// create an empty byte buffer
var buffer = forge.util.createBuffer();
// create a byte buffer from raw binary bytes
var buffer = forge.util.createBuffer(input, 'raw');
// create a byte buffer from utf8 bytes
...
```

#### <a name="apidoc.element.node-forge.util.inflate"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>inflate (api, bytes, raw)](#apidoc.element.node-forge.util.inflate)
- description and source-code
```javascript
inflate = function (api, bytes, raw) {
  // TODO: add zlib header and trailer if necessary/possible
  var rval = api.inflate(util.encode64(bytes)).rval;
  return (rval === null) ? null : util.decode64(rval);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.int32ToBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>int32ToBytes (i)](#apidoc.element.node-forge.util.int32ToBytes)
- description and source-code
```javascript
int32ToBytes = function (i) {
  return (
    String.fromCharCode(i >> 24 & 0xFF) +
    String.fromCharCode(i >> 16 & 0xFF) +
    String.fromCharCode(i >> 8 & 0xFF) +
    String.fromCharCode(i & 0xFF));
}
```
- example usage
```shell
...

  // sync version
  if(!callback) {
    for(var i = 1; i <= len; ++i) {
// PRF(P, S || INT(i)) (first iteration)
prf.start(null, null);
prf.update(s);
prf.update(forge.util.int32ToBytes(i));
xor = u_c1 = prf.digest().getBytes();

// PRF(P, u_{c-1}) (other iterations)
for(var j = 2; j <= c; ++j) {
  prf.start(null, null);
  prf.update(u_c1);
  u_c = prf.digest().getBytes();
...
```

#### <a name="apidoc.element.node-forge.util.isArray"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>isArray ()](#apidoc.element.node-forge.util.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.isArrayBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>isArrayBuffer (x)](#apidoc.element.node-forge.util.isArrayBuffer)
- description and source-code
```javascript
isArrayBuffer = function (x) {
  return typeof ArrayBuffer !== 'undefined' && x instanceof ArrayBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.isArrayBufferView"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>isArrayBufferView (x)](#apidoc.element.node-forge.util.isArrayBufferView)
- description and source-code
```javascript
isArrayBufferView = function (x) {
  return x && util.isArrayBuffer(x.buffer) && x.byteLength !== undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.isEmpty"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>isEmpty (obj)](#apidoc.element.node-forge.util.isEmpty)
- description and source-code
```javascript
isEmpty = function (obj) {
  for(var prop in obj) {
    if(obj.hasOwnProperty(prop)) {
      return false;
    }
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.makeLink"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>makeLink (path, query, fragment)](#apidoc.element.node-forge.util.makeLink)
- description and source-code
```javascript
makeLink = function (path, query, fragment) {
  // join path parts if needed
  path = jQuery.isArray(path) ? path.join('/') : path;

  var qstr = jQuery.param(query || {});
  fragment = fragment || '';
  return path +
    ((qstr.length > 0) ? ('?' + qstr) : '') +
    ((fragment.length > 0) ? ('#' + fragment) : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.makeRequest"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>makeRequest (reqString)](#apidoc.element.node-forge.util.makeRequest)
- description and source-code
```javascript
makeRequest = function (reqString) {
  var frag = util.parseFragment(reqString);
  var req = {
    // full path string
    path: frag.pathString,
    // full query string
    query: frag.queryString,
<span class="apidocCodeCommentSpan">    /**
     * Get path or element in path.
     *
     * @param i optional path index.
     *
     * @return path or part of path if i provided.
     */
</span>    getPath: function(i) {
      return (typeof(i) === 'undefined') ? frag.path : frag.path[i];
    },
    /**
     * Get query, values for a key, or value for a key index.
     *
     * @param k optional query key.
     * @param i optional query key index.
     *
     * @return query, values for a key, or value for a key index.
     */
    getQuery: function(k, i) {
      var rval;
      if(typeof(k) === 'undefined') {
        rval = frag.query;
      } else {
        rval = frag.query[k];
        if(rval && typeof(i) !== 'undefined') {
           rval = rval[i];
        }
      }
      return rval;
    },
    getQueryLast: function(k, _default) {
      var rval;
      var vals = req.getQuery(k);
      if(vals) {
        rval = vals[vals.length - 1];
      } else {
        rval = _default;
      }
      return rval;
    }
  };
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.nextTick"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>nextTick (callback)](#apidoc.element.node-forge.util.nextTick)
- description and source-code
```javascript
function nextTick(callback) {
  if (typeof callback !== 'function')
    throw new TypeError('callback is not a function');
  // on the way out, don't bother. it won't get fired anyway.
  if (process._exiting)
    return;

  var args;
  if (arguments.length > 1) {
    args = new Array(arguments.length - 1);
    for (var i = 1; i < arguments.length; i++)
      args[i - 1] = arguments[i];
  }

  nextTickQueue.push({
    callback,
    domain: process.domain || null,
    args
  });
  tickInfo[kLength]++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.parseFragment"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>parseFragment (fragment)](#apidoc.element.node-forge.util.parseFragment)
- description and source-code
```javascript
parseFragment = function (fragment) {
  // default to whole fragment
  var fp = fragment;
  var fq = '';
  // split into path and query if possible at the first '?'
  var pos = fragment.indexOf('?');
  if(pos > 0) {
    fp = fragment.substring(0, pos);
    fq = fragment.substring(pos + 1);
  }
  // split path based on '/' and ignore first element if empty
  var path = fp.split('/');
  if(path.length > 0 && path[0] === '') {
    path.shift();
  }
  // convert query into object
  var query = (fq === '') ? {} : util.getQueryVariables(fq);

  return {
    pathString: fp,
    queryString: fq,
    path: path,
    query: query
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.parseUrl"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>parseUrl (str)](#apidoc.element.node-forge.util.parseUrl)
- description and source-code
```javascript
parseUrl = function (str) {
  // FIXME: this regex looks a bit broken
  var regex = /^(https?):\/\/([^:&^\/]*):?(\d*)(.*)$/g;
  regex.lastIndex = 0;
  var m = regex.exec(str);
  var url = (m === null) ? null : {
    full: str,
    scheme: m[1],
    host: m[2],
    port: m[3],
    path: m[4]
  };
  if(url) {
    url.fullHost = url.host;
    if(url.port) {
      if(url.port !== 80 && url.scheme === 'http') {
        url.fullHost += ':' + url.port;
      } else if(url.port !== 443 && url.scheme === 'https') {
        url.fullHost += ':' + url.port;
      }
    } else if(url.scheme === 'http') {
      url.port = 80;
    } else if(url.scheme === 'https') {
      url.port = 443;
    }
    url.full = url.scheme + '://' + url.fullHost;
  }
  return url;
}
```
- example usage
```shell
...

// convert a Node.js Buffer into a forge buffer
// make sure you specify the encoding as 'binary'
var nodeBuffer = new Buffer();
var forgeBuffer = forge.util.createBuffer(nodeBuffer.toString('binary'));

// parse a URL
var parsed = forge.util.parseUrl('http://example.com/foo?bar=baz');
// parsed.scheme, parsed.host, parsed.port, parsed.path, parsed.fullHost
'''

<a name="log" />
### Logging

Provides logging to a javascript console using various categories and
...
```

#### <a name="apidoc.element.node-forge.util.removeItem"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>removeItem (api, id, key, location)](#apidoc.element.node-forge.util.removeItem)
- description and source-code
```javascript
removeItem = function (api, id, key, location) {
  _callStorageFunction(_removeItem, arguments, location);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.setImmediate"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>setImmediate (callback, arg1, arg2, arg3)](#apidoc.element.node-forge.util.setImmediate)
- description and source-code
```javascript
setImmediate = function (callback, arg1, arg2, arg3) {
  if (typeof callback !== 'function') {
    throw new TypeError('"callback" argument must be a function');
  }

  var i, args;

  switch (arguments.length) {
    // fast cases
    case 1:
      break;
    case 2:
      args = [arg1];
      break;
    case 3:
      args = [arg1, arg2];
      break;
    default:
      args = [arg1, arg2, arg3];
      for (i = 4; i < arguments.length; i++)
        // extend array dynamically, makes .apply run much faster in v6.0.0
        args[i - 1] = arguments[i];
      break;
  }
  return createImmediate(args, callback);
}
```
- example usage
```shell
...
  prf.start(null, null);
  prf.update(u_c1);
  u_c = prf.digest().getBytes();
  // F(p, s, c, i)
  xor = forge.util.xorBytes(xor, u_c, hLen);
  u_c1 = u_c;
  ++j;
  return forge.util.setImmediate(inner);
}

/* 4. Concatenate the blocks and extract the first dkLen octets to
  produce a derived key DK:

  DK = T_1 || T_2 ||  ...  || T_len<0..r-1> */
dk += (i < len) ? xor : xor.substr(0, r);
...
```

#### <a name="apidoc.element.node-forge.util.setItem"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>setItem (api, id, key, data, location)](#apidoc.element.node-forge.util.setItem)
- description and source-code
```javascript
setItem = function (api, id, key, data, location) {
  _callStorageFunction(_setItem, arguments, location);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.setPath"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>setPath (object, keys, value)](#apidoc.element.node-forge.util.setPath)
- description and source-code
```javascript
setPath = function (object, keys, value) {
  // need to start at an object
  if(typeof(object) === 'object' && object !== null) {
    var i = 0;
    var len = keys.length;
    while(i < len) {
      var next = keys[i++];
      if(i == len) {
        // last
        object[next] = value;
      } else {
        // more
        var hasNext = (next in object);
        if(!hasNext ||
          (hasNext && typeof(object[next]) !== 'object') ||
          (hasNext && object[next] === null)) {
          object[next] = {};
        }
        object = object[next];
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.xorBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>xorBytes (s1, s2, n)](#apidoc.element.node-forge.util.xorBytes)
- description and source-code
```javascript
xorBytes = function (s1, s2, n) {
  var s3 = '';
  var b = '';
  var t = '';
  var i = 0;
  var c = 0;
  for(; n > 0; --n, ++i) {
    b = s1.charCodeAt(i) ^ s2.charCodeAt(i);
    if(c >= 10) {
      s3 += t;
      t = '';
      c = 0;
    }
    t += String.fromCharCode(b);
    ++c;
  }
  s3 += t;
  return s3;
}
```
- example usage
```shell
...

      // PRF(P, u_{c-1}) (other iterations)
      for(var j = 2; j <= c; ++j) {
prf.start(null, null);
prf.update(u_c1);
u_c = prf.digest().getBytes();
// F(p, s, c, i)
xor = forge.util.xorBytes(xor, u_c, hLen);
u_c1 = u_c;
      }

      /* 4. Concatenate the blocks and extract the first dkLen octets to
produce a derived key DK:

DK = T_1 || T_2 ||  ...  || T_len<0..r-1> */
...
```



# <a name="apidoc.module.node-forge.util.ByteBuffer"></a>[module node-forge.util.ByteBuffer](#apidoc.module.node-forge.util.ByteBuffer)

#### <a name="apidoc.element.node-forge.util.ByteBuffer.ByteBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>ByteBuffer (b)](#apidoc.element.node-forge.util.ByteBuffer.ByteBuffer)
- description and source-code
```javascript
function ByteStringBuffer(b) {
  // TODO: update to match DataBuffer API

  // the data in this buffer
  this.data = '';
  // the pointer for reading from this buffer
  this.read = 0;

  if(typeof b === 'string') {
    this.data = b;
  } else if(util.isArrayBuffer(b) || util.isArrayBufferView(b)) {
    // convert native buffer to forge buffer
    // FIXME: support native buffers internally instead
    var arr = new Uint8Array(b);
    try {
      this.data = String.fromCharCode.apply(null, arr);
    } catch(e) {
      for(var i = 0; i < arr.length; ++i) {
        this.putByte(arr[i]);
      }
    }
  } else if(b instanceof ByteStringBuffer ||
    (typeof b === 'object' && typeof b.data === 'string' &&
    typeof b.read === 'number')) {
    // copy existing buffer
    this.data = b.data;
    this.read = b.read;
  }

  // used for v8 optimization
  this._constructedStringLength = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.util.ByteBuffer.prototype"></a>[module node-forge.util.ByteBuffer.prototype](#apidoc.module.node-forge.util.ByteBuffer.prototype)

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype._optimizeConstructedString"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>_optimizeConstructedString (x)](#apidoc.element.node-forge.util.ByteBuffer.prototype._optimizeConstructedString)
- description and source-code
```javascript
_optimizeConstructedString = function (x) {
  this._constructedStringLength += x;
  if(this._constructedStringLength > _MAX_CONSTRUCTED_STRING_LENGTH) {
    // this substr() should cause the constructed string to join
    this.data.substr(0, 1);
    this._constructedStringLength = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.at"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>at (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.at)
- description and source-code
```javascript
at = function (i) {
  return this.data.charCodeAt(this.read + i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.bytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>bytes (count)](#apidoc.element.node-forge.util.ByteBuffer.prototype.bytes)
- description and source-code
```javascript
bytes = function (count) {
  return (typeof(count) === 'undefined' ?
    this.data.slice(this.read) :
    this.data.slice(this.read, this.read + count));
}
```
- example usage
```shell
...
// (defaults to RSASSA PKCS#1 v1.5)
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
var signature = privateKey.sign(md);

// verify data with a public key
// (defaults to RSASSA PKCS#1 v1.5)
var verified = publicKey.verify(md.digest().bytes(), signature);

// sign data using RSASSA-PSS where PSS uses a SHA-1 hash, a SHA-1 based
// masking function MGF1, and a 20 byte salt
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
var pss = forge.pss.create({
md: forge.md.sha1.create(),
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.clear"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>clear ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.clear)
- description and source-code
```javascript
clear = function () {
  this.data = '';
  this.read = 0;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.compact"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>compact ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.compact)
- description and source-code
```javascript
compact = function () {
  if(this.read > 0) {
    this.data = this.data.slice(this.read);
    this.read = 0;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.copy"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>copy ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.copy)
- description and source-code
```javascript
copy = function () {
  var c = util.createBuffer(this.data);
  c.read = this.read;
  return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.fillWithByte"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>fillWithByte (b, n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.fillWithByte)
- description and source-code
```javascript
fillWithByte = function (b, n) {
  b = String.fromCharCode(b);
  var d = this.data;
  while(n > 0) {
    if(n & 1) {
      d += b;
    }
    n >>>= 1;
    if(n > 0) {
      b += b;
    }
  }
  this.data = d;
  this._optimizeConstructedString(n);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getByte"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getByte ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getByte)
- description and source-code
```javascript
getByte = function () {
  return this.data.charCodeAt(this.read++);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getBytes (count)](#apidoc.element.node-forge.util.ByteBuffer.prototype.getBytes)
- description and source-code
```javascript
getBytes = function (count) {
  var rval;
  if(count) {
    // read count bytes
    count = Math.min(this.length(), count);
    rval = this.data.slice(this.read, this.read + count);
    this.read += count;
  } else if(count === 0) {
    rval = '';
  } else {
    // read all bytes, optimize to only copy when needed
    rval = (this.read === 0) ? this.data : this.data.slice(this.read);
    this.clear();
  }
  return rval;
}
```
- example usage
```shell
...
},
/* the private key for the client-side cert if provided */
getPrivateKey: function(connection, cert) {
  return myClientPrivateKey;
},
tlsDataReady: function(connection) {
  // TLS data (encrypted) is ready to be sent to the server
  sendToServerSomehow(connection.tlsData.getBytes());
  // if you were communicating with the server below, you'd do:
  // server.process(connection.tlsData.getBytes());
},
dataReady: function(connection) {
  // clear data from the server is ready
  console.log('the server sent: ' +
    forge.util.decodeUtf8(connection.data.getBytes()));
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt (n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt)
- description and source-code
```javascript
getInt = function (n) {
  _checkBitsParam(n);
  var rval = 0;
  do {
    // TODO: Use (rval * 0x100) if adding support for 33 to 53 bits.
    rval = (rval << 8) + this.data.charCodeAt(this.read++);
    n -= 8;
  } while(n > 0);
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt16"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt16 ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt16)
- description and source-code
```javascript
getInt16 = function () {
  var rval = (
    this.data.charCodeAt(this.read) << 8 ^
    this.data.charCodeAt(this.read + 1));
  this.read += 2;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt16Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt16Le ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt16Le)
- description and source-code
```javascript
getInt16Le = function () {
  var rval = (
    this.data.charCodeAt(this.read) ^
    this.data.charCodeAt(this.read + 1) << 8);
  this.read += 2;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt24"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt24 ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt24)
- description and source-code
```javascript
getInt24 = function () {
  var rval = (
    this.data.charCodeAt(this.read) << 16 ^
    this.data.charCodeAt(this.read + 1) << 8 ^
    this.data.charCodeAt(this.read + 2));
  this.read += 3;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt24Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt24Le ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt24Le)
- description and source-code
```javascript
getInt24Le = function () {
  var rval = (
    this.data.charCodeAt(this.read) ^
    this.data.charCodeAt(this.read + 1) << 8 ^
    this.data.charCodeAt(this.read + 2) << 16);
  this.read += 3;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt32"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt32 ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt32)
- description and source-code
```javascript
getInt32 = function () {
  var rval = (
    this.data.charCodeAt(this.read) << 24 ^
    this.data.charCodeAt(this.read + 1) << 16 ^
    this.data.charCodeAt(this.read + 2) << 8 ^
    this.data.charCodeAt(this.read + 3));
  this.read += 4;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getInt32Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getInt32Le ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.getInt32Le)
- description and source-code
```javascript
getInt32Le = function () {
  var rval = (
    this.data.charCodeAt(this.read) ^
    this.data.charCodeAt(this.read + 1) << 8 ^
    this.data.charCodeAt(this.read + 2) << 16 ^
    this.data.charCodeAt(this.read + 3) << 24);
  this.read += 4;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.getSignedInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>getSignedInt (n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.getSignedInt)
- description and source-code
```javascript
getSignedInt = function (n) {
  // getInt checks n
  var x = this.getInt(n);
  var max = 2 << (n - 2);
  if(x >= max) {
    x -= max << 1;
  }
  return x;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>isEmpty ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return this.length() <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.last"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>last ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.last)
- description and source-code
```javascript
last = function () {
  return this.data.charCodeAt(this.data.length - 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.length"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>length ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.length)
- description and source-code
```javascript
length = function () {
  return this.data.length - this.read;
}
```
- example usage
```shell
...
var buffer = forge.util.createBuffer();
// create a byte buffer from raw binary bytes
var buffer = forge.util.createBuffer(input, 'raw');
// create a byte buffer from utf8 bytes
var buffer = forge.util.createBuffer(input, 'utf8');

// get the length of the buffer in bytes
buffer.length();
// put bytes into the buffer
buffer.putBytes(bytes);
// put a 32-bit integer into the buffer
buffer.putInt32(10);
// buffer to hex
buffer.toHex();
// get a copy of the bytes in the buffer
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putBuffer (buffer)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putBuffer)
- description and source-code
```javascript
putBuffer = function (buffer) {
  return this.putBytes(buffer.getBytes());
}
```
- example usage
```shell
...
var output = forge.util.createBuffer();

// if using a salt, prepend this to the output:
if(salt !== null) {
  output.putBytes('Salted__'); // (add to match openssl tool output)
  output.putBytes(salt);
}
output.putBuffer(cipher.output);

fs.writeFileSync('input.enc', output.getBytes(), {encoding: 'binary'});
}

// openssl enc -d -des3 -in input.enc -out input.dec.txt
function decrypt(password) {
var input = fs.readFileSync('input.enc', {encoding: 'binary'});
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putByte"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putByte (b)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putByte)
- description and source-code
```javascript
putByte = function (b) {
  return this.putBytes(String.fromCharCode(b));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putBytes (bytes)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putBytes)
- description and source-code
```javascript
putBytes = function (bytes) {
  this.data += bytes;
  this._optimizeConstructedString(bytes.length);
  return this;
}
```
- example usage
```shell
...
sendSomehow(request.toString());

// receive response
var buffer = forge.util.createBuffer();
var response = forge.http.createResponse();
var someAsyncDataHandler = function(bytes) {
if(!response.bodyReceived) {
  buffer.putBytes(bytes);
  if(!response.headerReceived) {
    if(response.readHeader(buffer)) {
      console.log('HTTP response header: ' + response.toString());
    }
  }
  if(response.headerReceived && !response.bodyReceived) {
    if(response.readBody(buffer)) {
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt (i, n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt)
- description and source-code
```javascript
putInt = function (i, n) {
  _checkBitsParam(n);
  var bytes = '';
  do {
    n -= 8;
    bytes += String.fromCharCode((i >> n) & 0xFF);
  } while(n > 0);
  return this.putBytes(bytes);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt16"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt16 (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt16)
- description and source-code
```javascript
putInt16 = function (i) {
  return this.putBytes(
    String.fromCharCode(i >> 8 & 0xFF) +
    String.fromCharCode(i & 0xFF));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt16Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt16Le (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt16Le)
- description and source-code
```javascript
putInt16Le = function (i) {
  return this.putBytes(
    String.fromCharCode(i & 0xFF) +
    String.fromCharCode(i >> 8 & 0xFF));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt24"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt24 (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt24)
- description and source-code
```javascript
putInt24 = function (i) {
  return this.putBytes(
    String.fromCharCode(i >> 16 & 0xFF) +
    String.fromCharCode(i >> 8 & 0xFF) +
    String.fromCharCode(i & 0xFF));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt24Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt24Le (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt24Le)
- description and source-code
```javascript
putInt24Le = function (i) {
  return this.putBytes(
    String.fromCharCode(i & 0xFF) +
    String.fromCharCode(i >> 8 & 0xFF) +
    String.fromCharCode(i >> 16 & 0xFF));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt32"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt32 (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt32)
- description and source-code
```javascript
putInt32 = function (i) {
  return this.putBytes(
    String.fromCharCode(i >> 24 & 0xFF) +
    String.fromCharCode(i >> 16 & 0xFF) +
    String.fromCharCode(i >> 8 & 0xFF) +
    String.fromCharCode(i & 0xFF));
}
```
- example usage
```shell
...
var buffer = forge.util.createBuffer(input, 'utf8');

// get the length of the buffer in bytes
buffer.length();
// put bytes into the buffer
buffer.putBytes(bytes);
// put a 32-bit integer into the buffer
buffer.putInt32(10);
// buffer to hex
buffer.toHex();
// get a copy of the bytes in the buffer
bytes.bytes(/* count */);
// empty this buffer and get its contents
bytes.getBytes(/* count */);
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putInt32Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putInt32Le (i)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putInt32Le)
- description and source-code
```javascript
putInt32Le = function (i) {
  return this.putBytes(
    String.fromCharCode(i & 0xFF) +
    String.fromCharCode(i >> 8 & 0xFF) +
    String.fromCharCode(i >> 16 & 0xFF) +
    String.fromCharCode(i >> 24 & 0xFF));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putSignedInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putSignedInt (i, n)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putSignedInt)
- description and source-code
```javascript
putSignedInt = function (i, n) {
  // putInt checks n
  if(i < 0) {
    i += 2 << (n - 1);
  }
  return this.putInt(i, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.putString"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>putString (str)](#apidoc.element.node-forge.util.ByteBuffer.prototype.putString)
- description and source-code
```javascript
putString = function (str) {
  return this.putBytes(util.encodeUtf8(str));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.setAt"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>setAt (i, b)](#apidoc.element.node-forge.util.ByteBuffer.prototype.setAt)
- description and source-code
```javascript
setAt = function (i, b) {
  this.data = this.data.substr(0, this.read + i) +
    String.fromCharCode(b) +
    this.data.substr(this.read + i + 1);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.toHex"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>toHex ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.toHex)
- description and source-code
```javascript
toHex = function () {
  var rval = '';
  for(var i = this.read; i < this.data.length; ++i) {
    var b = this.data.charCodeAt(i);
    if(b < 16) {
      rval += '0';
    }
    rval += b.toString(16);
  }
  return rval;
}
```
- example usage
```shell
...
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
// (other modes include: CFB, OFB, CTR, and GCM)
var decipher = forge.cipher.createDecipher('AES-CBC', key);
decipher.start({iv: iv});
decipher.update(encrypted);
decipher.finish();
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.toString"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>toString ()](#apidoc.element.node-forge.util.ByteBuffer.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return util.decodeUtf8(this.bytes());
}
```
- example usage
```shell
...
});

socket.on('connect', function() {
  console.log('[socket] connected');
  client.handshake();
});
socket.on('data', function(data) {
  client.process(data.toString('binary')); // encoding should be 'binary'
});
socket.on('end', function() {
  console.log('[socket] disconnected');
});

// connect to google.com
socket.connect(443, 'google.com');
...
```

#### <a name="apidoc.element.node-forge.util.ByteBuffer.prototype.truncate"></a>[function <span class="apidocSignatureSpan">node-forge.util.ByteBuffer.prototype.</span>truncate (count)](#apidoc.element.node-forge.util.ByteBuffer.prototype.truncate)
- description and source-code
```javascript
truncate = function (count) {
  var len = Math.max(0, this.length() - count);
  this.data = this.data.substr(this.read, len);
  this.read = 0;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.util.DataBuffer"></a>[module node-forge.util.DataBuffer](#apidoc.module.node-forge.util.DataBuffer)

#### <a name="apidoc.element.node-forge.util.DataBuffer.DataBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.</span>DataBuffer (b, options)](#apidoc.element.node-forge.util.DataBuffer.DataBuffer)
- description and source-code
```javascript
function DataBuffer(b, options) {
  // default options
  options = options || {};

  // pointers for read from/write to buffer
  this.read = options.readOffset || 0;
  this.growSize = options.growSize || 1024;

  var isArrayBuffer = util.isArrayBuffer(b);
  var isArrayBufferView = util.isArrayBufferView(b);
  if(isArrayBuffer || isArrayBufferView) {
    // use ArrayBuffer directly
    if(isArrayBuffer) {
      this.data = new DataView(b);
    } else {
      // TODO: adjust read/write offset based on the type of view
      // or specify that this must be done in the options ... that the
      // offsets are byte-based
      this.data = new DataView(b.buffer, b.byteOffset, b.byteLength);
    }
    this.write = ('writeOffset' in options ?
      options.writeOffset : this.data.byteLength);
    return;
  }

  // initialize to empty array buffer and add any given bytes using putBytes
  this.data = new DataView(new ArrayBuffer(0));
  this.write = 0;

  if(b !== null && b !== undefined) {
    this.putBytes(b);
  }

  if('writeOffset' in options) {
    this.write = options.writeOffset;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-forge.util.DataBuffer.prototype"></a>[module node-forge.util.DataBuffer.prototype](#apidoc.module.node-forge.util.DataBuffer.prototype)

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.accommodate"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>accommodate (amount, growSize)](#apidoc.element.node-forge.util.DataBuffer.prototype.accommodate)
- description and source-code
```javascript
accommodate = function (amount, growSize) {
  if(this.length() >= amount) {
    return this;
  }
  growSize = Math.max(growSize || this.growSize, amount);

  // grow buffer
  var src = new Uint8Array(
    this.data.buffer, this.data.byteOffset, this.data.byteLength);
  var dst = new Uint8Array(this.length() + growSize);
  dst.set(src);
  this.data = new DataView(dst.buffer);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.at"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>at (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.at)
- description and source-code
```javascript
at = function (i) {
  return this.data.getUint8(this.read + i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.bytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>bytes (count)](#apidoc.element.node-forge.util.DataBuffer.prototype.bytes)
- description and source-code
```javascript
bytes = function (count) {
  // TODO: deprecate this method, it is poorly named, add "getString()"
  return (typeof(count) === 'undefined' ?
    this.data.slice(this.read) :
    this.data.slice(this.read, this.read + count));
}
```
- example usage
```shell
...
// (defaults to RSASSA PKCS#1 v1.5)
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
var signature = privateKey.sign(md);

// verify data with a public key
// (defaults to RSASSA PKCS#1 v1.5)
var verified = publicKey.verify(md.digest().bytes(), signature);

// sign data using RSASSA-PSS where PSS uses a SHA-1 hash, a SHA-1 based
// masking function MGF1, and a 20 byte salt
var md = forge.md.sha1.create();
md.update('sign this', 'utf8');
var pss = forge.pss.create({
md: forge.md.sha1.create(),
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.clear"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>clear ()](#apidoc.element.node-forge.util.DataBuffer.prototype.clear)
- description and source-code
```javascript
clear = function () {
  this.data = new DataView(new ArrayBuffer(0));
  this.read = this.write = 0;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.compact"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>compact ()](#apidoc.element.node-forge.util.DataBuffer.prototype.compact)
- description and source-code
```javascript
compact = function () {
  if(this.read > 0) {
    var src = new Uint8Array(this.data.buffer, this.read);
    var dst = new Uint8Array(src.byteLength);
    dst.set(src);
    this.data = new DataView(dst);
    this.write -= this.read;
    this.read = 0;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.copy"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>copy ()](#apidoc.element.node-forge.util.DataBuffer.prototype.copy)
- description and source-code
```javascript
copy = function () {
  return new util.DataBuffer(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.fillWithByte"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>fillWithByte (b, n)](#apidoc.element.node-forge.util.DataBuffer.prototype.fillWithByte)
- description and source-code
```javascript
fillWithByte = function (b, n) {
  this.accommodate(n);
  for(var i = 0; i < n; ++i) {
    this.data.setUint8(b);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getByte"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getByte ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getByte)
- description and source-code
```javascript
getByte = function () {
  return this.data.getInt8(this.read++);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getBytes (count)](#apidoc.element.node-forge.util.DataBuffer.prototype.getBytes)
- description and source-code
```javascript
getBytes = function (count) {
  // TODO: deprecate this method, it is poorly named and
  // this.toString('binary') replaces it
  // add a toTypedArray()/toArrayBuffer() function
  var rval;
  if(count) {
    // read count bytes
    count = Math.min(this.length(), count);
    rval = this.data.slice(this.read, this.read + count);
    this.read += count;
  } else if(count === 0) {
    rval = '';
  } else {
    // read all bytes, optimize to only copy when needed
    rval = (this.read === 0) ? this.data : this.data.slice(this.read);
    this.clear();
  }
  return rval;
}
```
- example usage
```shell
...
},
/* the private key for the client-side cert if provided */
getPrivateKey: function(connection, cert) {
  return myClientPrivateKey;
},
tlsDataReady: function(connection) {
  // TLS data (encrypted) is ready to be sent to the server
  sendToServerSomehow(connection.tlsData.getBytes());
  // if you were communicating with the server below, you'd do:
  // server.process(connection.tlsData.getBytes());
},
dataReady: function(connection) {
  // clear data from the server is ready
  console.log('the server sent: ' +
    forge.util.decodeUtf8(connection.data.getBytes()));
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt (n)](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt)
- description and source-code
```javascript
getInt = function (n) {
  _checkBitsParam(n);
  var rval = 0;
  do {
    // TODO: Use (rval * 0x100) if adding support for 33 to 53 bits.
    rval = (rval << 8) + this.data.getInt8(this.read++);
    n -= 8;
  } while(n > 0);
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt16"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt16 ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt16)
- description and source-code
```javascript
getInt16 = function () {
  var rval = this.data.getInt16(this.read);
  this.read += 2;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt16Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt16Le ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt16Le)
- description and source-code
```javascript
getInt16Le = function () {
  var rval = this.data.getInt16(this.read, true);
  this.read += 2;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt24"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt24 ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt24)
- description and source-code
```javascript
getInt24 = function () {
  var rval = (
    this.data.getInt16(this.read) << 8 ^
    this.data.getInt8(this.read + 2));
  this.read += 3;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt24Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt24Le ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt24Le)
- description and source-code
```javascript
getInt24Le = function () {
  var rval = (
    this.data.getInt8(this.read) ^
    this.data.getInt16(this.read + 1, true) << 8);
  this.read += 3;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt32"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt32 ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt32)
- description and source-code
```javascript
getInt32 = function () {
  var rval = this.data.getInt32(this.read);
  this.read += 4;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getInt32Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getInt32Le ()](#apidoc.element.node-forge.util.DataBuffer.prototype.getInt32Le)
- description and source-code
```javascript
getInt32Le = function () {
  var rval = this.data.getInt32(this.read, true);
  this.read += 4;
  return rval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.getSignedInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>getSignedInt (n)](#apidoc.element.node-forge.util.DataBuffer.prototype.getSignedInt)
- description and source-code
```javascript
getSignedInt = function (n) {
  // getInt checks n
  var x = this.getInt(n);
  var max = 2 << (n - 2);
  if(x >= max) {
    x -= max << 1;
  }
  return x;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>isEmpty ()](#apidoc.element.node-forge.util.DataBuffer.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return this.length() <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.last"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>last ()](#apidoc.element.node-forge.util.DataBuffer.prototype.last)
- description and source-code
```javascript
last = function () {
  return this.data.getUint8(this.write - 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.length"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>length ()](#apidoc.element.node-forge.util.DataBuffer.prototype.length)
- description and source-code
```javascript
length = function () {
  return this.write - this.read;
}
```
- example usage
```shell
...
var buffer = forge.util.createBuffer();
// create a byte buffer from raw binary bytes
var buffer = forge.util.createBuffer(input, 'raw');
// create a byte buffer from utf8 bytes
var buffer = forge.util.createBuffer(input, 'utf8');

// get the length of the buffer in bytes
buffer.length();
// put bytes into the buffer
buffer.putBytes(bytes);
// put a 32-bit integer into the buffer
buffer.putInt32(10);
// buffer to hex
buffer.toHex();
// get a copy of the bytes in the buffer
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putBuffer"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putBuffer (buffer)](#apidoc.element.node-forge.util.DataBuffer.prototype.putBuffer)
- description and source-code
```javascript
putBuffer = function (buffer) {
  this.putBytes(buffer);
  buffer.clear();
  return this;
}
```
- example usage
```shell
...
var output = forge.util.createBuffer();

// if using a salt, prepend this to the output:
if(salt !== null) {
  output.putBytes('Salted__'); // (add to match openssl tool output)
  output.putBytes(salt);
}
output.putBuffer(cipher.output);

fs.writeFileSync('input.enc', output.getBytes(), {encoding: 'binary'});
}

// openssl enc -d -des3 -in input.enc -out input.dec.txt
function decrypt(password) {
var input = fs.readFileSync('input.enc', {encoding: 'binary'});
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putByte"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putByte (b)](#apidoc.element.node-forge.util.DataBuffer.prototype.putByte)
- description and source-code
```javascript
putByte = function (b) {
  this.accommodate(1);
  this.data.setUint8(this.write++, b);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putBytes"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putBytes (bytes, encoding)](#apidoc.element.node-forge.util.DataBuffer.prototype.putBytes)
- description and source-code
```javascript
putBytes = function (bytes, encoding) {
  if(util.isArrayBufferView(bytes)) {
    var src = new Uint8Array(bytes.buffer, bytes.byteOffset, bytes.byteLength);
    var len = src.byteLength - src.byteOffset;
    this.accommodate(len);
    var dst = new Uint8Array(this.data.buffer, this.write);
    dst.set(src);
    this.write += len;
    return this;
  }

  if(util.isArrayBuffer(bytes)) {
    var src = new Uint8Array(bytes);
    this.accommodate(src.byteLength);
    var dst = new Uint8Array(this.data.buffer);
    dst.set(src, this.write);
    this.write += src.byteLength;
    return this;
  }

  // bytes is a util.DataBuffer or equivalent
  if(bytes instanceof util.DataBuffer ||
    (typeof bytes === 'object' &&
    typeof bytes.read === 'number' && typeof bytes.write === 'number' &&
    util.isArrayBufferView(bytes.data))) {
    var src = new Uint8Array(bytes.data.byteLength, bytes.read, bytes.length());
    this.accommodate(src.byteLength);
    var dst = new Uint8Array(bytes.data.byteLength, this.write);
    dst.set(src);
    this.write += src.byteLength;
    return this;
  }

  if(bytes instanceof util.ByteStringBuffer) {
    // copy binary string and process as the same as a string parameter below
    bytes = bytes.data;
    encoding = 'binary';
  }

  // string conversion
  encoding = encoding || 'binary';
  if(typeof bytes === 'string') {
    var view;

    // decode from string
    if(encoding === 'hex') {
      this.accommodate(Math.ceil(bytes.length / 2));
      view = new Uint8Array(this.data.buffer, this.write);
      this.write += util.binary.hex.decode(bytes, view, this.write);
      return this;
    }
    if(encoding === 'base64') {
      this.accommodate(Math.ceil(bytes.length / 4) * 3);
      view = new Uint8Array(this.data.buffer, this.write);
      this.write += util.binary.base64.decode(bytes, view, this.write);
      return this;
    }

    // encode text as UTF-8 bytes
    if(encoding === 'utf8') {
      // encode as UTF-8 then decode string as raw binary
      bytes = util.encodeUtf8(bytes);
      encoding = 'binary';
    }

    // decode string as raw binary
    if(encoding === 'binary' || encoding === 'raw') {
      // one byte per character
      this.accommodate(bytes.length);
      view = new Uint8Array(this.data.buffer, this.write);
      this.write += util.binary.raw.decode(view);
      return this;
    }

    // encode text as UTF-16 bytes
    if(encoding === 'utf16') {
      // two bytes per character
      this.accommodate(bytes.length * 2);
      view = new Uint16Array(this.data.buffer, this.write);
      this.write += util.text.utf16.encode(view);
      return this;
    }

    throw new Error('Invalid encoding: ' + encoding);
  }

  throw Error('Invalid parameter: ' + bytes);
}
```
- example usage
```shell
...
sendSomehow(request.toString());

// receive response
var buffer = forge.util.createBuffer();
var response = forge.http.createResponse();
var someAsyncDataHandler = function(bytes) {
if(!response.bodyReceived) {
  buffer.putBytes(bytes);
  if(!response.headerReceived) {
    if(response.readHeader(buffer)) {
      console.log('HTTP response header: ' + response.toString());
    }
  }
  if(response.headerReceived && !response.bodyReceived) {
    if(response.readBody(buffer)) {
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt (i, n)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt)
- description and source-code
```javascript
putInt = function (i, n) {
  _checkBitsParam(n);
  this.accommodate(n / 8);
  do {
    n -= 8;
    this.data.setInt8(this.write++, (i >> n) & 0xFF);
  } while(n > 0);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt16"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt16 (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt16)
- description and source-code
```javascript
putInt16 = function (i) {
  this.accommodate(2);
  this.data.setInt16(this.write, i);
  this.write += 2;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt16Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt16Le (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt16Le)
- description and source-code
```javascript
putInt16Le = function (i) {
  this.accommodate(2);
  this.data.setInt16(this.write, i, true);
  this.write += 2;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt24"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt24 (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt24)
- description and source-code
```javascript
putInt24 = function (i) {
  this.accommodate(3);
  this.data.setInt16(this.write, i >> 8 & 0xFFFF);
  this.data.setInt8(this.write, i >> 16 & 0xFF);
  this.write += 3;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt24Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt24Le (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt24Le)
- description and source-code
```javascript
putInt24Le = function (i) {
  this.accommodate(3);
  this.data.setInt8(this.write, i >> 16 & 0xFF);
  this.data.setInt16(this.write, i >> 8 & 0xFFFF, true);
  this.write += 3;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt32"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt32 (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt32)
- description and source-code
```javascript
putInt32 = function (i) {
  this.accommodate(4);
  this.data.setInt32(this.write, i);
  this.write += 4;
  return this;
}
```
- example usage
```shell
...
var buffer = forge.util.createBuffer(input, 'utf8');

// get the length of the buffer in bytes
buffer.length();
// put bytes into the buffer
buffer.putBytes(bytes);
// put a 32-bit integer into the buffer
buffer.putInt32(10);
// buffer to hex
buffer.toHex();
// get a copy of the bytes in the buffer
bytes.bytes(/* count */);
// empty this buffer and get its contents
bytes.getBytes(/* count */);
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putInt32Le"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putInt32Le (i)](#apidoc.element.node-forge.util.DataBuffer.prototype.putInt32Le)
- description and source-code
```javascript
putInt32Le = function (i) {
  this.accommodate(4);
  this.data.setInt32(this.write, i, true);
  this.write += 4;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putSignedInt"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putSignedInt (i, n)](#apidoc.element.node-forge.util.DataBuffer.prototype.putSignedInt)
- description and source-code
```javascript
putSignedInt = function (i, n) {
  _checkBitsParam(n);
  this.accommodate(n / 8);
  if(i < 0) {
    i += 2 << (n - 1);
  }
  return this.putInt(i, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.putString"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>putString (str)](#apidoc.element.node-forge.util.DataBuffer.prototype.putString)
- description and source-code
```javascript
putString = function (str) {
  return this.putBytes(str, 'utf16');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.setAt"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>setAt (i, b)](#apidoc.element.node-forge.util.DataBuffer.prototype.setAt)
- description and source-code
```javascript
setAt = function (i, b) {
  this.data.setUint8(i, b);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.toHex"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>toHex ()](#apidoc.element.node-forge.util.DataBuffer.prototype.toHex)
- description and source-code
```javascript
toHex = function () {
  var rval = '';
  for(var i = this.read; i < this.data.byteLength; ++i) {
    var b = this.data.getUint8(i);
    if(b < 16) {
      rval += '0';
    }
    rval += b.toString(16);
  }
  return rval;
}
```
- example usage
```shell
...
// Note: CBC and ECB modes use PKCS#7 padding as default
var cipher = forge.cipher.createCipher('AES-CBC', key);
cipher.start({iv: iv});
cipher.update(forge.util.createBuffer(someBytes));
cipher.finish();
var encrypted = cipher.output;
// outputs encrypted hex
console.log(encrypted.toHex());

// decrypt some bytes using CBC mode
// (other modes include: CFB, OFB, CTR, and GCM)
var decipher = forge.cipher.createDecipher('AES-CBC', key);
decipher.start({iv: iv});
decipher.update(encrypted);
decipher.finish();
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.toString"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>toString (encoding)](#apidoc.element.node-forge.util.DataBuffer.prototype.toString)
- description and source-code
```javascript
toString = function (encoding) {
  var view = new Uint8Array(this.data, this.read, this.length());
  encoding = encoding || 'utf8';

  // encode to string
  if(encoding === 'binary' || encoding === 'raw') {
    return util.binary.raw.encode(view);
  }
  if(encoding === 'hex') {
    return util.binary.hex.encode(view);
  }
  if(encoding === 'base64') {
    return util.binary.base64.encode(view);
  }

  // decode to text
  if(encoding === 'utf8') {
    return util.text.utf8.decode(view);
  }
  if(encoding === 'utf16') {
    return util.text.utf16.decode(view);
  }

  throw new Error('Invalid encoding: ' + encoding);
}
```
- example usage
```shell
...
});

socket.on('connect', function() {
  console.log('[socket] connected');
  client.handshake();
});
socket.on('data', function(data) {
  client.process(data.toString('binary')); // encoding should be 'binary'
});
socket.on('end', function() {
  console.log('[socket] disconnected');
});

// connect to google.com
socket.connect(443, 'google.com');
...
```

#### <a name="apidoc.element.node-forge.util.DataBuffer.prototype.truncate"></a>[function <span class="apidocSignatureSpan">node-forge.util.DataBuffer.prototype.</span>truncate (count)](#apidoc.element.node-forge.util.DataBuffer.prototype.truncate)
- description and source-code
```javascript
truncate = function (count) {
  this.write = Math.max(0, this.length() - count);
  this.read = Math.min(this.read, this.write);
  return this;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
