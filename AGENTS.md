# Agent guidance

This project is a separate formal proof package about Bitcoin liquidity
accounting, imported from Spiral at the pinned source commit in PROVENANCE.md.

For each new claim, state exact quantifiers, assumptions, and target
implementation correspondence. Keep proof status distinct from finite model
tests and real Bitcoin consensus semantics. Do not silently weaken a theorem
to make it provable.

After edits run `lake build` and `lake build SpiralFormal.Audit` and verify
all named roots are registered in the audit. If a claim remains unproved, record
its precise boundary in README.md or a tracking issue instead of using
`sorry` or adding unexplained axioms.

The manuscript lives in patrickdugan/Spiral, and upstream
ProofOfKeags/btc-verified has its own `AGENTS.md` and contribution conventions.
