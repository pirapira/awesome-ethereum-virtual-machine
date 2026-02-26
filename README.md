# Awesome Ethereum Virtual Machine

A curated list of resources on the Ethereum Virtual Machine (EVM), which is the virtual machine executed on the [Ethereum](https://ethereum.org/) network.

Not listed there yet, but in the spirit of [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

Here is [how to contribute](./contributing.md).

Outdated and archived resources have been moved to [STALE.md](./STALE.md).

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

### Live on Main Network

* [go-ethereum](https://github.com/ethereum/go-ethereum)
    - A popular Ethereum client with its own EVM implementation ([core/vm](https://github.com/ethereum/go-ethereum/tree/master/core/vm) directory)
* [py-ethclient](https://github.com/tokamak-network/py-ethclient) in Python
    - A from-scratch Python execution client with 140+ EVM opcodes, RLPx transport, eth/68 and snap/1 wire protocols, full sync, snap sync, Engine API V1/V2/V3, and JSON-RPC
* For more, see
  [here](https://ethereum.org/developers/docs/nodes-and-clients/#execution-clients).

### Other Implementations

* [Modeling EVM in the K framework](https://github.com/runtimeverification/evm-semantics) ([whitepaper](https://www.ideals.illinois.edu/items/102260))
    - An EVM implementation for the [K framework](https://kframework.org/), maintained by Runtime Verification
* [hevm](https://github.com/ethereum/hevm)
    - An EVM implementation written in Haskell, focused on debugging and formal verification
* [Ethereumjs-VM](https://github.com/ethereumjs/ethereumjs-monorepo)
    - Implements Ethereum's VM in JS (part of the ethereumjs monorepo)

## Programming Languages that Compile into EVM

* [Solidity](https://github.com/ethereum/solidity)
    - The most popular programming language for Ethereum contracts
    - [Awesome Solidity](https://github.com/bkrem/awesome-solidity)
* [Vyper](https://github.com/vyperlang/vyper)
    - A language with overflow-checking, numeric units but without unlimited loops

### Programming Languages that Compile zk-SNARK Circuits and Proofs

* [Zokrates](https://github.com/Zokrates/ZoKrates)
    - A toolbox for zkSNARKs on Ethereum
* [snarky](https://github.com/o1-labs/snarky)
    - An OCaml front-end for writing R1CS SNARKs (parametrized over the backend SNARK libraries)
    - Shallowly embedded DSL that can be compiled into SNARK circuits
    - The verifier is an OCaml function, so some more work is necessary before using it on Ethereum

## Debuggers

* [Remix IDE](https://github.com/ethereum/remix-project)
    - An IDE containing an EVM code debugger
* [debug\_traceTransaction method](https://geth.ethereum.org/docs/interacting-with-geth/rpc/ns-debug)
    - An instruction-wise trace information provided by go-ethereum
* [Ethereum Function Signature Database](https://www.4byte.directory/)
    - A database for deciphering `0x165ffd10` into `restart(bytes32,bytes32)`.

## Code Analyzers

* [Echidna](https://github.com/crytic/echidna)
    - A fuzzer on EVM that also takes Solidity input
    - Able to fuzz a program with sequences of multiple transactions
* [MAIAN](https://arxiv.org/abs/1802.06038)
    - An automatic tool that detects trace vulnerabilities (Greedy, Prodigal and Suicidal) with depth-first search of symbolic execution of multiple invocations
* [Mythril](https://github.com/muellerberndt/mythril)
    - A security analysis tool for EVM bytecode; supports Solidity and Vyper
* [Manticore](https://github.com/trailofbits/manticore)
    - A symbolic execution engine that can generate inputs to cover codepaths ([asciicast](https://asciinema.org/a/154012)), which also comes with a Python API
* [Securify](https://github.com/eth-sri/securify2)
    - A tool that strives to achieve no false-negatives
* [L3X](https://github.com/VulnPlanet/l3x)
    - L3X - AI-driven Smart Contract Static Analyzer

## Improvement Proposals

* [Ethereum Improvement Proposals](https://github.com/ethereum/EIPs)
    - A portal for EVM & Ethereum improvements
    - The soonest changes are listed in the README

## License of This List

Awesome Ethereum Virtual Machine

Written in 2017 by Yoichi Hirai <i@yoichihirai.com>

[other author/contributor lines as appropriate]

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
