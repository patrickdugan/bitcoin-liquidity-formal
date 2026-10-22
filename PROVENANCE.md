# Source provenance

This repository was extracted from the **formal** directory of
[patrickdugan/Spiral](https://github.com/patrickdugan/Spiral/tree/878e201f709e1fcb217abb6555f46da7c3732e93/formal).

- Immutable source commit: `878e201f709e1fcb217abb6555f46da7c3732e93`
- Original source review: [Spiral PR #4](https://github.com/patrickdugan/Spiral/pull/4), closed as superseded by narrowly scoped fixes
- Original Lean+Mathlib CI: [passing run 39756621856](https://github.com/patrickdugan/Spiral/actions/runs/39756621856)
- Model witness CI: [passing run 39756621959](https://github.com/patrickdugan/Spiral/actions/runs/39756621959)
- Model review packet: [REVIEW.md](REVIEW.md), migrated from `formal/REVIEW.md`
- Separate manuscript correction: [Spiral PR #7](https://github.com/patrickdugan/Spiral/pull/7)
- Isolated model fixes: [#8 routing](https://github.com/patrickdugan/Spiral/pull/8), [#9 Ark capital clock](https://github.com/patrickdugan/Spiral/pull/9), [#10 registry encoding](https://github.com/patrickdugan/Spiral/pull/10)

The Lean files retain their original bytes. This standalone import gives the
formalization a separate Git history and dependency boundary; source authorship
and historical test evidence remain discoverable from the immutable source
commit. The extraction is **a copy with provenance**, not a claim to have
preserved the original `git subtree` commit ancestry.

## Verification boundary

Theorems describe finite abstract models of directional cut conservation,
atomic server fronting, cross-class ledger accounting, deterministic pooling,
and bilateral channel-to-cut refinement. They do not establish universal
equivalence with Bitcoin Core or deployed Lightning/Ark implementations, and
the stochastic π/2 pooling limit remains an independent claim.

Run locally:

```sh
lake update
lake exe cache get
lake build
lake build SpiralFormal.Audit
```

CI repeats these steps and fails on admitted placeholders.
