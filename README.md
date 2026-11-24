# zkp-playground

Personal practice repository to learn zero-knowledge proofs (R1CS, QAP, Groth16) in Rust,
in preparation for milestone 2 of the Fuzzion³ / Human Vault SDK project.

> **Rule:** this repository only contains my own exercises. No code from the client project
> is copied here.

## Structure

| Crate / folder | Exercise | Status |
|---|---|---|
| `lagrange` | Lagrange interpolation over a finite field | in progress |
| `r1cs` | `x³ + x + 5 = 35` as R1CS constraints, witness check | planned |
| `groth16-toy` | the same circuit proved and verified with Groth16 (arkworks 0.4) | planned |
| `notes/` | reading notes on *Proofs, Arguments, and Zero-Knowledge* (J. Thaler) | in progress |

## Usage

```bash
cargo test                 # all exercises
cargo test -p lagrange     # a single exercise
```

## References

- Justin Thaler, *Proofs, Arguments, and Zero-Knowledge*
- Vitalik Buterin, *Quadratic Arithmetic Programs: from Zero to Hero*
- arkworks documentation (`ark-relations`, `ark-groth16`)