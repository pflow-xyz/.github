# pFlow-dev

Turning static diagrams into dynamic narratives of change.

## Tools

We provide tools to build and use Petri-net models in go, js, python, lua, solidity

- https://pflow.dev/p/ - model editor: build Petri-nets in the browser
- https://pflow.dev/sandbox/ - javascript sandbox: edit Petri-nets as javascript
- WIP: pflow.eth web3 support in solidity - compose contracts with petri-nets

[![pflow](https://pflow.dev/img/zb2rhgQVj436skxwVfhjkoX2E8tHbuwvU3HHY5quYcFKZb38y.svg)](https://pflow.dev/p/zb2rhgQVj436skxwVfhjkoX2E8tHbuwvU3HHY5quYcFKZb38y/)

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

