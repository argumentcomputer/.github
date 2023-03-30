# Welcome to Lurk Lab
<p align="center">
  <img width="250" height="250" src="/lurk-lab-logo.png">
</p>

# Lurk Lang
Lurk is an in-development, Turing-complete programming language for recursive zk-SNARKs.

## Disclaimer
**DISCLAIMER:** Lurk is an early research-stage language. Neither the cryptography nor the software has been audited, and there is currently no trusted setup for Groth16 circuits. Do not use Lurk in production environments or anywhere else that security is necessary.

## lurk and lurk-rs
[```lurk-rs```](https://github.com/lurk-lab/lurk-rs) is the Rust implementation of Lurk, which generates binaries via ```rustc```. The Rust implementation supports expression evaluation, proof of correct evaluation, and proof verification. ```lurk-rs``` also provides preliminary support for WASM.

[```lurk```](https://github.com/lurk-lab/lurk) is a Common Lisp reference implementation of Lurk. This implementation only supports expression evaluation. The [language specification](https://github.com/lurk-lab/lurk/blob/master/spec/v0-1.md) lives in this repo, and the implementation provided there aims for simplicity and demonstration of the intended semantics without the proving tools of ```lurk-rs```.

## Features of Lurk
- Lurk program execution can be proved in zero knowledge.
- Lurk proofs support multiple backend SNARK proving systems.
- Lurk enables incremental computation and proofs in unbounded loops.
- Lurk provides conditional control flow.
- Lurk programs are data and vice versa.
- Lurk data is content-addressable for compatibility with IPLD/IPFS.

# Yatima
[Yatima](https://github.com/lurk-lab/yatima) is a dependently typed, content addressed compiler from the [Lean Theorem Prover](https://github.com/leanprover/lean4) to Lurk. This enables formally verified zk-proofs of execution, whether it's abstract cryptography via [FFaCiL.lean](https://github.com/lurk-lab/FFaCiL.lean) or interpreted WebAssembly code via [Wasm.lean](https://github.com/lurk-lab/Wasm.lean).

## Website
Visit us on the web at https://lurk-lab.com or https://lurk-lang.org. 

## Zulip
Come hang out on our [Zulip](https://zulip.lurk-lab.com). 

## Twitter
Follow [@LurkLab](https://twitter.com/LurkLab) on Twitter.

## License
MIT or Apache 2.0
