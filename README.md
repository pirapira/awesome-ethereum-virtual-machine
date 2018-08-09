# Awesome Ethereum Virtual Machine

[![Documentation chat](https://img.shields.io/badge/gitter-Docs%20chat-4AB495.svg)](https://gitter.im/ethereum/documentation)

> A list about the Ethereum Virtual Machine using the Awesome format.

A curated list of resources on the Ethereum Virtual Machine (EVM), which is the virtual machine executed on the [Ethereum](https://ethereum.org/) network.

Not listed there yet, but in the spirit of [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

Here is [how to contribute](./contributing.md).

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Contents**

- [Specification](#specification)
- [Illustration](#illustration)
- [Tutorials](#tutorials)
- [Tests](#tests)
- [EVM Implementations](#evm-implementations)
  - [Live on Main Network](#live-on-main-network)
  - [Other Implementations](#other-implementations)
- [Programming Languages that Compile into EVM](#programming-languages-that-compile-into-evm)
  - [Programming Languages that Compile zk-SNARK Circuits and Proofs](#programming-languages-that-compile-zk-snark-circuits-and-proofs)
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
* [Consensus Datastructures](https://github.com/ethereum/wiki/wiki/Consensus-Datastructures)

## Tests

* [Consensus test suite](https://github.com/ethereum/tests)
    - EVM implementations can be tested against this test suite

## EVM Implementations

### Live on Main Network

* [go-ethereum](https://github.com/ethereum/go-ethereum)
    - A popular Ethereum client with its own EVM implementation ([core/vm](https://github.com/ethereum/go-ethereum/tree/master/core/vm) directory)
* [Parity](https://github.com/paritytech/parity) in Rust
    - Another popular Ethereum client with its own EVM implementation ([ethcore](https://github.com/paritytech/parity/tree/master/ethcore) directory)
* [cpp-ethereum](https://github.com/ethereum/cpp-ethereum)
    - An Ethereum client that generates the consensus test suite ([libevm/VM.cpp](https://github.com/ethereum/cpp-ethereum/blob/develop/libevm/VM.cpp))
* [Pyethereum](https://github.com/ethereum/pyethereum) in Python
    - A mostly deprecated client ([ethereum/vm.py](https://github.com/ethereum/pyethereum/blob/develop/ethereum/vm.py))
* [Py-EVM](https://github.com/pipermerriam/py-evm) in Python
    - A Python implementation designed to be highly configurable and modular and compliant with the Ethereum test suite, work is in progress on it to run a full node and develop sharding.
* [EthereumJ](https://github.com/ethereum/ethereumj) in Java
    - A client with its own EVM implementation
* For more, see [here](https://github.com/ethereum/wiki/wiki/Clients).

### Other Implementations

* [SputnikVM](https://github.com/ethereumproject/sputnikvm) in Rust for Ethereum Classic
    - A standalone EVM featuring [a developer
      environment](https://github.com/ethereumproject/sputnikvm-dev),
      a [browser through wasm32-unknown-emscripten
      target](https://github.com/sorpaas/sputnikvm-in-browser), and for
      [embedded devices](https://github.com/sorpaas/sputnikvm-on-rux)
* [Modeling EVM in the K framework](https://github.com/kframework/evm-semantics) ([whitepaper](https://www.ideals.illinois.edu/handle/2142/97207))
    - An EVM implementation for [K framework](http://www.kframework.org/index.php/Main_Page)
* [hevm](https://github.com/dapphub/hevm)
    - An EVM implementation written in Haskell with debugging in mind
* [eth-isabelle](https://github.com/pirapira/eth-isabelle)
    - An EVM implementation for theorem provers
* [Burrow](https://github.com/hyperledger/burrow)
    - An EVM implementation in Go extended with a native name registry and permissioning layer
* [Ethereumjs-VM](https://github.com/ethereumjs/ethereumjs-vm)
    - Implements Ethereum's VM in JS
* [ruby-ethereum](https://github.com/cryptape/ruby-ethereum)
    - An EVM implementation in Ruby (passed all tests in [ethereum tests](https://github.com/ethereum/tests/tree/55a18b3ded93bf6083f23ea1f4bf7be4ba973016))
* [sputter](https://github.com/nervous-systems/sputter)
    - An EVM implementation in Clojure (so far passes VM tests)
* [eth-acl2](https://github.com/zchn/eth-acl2)
    - An EVM implementation in ACL2 (work in progress)
* [Ciri](https://github.com/ciri-ethereum/ciri)
    - An EVM implementation in Ruby (so far passed all tests in [ethereum tests](https://github.com/ethereum/tests/tree/073035c6ef89ae878c528e78d3b5ce59d1b71df7), aims to be a full Ethereum implementation)

## Programming Languages that Compile into EVM

* [Solidity](https://github.com/ethereum/solidity)
    - The most popular programming language for Ethereum contracts
    - [Awesome Solidity](https://github.com/bkrem/awesome-solidity)
    - The LLL compiler is also in the same repository
* [Vyper](https://github.com/ethereum/vyper)
    - A language with overflow-checking, numeric units but without unlimited loops
* [Pyramid Scheme](https://github.com/MichaelBurge/pyramid-scheme) (experimental)
    - A Scheme compiler into EVM that follows the [SICP compilation approach](https://mitpress.mit.edu/sicp/full-text/book/book-Z-H-35.html#%_sec_5.5)
    - [ceagle](https://github.com/MichaelBurge/ceagle) compiles C into Pyramid Scheme
* [Flint](https://github.com/franklinsch/flint)
    - A language with several security features: e.g. asset types with a restricted set of atomic operations
* [LLLL](https://github.com/mmalvarez/eth-isabelle/blob/master/example/LLLL.thy)
    - An LLL-like compiler being implemented in Isabelle/HOL
* [HAseembly-evm](https://github.com/takenobu-hs/haskell-ethereum-assembly)
    - An EVM assembly implemented as a Haskell DSL
* [Bamboo](https://github.com/pirapira/bamboo) (experimental)
    - A language without loops but with explicit constructor invocation at the end of every call

### Programming Languages that Compile zk-SNARK Circuits and Proofs

* [Zokrates](https://github.com/JacobEberhardt/ZoKrates)
    - A toolbox for zkSNARKs on Ethereum
    - [a third-party tutorial](https://github.com/jstoxrocky/zksnarks_example)
* [snarky](https://github.com/o1-labs/snarky)
    - An OCaml front-end for writing R1CS SNARKs (parametrized over the backend SNARK libraries)
    - Shallowly embedded DSL that can be compiled into SNARK circuits
    - The verifier is an OCaml function, so some more work is necessary before using it on Ethereum
* [jsnark](https://github.com/akosba/jsnark)
    - A Java front-end for writing R1CS SNARKs 

## Debuggers

* [REMIX](https://github.com/ethereum/remix)
    - An IDE containing an EVM code debugger
* [debug\_traceTransaction method](https://github.com/ethereum/go-ethereum/wiki/Management-APIs#debug_tracetransaction)
    - An instruction-wise trace information provided by go-ethereum
* [Ethereum Function Signature Database](https://www.4byte.directory/)
    - A database for deciphering `0x165ffd10` into `restart(bytes32,bytes32)`.

## Code Analyzers

* [Echidna](https://github.com/trailofbits/echidna)
    - A fuzzer on EVM that also takes Solidity input
    - Able to fuzz a program with sequences of multiple transactions
* [MAIAN](https://arxiv.org/abs/1802.06038)
    - An automatic tool that detects trace vulnerabilities (Greedy, Prodigal and Suicidal) with depth-first search of symbolic execution of multiple invocations
* [Mythril](https://github.com/b-mueller/mythril)
    - A blockchain exploration tool that indexes all contracts on the network, containing a disassembler, an ABI function detector and a control flow analyzer
    - Comes with a [--fire-laser option](https://hackernoon.com/crafting-ethereum-exploits-by-laser-fire-1c9acf25af4f)
    - Powered by [laser-ethereum](https://github.com/b-mueller/laser-ethereum)
* [porosity](https://github.com/comaeio/porosity)
    - A reverse enginering tool, a disassembler, an ABI function detector and a decompiler that also highlights vulnerabilities
* [Manticore](https://github.com/trailofbits/manticore)
    - A symtolic execution engine that can generate inputs to cover codepaths ([asciicast](https://asciinema.org/a/154012)), which also comes with a Python API
* [evmdis](https://github.com/arachnid/evmdis)
    - A disassembler for EVM code
* [ethersplay](https://github.com/trailofbits/ethersplay)
    - An EVM plugin for [Binary Ninja](https://binary.ninja/)
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
    - An EVM ABI compliant implementation to use [WebAssembly](http://webassembly.org/) for Ethereum contract execution, work is underway on [shasper](https://notes.ethereum.org/SCIg8AH5SA-O4C1G1LYZHQ)

## Related Resources

* [Awesome Ethereum](http://awesome-ethereum.com/)

## License of This List

Awesome Ethereum Virtual Machine

Written in 2017 by Yoichi Hirai: <i@yoichihirai.com>

[other author/contributor lines as appropriate]

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
