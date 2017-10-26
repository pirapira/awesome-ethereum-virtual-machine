# Awesome Ethereum Virtual Machine

A curated list of resources on the Ethereum Virtual Machine (EVM), which is the virtual machine executed on the [Ethereum](https://ethereum.org/) network.

Not listed there yet, but in the spirit of [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

Here is [how to contribute](./contributing.md).

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Specification](#specification)
- [Illustration](#illustration)
- [Tutorials](#tutorials)
- [Tests](#tests)
- [EVM Implementations](#evm-implementations)
- [Programming Languages that Compile into EVM](#programming-languages-that-compile-into-evm)
- [Debuggers](#debuggers)
- [Code Analyzers](#code-analyzers)
- [Improvement Proposals](#improvement-proposals)
- [Related Resources](#related-resources)
- [License of This List](#license-of-this-list)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Specification

* [Yellow Paper](https://github.com/ethereum/yellowpaper)
    - A terse specification of EVM and Ethereum blocks

## Illustration

* [A detailed illustration of the Ethereum Virtual Machine](https://ethereum.stackexchange.com/a/6413/280)
    - The illustration shows the contents of blocks and block headers faithfully

## Tutorials

* [CoinCulture's Guide to the EVM](https://github.com/CoinCulture/evm-tools/blob/master/analysis/guide.md)
    - A hands on guide to understanding how the EVM works, with examples written in raw byte-code and solidity
* [Diving Into The Ethereum Virtual Machine](https://medium.com/@hayeah/diving-into-the-ethereum-vm-6e8d5d2f3c30)
    - An article series examining different aspects of the EVM by walking you through Solidity's assembly output

## Tests

* [Consensus test suite](https://github.com/ethereum/tests)
    - EVM implementations can be tested against this test suite

## EVM Implementations

* [go-ethereum](https://github.com/ethereum/go-ethereum)
    - A popular Ethereum client with its own EVM implementation ([core/vm](https://github.com/ethereum/go-ethereum/tree/master/core/vm) directory)
* [Parity](https://github.com/paritytech/parity) in Rust
    - Another popular Ethereum client with its own EVM implementation ([ethcore](https://github.com/paritytech/parity/tree/master/ethcore) directory)
* [cpp-ethereum](https://github.com/ethereum/cpp-ethereum)
    - An Ethereum client that generates the consensus test suite ([libevm/VM.cpp](https://github.com/ethereum/cpp-ethereum/blob/develop/libevm/VM.cpp))
* [Pyethereum](https://github.com/ethereum/pyethereum) in Python
    - Another client with probably the best readable EVM implementation ([ethereum/vm.py](https://github.com/ethereum/pyethereum/blob/develop/ethereum/vm.py))
* [Py-EVM](https://github.com/pipermerriam/py-evm) in Python
    - An alternate Python implementation designed to be highly configurable and modular.
* [EthereumJ](https://github.com/ethereum/ethereumj) in Java
    - A client with its own EVM implementation
* [eth-isabelle](https://github.com/pirapira/eth-isabelle)
    - An EVM implementation for theorem provers
* [Modeling EVM in the K framework](https://github.com/kframework/evm-semantics) ([whitepaper](https://www.ideals.illinois.edu/handle/2142/97207))
    - An EVM implementation for [K framework](http://www.kframework.org/index.php/Main_Page)
* [hevm](https://github.com/dapphub/hevm)
    - An EVM implementation written in Haskell with debugging in mind
* [Burrow](https://github.com/hyperledger/burrow)
    - An EVM implementation in Go extended with a native name registry and permissioning layer

## Programming Languages that Compile into EVM

* [Solidity](https://github.com/ethereum/solidity)
    - The most popular programming language for Ethereum contracts
    - [Awesome Solidity](https://github.com/bkrem/awesome-solidity)
    - The LLL compiler is also in the same repository
* [Viper](https://github.com/ethereum/viper)
    - A language with overflow-checking, numeric units but without unlimited loops
* [Bamboo](https://github.com/pirapira/bamboo)
    - A language without loops but with explict constructor invocation at the end of every call
* [EthSharp](https://github.com/EthSharp/ethsharp-compiler)
    - A C# compiler for Ethereum smart contracts

## Debuggers

* [REMIX](https://github.com/ethereum/remix)
    - An IDE containing an EVM code debugger
* [debug\_traceTransaction method](https://github.com/ethereum/go-ethereum/wiki/Management-APIs#debug_tracetransaction)
    - An instruction-wise trace information provided by go-ethereum
* [Ethereum Function Signature Database](https://www.4byte.directory/)
    - A database for deciphering `0x165ffd10` into `restart(bytes32,bytes32)`.

## Code Analyzers

* [Mythril](https://github.com/b-mueller/mythril)
    - A blockchain exploration tool that indexes all contracts on the network, containing a disassembler, an ABI function detector and a control flow analyzer.
    - Comes with a [--fire-laser option](https://hackernoon.com/crafting-ethereum-exploits-by-laser-fire-1c9acf25af4f)
* [porosity](https://github.com/comaeio/porosity)
    - A reverse enginering tool, a disassembler, an ABI function detector and a decompiler that also highlights vulnerabilities
* [evmdis](https://github.com/arachnid/evmdis)
    - A disassembler for EVM code
* [Securify](http://securify.ch/)
    - A tool that strives to achieve no false-negatives
    - The implementation seems not public as of now
* [Oyente](https://github.com/melonproject/oyente)
    - An automatic EVM code analyzer based on symbolic execution and [Z3](https://github.com/Z3Prover/z3) SMT solver
* [Dr. Y's Ethereum Contract Analyzer](http://dry.yoichihirai.com/)
    - A symbolic executor for EVM code

## Improvement Proposals

* [Ethereum Improvement Proposals](https://github.com/ethereum/EIPs)
    - A portal for EVM & Ethereum improvements
    - The soonest changes are listed in the README
* [EVM 1.5](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-615.md)
    - A proposal to tame jumps so that a linear-time scan can determine stack layouts
* [eWASM](https://github.com/ewasm)
    - A proposal to use a [WebAssembly](http://webassembly.org/) for Ethereum contract execution

## Related Resources

* [Awesome Ethereum](http://awesome-ethereum.com/)

## License of This List

Awesome Ethereum Virtual Machine

Written in 2017 by Yoichi Hirai <i@yoichihirai.com>

[other author/contributor lines as appropriate]

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
