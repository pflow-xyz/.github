## Tools

We provide tools to build and use Petri-net models in go, js, python, lua, solidity, and rust

- https://pflow.dev/p/ - model editor: build Petri-nets in the browser
- https://pflow.dev/sandbox/ - javascript sandbox: edit Petri-nets as javascript
- WIP: pflow.eth web3 support in solidity - compose contracts with petri-nets


## Reference Specification
* [pflow-js](https://github.com/pFlow-dev/pflow-js) - a javascript library
  * usable from the browser
  * this project hosts the *reference implementation*
  * the repo also hosts a snapshot of the js tools [released via CDN](https://www.jsdelivr.com/package/gh/pflow-dev/pflow-js)
   
* [metamodel-js](https://github.com/pFlow-dev/metamodel-js) - a typescript library
  * usable from npm
  * conforms to the reference implementation

## Current Focus

Advance the state of solidity smart contract development by
providing a library that can be used to create petri-net based
smart contracts.

## Future Focus

Deploy a smart contract based registry that can be used to
store and retrieve petri-net based smart contracts.

## Why Petri Nets?

Petri nets are a well known and well studied formalism that
can be used to model a wide variety of systems.

Petri nets are a natural fit for model development
because they are:

* simple
* expressive
* composable
* verifiable

