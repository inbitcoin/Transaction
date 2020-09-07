# Colored Coins Transaction

> Colored Coins Transaction provides the basic functionality for creating and managing a Colored Coins Transaction Object

### Installation

```sh
$ npm install cc-transaction
```

### properties

```js
// which type is the transaction ('issue'/'send'/'burn') [String]
this.type
// [Boolean]
this.noRules
// transfer objects to pass assets from inputs to outputs [Array[Object]] 
this.payments
// [Number]
this.protocol
// Colored-Coins protocol version [Number]
this.version
// how many places after the decimal point can the smallest asset amount be (for example divisibility 2 => smallest asset amount is 0.01) [Number]
this.divisibility
// is an issued asset locked or can it be re-issued [Boolean]
this.lockStatus
// amount of units of an asset to issue [Number]
this.amount
// SHA2 of the metadata [Buffer]
this.sha2
// the torrent hash of the metadata torrent [Buffer]
this.torrentHash
// list of objects which indicate how a multisig stores the hashes (index and type) [Array[Object]]
this.multiSig
```

### Testing

In order to test you need to install [mocha] globaly on your machine

```sh
$ cd /"module-path"/cc-transaction
$ mocha
```


### License

This software is licensed under the Apache License, Version 2.0.
See [LICENSE](LICENSE) for the full license text.


[mocha]:https://www.npmjs.com/package/mocha
