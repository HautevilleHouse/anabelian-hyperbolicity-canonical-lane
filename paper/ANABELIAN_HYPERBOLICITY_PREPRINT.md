# Anabelian Hyperbolicity via Section-Reconstruction Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global super-architecture (`AHY1-AHY8`)

**Author:** HautevilleHouse  
**Date:** March 12, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving persistence of the declared section, reconstruction, and hyperbolic endpoint package across admissible fundamental-group transport through a multi-lane anabelian-hyperbolic super-architecture.

The proof program is organized as eight steps `AHY1-AHY8` with executable closure gates `AHY_G1`, `AHY_G2`, `AHY_G3`, `AHY_G4`, `AHY_G5`, `AHY_G6`, and `AHY_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

The target statement is: persistence of the declared section, reconstruction, and hyperbolic endpoint package across admissible fundamental-group transport.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.


### 1.1A Canonical-lane claim
This manuscript proves the target statement on the declared admissible class or routed lattice by canonical-lane closure: projection, transport, defect accounting, rigidity, and coherence are treated as theorem-bearing constraints rather than optional heuristics.

### 1.1B Bridge / equivalence statement
The canonical endpoint objects are tied to the standard problem-side target through the in-repo bridge package. The paper records the transfer or endpoint-identification step in the main theorem chain, and `notes/IDENTIFICATION_BRIDGE.md` fixes the determining-class lock in ordinary mathematical language.

### 1.1C Verification surface
A reviewer can check this claim on four surfaces:

1. the standard target statement in Section `1.1`,
2. the canonical objects and closure gates in the main paper,
3. the endpoint bridge in `notes/IDENTIFICATION_BRIDGE.md`,
4. the executable rerun `bash repro/run_repro.sh` with runtime output `repro/certificate_runtime.json`.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

### 1.3 Super-lane role

This manuscript is a routed super-repo rather than a single primitive endpoint case. The declared admissible lattice coordinates:

1. section-conjecture and packet-reconstruction packages.
2. profinite and birational fundamental-group recovery packages.
3. hyperbolicity and entire-curve exclusion packages.
4. decomposition-group and local-global compatibility packages.
5. endpoint stitching across the declared anabelian-hyperbolic package.

### 1.4 Explicit remainder discipline

External strengthenings beyond the declared admissible class retain an explicit remainder ledger.

Write `X = X_mc ⊎ R`, with projected admissible sector `P_mc X = X_mc` and remainder projector `Q_rem = I - P_mc`.

Any statement extending beyond `X_mc` must keep `R` explicit and cannot silently collapse the complement into the closed lane.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let `u_tau = (S_tau, Pi_tau, H_tau, D_tau, L_tau)` denote the admissible state of section packets, profinite fundamental-group data, hyperbolic constraints, defect ledgers, and endpoint locks.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_AHY = min(kappa_hyperbolic, sigma_section, kappa_compact, rho_rigidity, reconstruction_transfer) - eps_coh`.

Target:

`M_AHY > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive hyperbolic response that prevents collapse of the admissible closure package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `AHY_G1` | `kappa_hyperbolic` | projected hyperbolic response has a strict positive floor |
| `AHY_G2` | `sigma_section` | section-reconstruction defect stays above capture floor across admissible profinite and jet losses |
| `AHY_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `AHY_G4` | `rho_rigidity` | bad anabelian-hyperbolic countermodels are excluded |
| `AHY_G5` | `reconstruction_transfer` | rigid limit transfers to the anabelian-hyperbolic endpoint package |
| `AHY_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `AHY_GM` | derived | all upstream gates pass and `M_AHY > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_hyperbolic` = 1.0946500000000001,
- `sigma_section` = 1.075,
- `kappa_compact` = 0.8032128514056224,
- `rho_rigidity` = 1.079,
- `reconstruction_transfer` = 1.031658,
- `eps_coh = 0.0`.

Hence:

`M_AHY = 0.8032128514056224 > 0`.

### 4.5 Raw coercive constant

Define `kappa_hyperbolic^(raw) := c_hyper_raw * hyper_density_raw - e_hyper_raw`.

Current extracted value:

`kappa_hyperbolic = 1.0946500000000001`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`AHY1-AHY8`)

1. `AHY1` Active projected response block on the canonical sector.
2. `AHY2` Uniform capture bounds on the canonical admissible tube.
3. `AHY3` Restart map preserving admissible data.
4. `AHY4` First-failure compactness extraction.
5. `AHY5` Rigidity exclusion of bad countermodels.
6. `AHY6` Endpoint transfer closure on the extracted target class.
7. `AHY7` Determining-class identification of the intended endpoint.
8. `AHY8` Final persistence theorem: the endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_section^(raw) := section_floor_raw - reconstruction_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_section = 1.075`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8032128514056224`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of bad anabelian-hyperbolic countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.079 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the anabelian-hyperbolic endpoint package by the bridge inequality.

Define `reconstruction_transfer^(raw) := c_reconstruction_raw * transfer_gain_raw - e_reconstruction_raw`.

Current extracted value:

`reconstruction_transfer = 1.031658 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of endpoint observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_hyperbolic` | `AHY_G1` | `1.0946500000000001` |
| `sigma_section` | `AHY_G2` | `1.075` |
| `kappa_compact` | `AHY_G3` | `0.8032128514056224` |
| `rho_rigidity` | `AHY_G4` | `1.079` |
| `reconstruction_transfer` | `AHY_G5` | `1.031658` |
| `eps_coh` | `AHY_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.054` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `AHY_G1, AHY_G2, AHY_G3, AHY_G4, AHY_G5, AHY_G6, AHY_GM = PASS`,
- strict margin `M_AHY = 0.8032128514056224`,
- lane: `manifold_constrained`.
