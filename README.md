<img src="http://digicore.io/css/images/module-mnemonic.png" alt="digicore mnemonics" height="35">
BIP39 Mnemonics for digicore
=======

[![NPM Package](https://img.shields.io/npm/v/digicore-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/digicore-mnemonic)
[![Build Status](https://img.shields.io/travis/bitpay/digicore-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/digicore-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/bitpay/digicore-mnemonic.svg?style=flat-square)](https://coveralls.io/r/bitpay/digicore-mnemonic)

A module for [digicore](https://github.com/bitpay/digicore) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install digicore-mnemonic
bower install digicore-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://digicore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('digicore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/bitpay/digicore/blob/master/CONTRIBUTING.md) on the main digicore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/digicore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Digicore is a trademark maintained by BitPay, Inc.
