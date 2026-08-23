![](/ArgumentComputerCorp_logo.png)
<br />

Accelerate Certified Computing. 

<br />

# Our Projects

## Ix
[```ix```](https://github.com/argumentcomputer/ix) is a zero-knowledge proof-carrying code platform for [Lean 4](https://github.com/leanprover/lean4). Ix compiles Lean programs and proofs into succinct cryptographic certificates: instead of rechecking a formal proof, anyone can verify a small zk-SNARK attesting that the proof was checked. This extends classical proof-carrying code into zero-knowledge proof-carrying code (zkPCC), compressing even mathlib-scale developments into kilobyte-sized certificates that verify in milliseconds.

Ix consists of:

- the **Ix compiler**, which transforms Lean 4 into ```ixon```, a content-addressable serialization format
- **Aiur**, a first-order functional zkDSL that generates multicircuit STARK proofs via [```multi-stark```](https://github.com/argumentcomputer/multi-stark)
- the **IxVM**, which implements reduction, typechecking, and binary ingress/egress of ```ixon```
- peer-to-peer sharing of ```ixon``` data via [Iroh](https://github.com/n0-computer/iroh)

**DISCLAIMER:** Ix is pre-alpha research software. Do not use Ix in production environments or anywhere else that security is necessary.

## multi-stark
[```multi-stark```](https://github.com/argumentcomputer/multi-stark) is a multicircuit STARK proving system built on [Plonky3](https://github.com/Plonky3/Plonky3). It proves and verifies multiple AIR circuits of independent trace heights in a single proof, with cross-circuit lookup arguments for shared state, preprocessed tables reusable across proofs, and generic parameterization over the field, hash function, and polynomial commitment scheme. ```multi-stark``` is the proving engine behind Ix's Aiur zkDSL.

## Lean 4 tooling
We build and maintain open-source tooling for the Lean 4 ecosystem, including:

- [```LSpec```](https://github.com/argumentcomputer/LSpec), a testing framework for Lean 4
- [```Blake3.lean```](https://github.com/argumentcomputer/Blake3.lean), Lean 4 bindings to the BLAKE3 cryptographic hash function
- [```lean-ffi```](https://github.com/argumentcomputer/lean-ffi), a Rust library for interfacing with the Lean 4 FFI

We also contribute to and maintain forks of ecosystem infrastructure such as [```lean4lean```](https://github.com/argumentcomputer/lean4lean), [```lean4-nix```](https://github.com/argumentcomputer/lean4-nix), and [```EVMYulLean```](https://github.com/argumentcomputer/EVMYulLean).

<br />

# Contact Us

## Website
Visit us on the web at https://argument.xyz

## Zulip

Chat with us on our [Zulip](https://zulip.argument.xyz) forum. 

## License
MIT or Apache 2.0
