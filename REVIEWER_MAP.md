# Reviewer Map

## Claim Scope

- Canonical-lane claim: inside the `manifold_constrained` routed lattice, if the theorem chain in this repository holds and the guard certificate passes, the repository-level super-lane closure claim is satisfied.
- Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.
- External-strengthening rule: any statement beyond the admissible class must retain the explicit remainder carried by the defect/coherence ledgers; see `notes/GEOMETRIC_GALOIS_BRIDGE.md`.

## Super-Lane Families

1. `section-conjecture and packet-reconstruction packages`
2. `profinite and birational fundamental-group recovery packages`
3. `hyperbolicity and entire-curve exclusion packages`
4. `decomposition-group and local-global compatibility packages`
5. `endpoint stitching across the declared anabelian-hyperbolic package`

## Theorem Dependency Chain

1. `EG1`: coercive response and active control floor.
2. `EG2`: capture and admissible continuation.
3. `EG3`: compactness and no-collapse spacing.
4. `EG4`: rigidity and transfer.
5. Identification bridge: strict coherence on the determining class.
6. Scalar closure: `AHY_G1`, `AHY_G2`, `AHY_G3`, `AHY_G4`, `AHY_G5`, `AHY_G6`, `AHY_GM` all `PASS`.

Primary files:

- `paper/ANABELIAN_HYPERBOLICITY_PREPRINT.md`
- `notes/EG1_public.md`
- `notes/EG2_public.md`
- `notes/EG3_public.md`
- `notes/EG4_public.md`
- `notes/IDENTIFICATION_BRIDGE.md`
- `notes/GEOMETRIC_GALOIS_BRIDGE.md`

## Closure Gates

| Gate | Constant | Description |
|------|----------|-------------|
| `AHY_G1` | `kappa_hyperbolic` | projected hyperbolic response has a strict positive floor |
| `AHY_G2` | `sigma_section` | section-reconstruction defect stays above capture floor across admissible profinite and jet losses |
| `AHY_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `AHY_G4` | `rho_rigidity` | bad anabelian-hyperbolic countermodels are excluded |
| `AHY_G5` | `reconstruction_transfer` | rigid limit transfers to the anabelian-hyperbolic endpoint package |
| `AHY_G6` | `eps_coh` | strict coherence / identification closure |
| `AHY_GM` | derived | final strict margin |

## Falsification Conditions

- `repro/certificate_runtime.json` has any non-`PASS` gate.
- `lane.active_lane != "manifold_constrained"`.
- `all_pass != true`.
- Any manifest hash mismatch under `repro/repro_manifest.json`.
- A verified counterexample to any EG theorem statement used in the paper.
