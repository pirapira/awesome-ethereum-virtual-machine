# Stale Resources

This file contains resources that were previously listed in the main [README](./README.md) but are now archived, abandoned, or otherwise no longer maintained. They are preserved here for historical reference.

---

## EVM Implementations (Stale)

### Former Main-Network Clients

* [Parity](https://github.com/paritytech/parity) in Rust
    - Redirects to the archived [openethereum/parity-ethereum](https://github.com/openethereum/parity-ethereum). Parity was superseded by OpenEthereum, which was itself discontinued in 2022.
* [cpp-ethereum](https://github.com/ethereum/cpp-ethereum)
    - Redirects to the archived [ethereum/aleth](https://github.com/ethereum/aleth). The C++ client was discontinued.
* [Pyethereum](https://github.com/ethereum/pyethereum) in Python
    - Officially archived. Superseded by Py-EVM.
* [Py-EVM](https://github.com/ethereum/py-evm) in Python
    - Officially archived. Was designed to be highly configurable and modular.
* [EthereumJ](https://github.com/ethereum/ethereumj) in Java
    - Officially archived. Java client abandoned.

### Other Implementations

* [SputnikVM](https://github.com/ethereumproject/sputnikvm) in Rust for Ethereum Classic
    - Redirects to the abandoned [ETCDEVTeam/sputnikvm](https://github.com/ETCDEVTeam/sputnikvm). The ETCDEV team disbanded. Featured a [developer environment](https://github.com/ethereumproject/sputnikvm-dev), a [browser through wasm32-unknown-emscripten target](https://github.com/sorpaas/sputnikvm-in-browser), and support for [embedded devices](https://github.com/sorpaas/sputnikvm-on-rux).
* [hevm](https://github.com/dapphub/hevm)
    - Officially archived. The project was relaunched at [ethereum/hevm](https://github.com/ethereum/hevm).
* [eth-isabelle](https://github.com/pirapira/eth-isabelle)
    - An EVM implementation for theorem provers. Abandoned, last active ~2022.
* [Burrow](https://github.com/hyperledger/burrow)
    - Redirects to the archived [hyperledger-archives/burrow](https://github.com/hyperledger-archives/burrow). An EVM implementation in Go extended with a native name registry and permissioning layer. Retired by Hyperledger in 2022.
* [ruby-ethereum](https://github.com/cryptape/ruby-ethereum)
    - Officially archived. An EVM implementation in Ruby (passed all tests in [ethereum tests](https://github.com/ethereum/tests/tree/55a18b3ded93bf6083f23ea1f4bf7be4ba973016)).
* [sputter](https://github.com/nervous-systems/sputter)
    - An EVM implementation in Clojure. Abandoned since ~2019.
* [solevm](https://github.com/Ohalo-Ltd/solevm)
    - Officially archived. An EVM implementation in Solidity.
* [eth-acl2](https://github.com/zchn/eth-acl2)
    - An EVM implementation in ACL2. Abandoned since ~2022.
* [mana](https://github.com/mana-ethereum/mana/)
    - An EVM implementation in Elixir. Repo moved from poanetwork; effectively inactive.

---

## Programming Languages (Stale)

### Languages that Compile into EVM

* [Pyramid Scheme](https://github.com/MichaelBurge/pyramid-scheme) (experimental)
    - Officially archived. A Scheme compiler into EVM that follows the [SICP compilation approach](https://web.mit.edu/6.001/6.037/sicp.pdf). [ceagle](https://github.com/MichaelBurge/ceagle) compiled C into Pyramid Scheme.
* [Flint](https://github.com/flintlang/flint)
    - A language with several security features (e.g. asset types with a restricted set of atomic operations). Research language; no commits since ~2022.
* [LLLL](https://github.com/mmalvarez/eth-isabelle/blob/master/example/LLLL.thy)
    - An LLL-like compiler implemented in Isabelle/HOL. The parent repo has been abandoned since ~2020.
* [HAseembly-evm](https://github.com/takenobu-hs/haskell-ethereum-assembly)
    - An EVM assembly implemented as a Haskell DSL. Abandoned since ~2018.
* [Bamboo](https://github.com/pirapira/bamboo) (experimental)
    - A language without loops but with explicit constructor invocation at the end of every call. Abandoned since ~2022.

### Languages that Compile zk-SNARK Circuits and Proofs

* [jsnark](https://github.com/akosba/jsnark)
    - A Java front-end for writing R1CS SNARKs. No commits since ~2022.

---

## Debuggers (Stale)

* [debug\_traceTransaction (go-ethereum wiki)](https://github.com/ethereum/go-ethereum/wiki/Management-APIs#debug_tracetransaction)
    - The go-ethereum GitHub wiki is a legacy resource; documentation has moved to [geth.ethereum.org](https://geth.ethereum.org/docs/interacting-with-geth/rpc/ns-debug).
* [Dr. Y's Ethereum Contract Analyzer](http://dry.yoichihirai.com/)
    - A symbolic executor for EVM code. Domain no longer exists (DNS NXDOMAIN).

---

## Code Analyzers (Stale)

* [porosity](https://github.com/msuiche/porosity)
    - A reverse engineering tool, disassembler, ABI function detector and decompiler that also highlights vulnerabilities. Abandoned since ~2019.
* [evmdis](https://github.com/arachnid/evmdis)
    - A disassembler for EVM code. Abandoned since ~2022.
* [ethersplay](https://github.com/crytic/ethersplay)
    - Officially archived. An EVM plugin for [Binary Ninja](https://binary.ninja/).
* [Oyente](https://github.com/enzymefinance/oyente)
    - Officially archived (under enzymefinance after Melon Protocol rebrand). An automatic EVM code analyzer based on symbolic execution and Z3 SMT solver.

---

## Improvement Proposals (Stale)

* [EVM 1.5](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-615.md)
    - A proposal to tame jumps so that a linear-time scan can determine stack layouts. EIP-615 has **Stagnant** status and was never advanced.
* [eWASM](https://github.com/ewasm)
    - A proposal to use [WebAssembly](http://webassembly.org/) for Ethereum contract execution. Superseded by other EVM evolution efforts; all repos effectively abandoned since ~2022.

---

## Related Resources (Stale)

* Awesome Ethereum (`http://awesome-ethereum.com/`)
    - Domain has been taken over by an unrelated website. The original content no longer exists.
