# Awesome Ethereum Virtual Machine

A curated list of resources on the Ethereum Virtual Machine (EVM), which is the virtual machine executed on the [Ethereum](https://ethereum.org/) network.

Not listed there yet, but in the spirit of [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

Here is [how to contribute](./contributing.md).

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Specification](#specification)
- [Tests](#tests)
- [EVM Implementations](#evm-implementations)
- [Programming Languages that Compile into EVM](#programming-languages-that-compile-into-evm)
- [Debuggers](#debuggers)
- [Code Analyzers](#code-analyzers)
- [Improvement Proposals](#improvement-proposals)
- [Tutorials](#tutorials)
- [Related Resources](#related-resources)
- [License of This List](#license-of-this-list)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Specification

* [Yellow Paper](https://github.com/ethereum/yellowpaper)
    - A terse specification of EVM and Ethereum blocks

## Tests

* [Consensus test suite](https://github.com/ethereum/tests)
    - EVM implementations can be tested against this test suite

## EVM Implementations

* [go-ethereum](https://github.com/ethereum/go-ethereum)
    - A popular Ethereum client with its own EVM implementation
* [Parity](https://github.com/paritytech/parity) in Rust
    - Another popular Ethereum client with its own EVM implementation
* [cpp-ethereum](https://github.com/ethereum/cpp-ethereum)
    - An Ethereum client that generates the consensus test suite
* [Pyethereum](https://github.com/ethereum/pyethereum) in Python
    - Another client with probably the best readable EVM implementation
* [Py-EVM](https://github.com/pipermerriam/py-evm) in Python
    - An alternate Python implementation designed to be highly configurable and modular.
* [EthereumJ](https://github.com/ethereum/ethereumj) in Java
    - A client with its own EVM implementation
* [eth-isabelle](https://github.com/pirapira/eth-isabelle)
    - An EVM implementation for theorem provers
* [Modeling EVM in the K framework](https://github.com/kframework/evm-semantics)
    - An EVM implementation for [K framework](http://www.kframework.org/index.php/Main_Page)
* [hsevm](https://github.com/dapphub/hsevm)
    - An EVM implementation written in Haskell with debugging in mind

## Programming Languages that Compile into EVM

* [Solidity](https://github.com/ethereum/solidity)
    - The most popular programming language for Ethereum contracts
    - [Awesome Solidity](https://github.com/bkrem/awesome-solidity)
    - The LLL compiler is also in the same repository.
* [Viper](https://github.com/ethereum/viper)
    - A language with overflow-checking, numeric units but without unlimited loops
* [Serpent](https://github.com/ethereum/serpent)
    - A language that looks like Python

## Debuggers

* [REMIX](https://github.com/ethereum/remix)
    - An IDE containing an EVM code debugger
* [debug_traceTransaction method](https://github.com/ethereum/go-ethereum/wiki/Management-APIs#debug_tracetransaction)
    - An instruction-wise trace information provided by go-ethereum

## Code Analyzers

* [evmdis](https://github.com/arachnid/evmdis)
    - A disassembler for EVM code
* [Oyente](https://github.com/melonproject/oyente)
    - An automatic EVM code analyzer based on symbolic execution and [Z3](https://github.com/Z3Prover/z3) SMT solver
* [Dr. Y's Ethereum Contract Analyzer](http://dry.yoichihirai.com/)
    - A symbolic executor for EVM code

## Improvement Proposals

* [Ethereum Improvement Proposals](https://github.com/ethereum/EIPs)
    - A portal for EVM & Ethereum improvements
    - The most immediate changes are listed in the README
* [EVM 1.5](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-615.md)
    - A proposal to tame jumps so that a linear-time scan can determine stack layouts
* [eWASM](https://github.com/ewasm)
    - A proposal to use a [WebAssembly](http://webassembly.org/) for Ethereum contract execution

## Tutorials

## Related Resources

* [Awesome Ethereum](http://awesome-ethereum.com/)

## License of This List

Awesome Ethereum Virtual Machine

Written in 2017 by Yoichi Hirai <i@yoichihirai.com>

[other author/contributor lines as appropriate]

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
