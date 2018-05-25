ltc BIP39 Mnemonics
=======

[![NPM Package](https://img.shields.io/npm/v/ltc-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/ltc-mnemonic)
[![Build Status](https://img.shields.io/travis/owstack/ltc-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/owstack/ltc-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/owstack/ltc-mnemonic.svg?style=flat-square)](https://coveralls.io/r/owstack/ltc-mnemonic)

A module for [owstack](http://owstack.org) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install @owstack/ltc-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://ltc.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('@owstack/ltc-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/owstack/ltc-mnemonic/blob/master/CONTRIBUTING.md) on the main ltc repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/owstack/ltc-mnemonic/blob/master/LICENSE).

Copyright 2017 Open Wallet Stack.
