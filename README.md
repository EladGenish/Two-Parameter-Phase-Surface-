RNSE: Two-Parameter Phase Surface (τ × ρ)
Summary

We present a public, surface-only characterization of the RNSE substrate under a two-parameter sweep over:

τ (morphology axis)

ρ (admissibility control axis)

The results demonstrate:

A sharp admissibility collapse along ρ.

Orthogonal modulation of internal morphology along τ.

Stable multi-threshold boundary behavior across 32 independent seeds.

Reproducible, public-safe artifacts with no internal trace disclosure.

Each plotted point aggregates over 32 seeds × 4,096 ticks.

Experimental Setup

A 2D grid was evaluated over normalized τ × ρ.

For each cell:

32 independent seeds were run.

Each run executed 4,096 ticks.

Aggregate metrics were computed:

acceptance rate

std(D)

entropy(ψ)

spectral flatness(ψ)

var_tail

composite regime intensity

No per-tick traces are included in the public release.

See: manifest_PUBLIC.json for certification metadata. 

manifest_PUBLIC

Key Result: Orthogonal Control Axes

The phase surface reveals:

ρ-axis (Admissibility Control)

Acceptance collapses sharply as ρ increases.
The boundary is invariant in τ under normalization.

τ-axis (Morphology Control)

Internal regime metrics (entropy, dispersion, spectral structure) vary along τ independently of admissibility collapse.

This separation produces a structured 2-parameter regime surface.

Boundary Certification

The admissibility boundary was extracted under multiple target thresholds:

β ∈ {0.003, 0.005, 0.007}

Results show:

Monotonic boundary shift under β variation.

Stable location across 32 seeds.

Minimal τ-dependence.

See:

boundary_overlay_PUBLIC_v2.png

tau_invariance_PUBLIC_v2.png

boundary_overlay_PUBLIC.csv

Public Artifact Policy

The public release includes:

Aggregated phase surfaces

Boundary overlays

Multi-seed certification metrics

Deterministic artifact hashes

Excluded:

Per-tick time series

Internal state traces

Exact non-normalized parameter coordinates

This ensures surface-only reproducibility while preserving internal substrate structure.

Reproducibility

All artifacts are certified in:

manifest_PUBLIC.json 

manifest_PUBLIC

Includes:

seed set hash

artifact SHA256 digests

sweep configuration

threshold values

aggregation policy

Interpretation

The τ × ρ surface demonstrates:

A control parameter governing admissibility collapse.

An orthogonal parameter governing morphology.

Stable boundary behavior under threshold perturbation.

This is consistent with a dimensionless computational substrate exhibiting structured regime transitions under constraint.
