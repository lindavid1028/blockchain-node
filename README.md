
# blockchain-node

Blockchain.info Bitcoin Wrapper For Node.js

Wesite: https://blockchain.info

API documentation : https://blockchain.info/api/json_rpc_api

## Installation

  npm install blockchain-node --save

## Usage


**Require blockchain-node**

```
  var blockchain = require('blockchain-node');
```

**Instantiate**

```
	var bc = new blockchain({
      username: 'username',
      password: 'password'
  });
```

**Example Usage**

```
    // Get info
    bc.getInfo(function(err, info) {
        // info;
    });
```

```
  // Get balance
  bc.getBalance(function(err, balance) {
      // balance;
  });
```

## List of commands

```
getBalance =>             (confirmations : number, callback : function)

getInfo =>                (callback : function)

listAccounts =>           (callback : function)

getAddressesByAccount =>  (account : string, callback : function)

listReceivedByAccount =>  (account : string, callback : function)

listTransactions =>       (callback : function)

validateAddress =>        (address : string, callback : function)

getTransaction =>         (txid : string, callback : function)

getBlockCount =>          (callback : function)

getBlockHash =>           (index : number, callback : function)

getDifficulty =>          (callback : function)


**UNTESTED**

sendFrom =>               (to : string, from : string, amount : number, callback : function)

move =>                   (to : string, from : string, amount : number, callback : function)

```

## Tests

  npm test

## Contributing

Contact or fork.

Email : richardmacarthy@hotmail.com

Website : www.cryptogrind.com

## Release History

* 1.0.0 Initial release

* 1.0.5 New Methods

* 1.0.6 Some refactoring

## Issues

Add issue on github.