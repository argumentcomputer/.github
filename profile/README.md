![](/ArgumentComputerCorp_logo.png)
<br />

# Our Mission
We are building the tools to accelerate verifiable computing. 

<br />

# Our Products

## Lurk
Lurk is a programming language build for the domain of zero-knowledge proofs. 

[```lurk```](https://github.com/argumentcomputer/lurk) is a Common Lisp reference implementation of Lurk. This implementation only supports expression evaluation. The [language specification](https://github.com/argumentcomputer/lurk/blob/master/spec/v0-1.md) lives in this repo, and the implementation provided there aims for simplicity and demonstration of the intended semantics without the proving tools of ```lurk-rs```.

[```lurk-rs```](https://github.com/argumentcomputer/lurk-rs) is the Rust implementation of Lurk, which generates binaries via ```rustc```. The Rust implementation supports expression evaluation, proof of correct evaluation, and proof verification. ```lurk-rs``` also provides preliminary support for WASM.

### Disclaimer
**DISCLAIMER:** Lurk is an early research-stage language. Neither the cryptography nor the software has been audited, and there is currently no trusted setup for Groth16 circuits. Do not use Lurk in production environments or anywhere else that security is necessary.

## Sphinx
[Sphinx](https://github.com/argumentcomputer/sphinx) is our fork of [Succinct](https://succinct.xyz/) Labs' [SP1 zero-knowledge virtual machine (ZKVM)](https://github.com/succinctlabs/sp1).

Sphinx underpins critical elements of our zero-knowledge proof efforts, including light clients in collaboration with [Wormhole](https://wormhole.foundation/blog/wormhole-foundation-awards-contributor-grant-to-lurk-lab-to-bring-trustless-transfers-to-wormhole-with-zk-proofs) and [Kadena](https://www.kadena.io/blog/kadena-announces-partnership-with-lurk-lab-to-build-zk-bridge). It also drives the forthcoming STARK engine of [Lurk](https://github.com/argumentcomputer/lurk-rs), Argument's next-generation zero-knowledge virtual machine

## Yatima
[Yatima](https://github.com/argumentcomputer/yatima) is a dependently typed, content addressed compiler from the [Lean Theorem Prover](https://github.com/leanprover/lean4) to Lurk. This enables formally verified zk-proofs of execution, whether it's abstract cryptography via [FFaCiL.lean](https://github.com/argumentcomputer/FFaCiL.lean) or interpreted WebAssembly code via [Wasm.lean](https://github.com/argumentcomputer/Wasm.lean).

## Loam
Loam is a reduction machine zkVM, purpose built to provide the smallest instruction set surface for the most performant verifiable virtual machine across a variety of back-ends.

(Coming soon)

## Light Clients
[ZK Light Clients](https://github.com/argumentcomputer/zk-light-clients/) built in collaboration with the [Wormhole Foundation](https://wormhole.foundation/blog/wormhole-foundation-awards-contributor-grant-to-lurk-lab-to-bring-trustless-transfers-to-wormhole-with-zk-proofs) and [Kadena](https://www.kadena.io/blog/kadena-announces-partnership-with-lurk-lab-to-build-zk-bridge), enable ZK proof-based cross-chain interoperability.

<br />

# Contact Us

## Website
Visit us on the web at https://argument.xyz

## Zulip
Come hang out on our [Zulip](https://zulip.argument.xyz). 

## Twitter
Follow [@argumentxyz](https://twitter.com/argumentxyz) on Twitter.

## License
MIT or Apache 2.0
