# pFlow-dev
Tools to build and use petri-net models in go, js, python, lua, solidity

- https://pflow.dev/p/ - model editor
- https://pflow.dev/sandbox/ - javascript sandbox
- WIP: web3 support in solidity + ipfs

  <img width="991" alt="Screenshot 2023-12-20 at 6 32 57 PM" src="https://github.com/pFlow-dev/.github/assets/243500/04be1793-f86d-4ff0-bcb4-5830e8891de6">


## Reference Specification
* [pflow-js](https://github.com/pFlow-dev/pflow-js) - a javascript library
  * usable from the browser
  * considered to the *reference implementation*
   
* [metamodel-js](https://github.com/pFlow-dev/metamodel-js) - a typescript library
  * usable from npm
  * conforms to the reference implementation

## Current Focus

Advance the state of solidty smart contract development by
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

