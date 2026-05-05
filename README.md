# Paper 11: Gravitational Entropy Escrow

**An Interpretive Synthesis of Thermodynamic Approaches to Gravity**

Grant Lavell Whitmer III · Windstorm Labs, The Windstorm Institute · Fort Ann, NY, USA

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20032023-blue)](https://doi.org/10.5281/zenodo.20032023)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey)](https://creativecommons.org/licenses/by/4.0/)
[![Track: Entropic Bounds](https://img.shields.io/badge/Track-2_·_Entropic_Bounds-8b5cf6)](https://windstorminstitute.org/#track2)

**Zenodo**: [10.5281/zenodo.20032023](https://doi.org/10.5281/zenodo.20032023) · **Current version: v0.6.11** (May 2026)

---

## What this paper proposes

> *Gravitational binding energy U between two masses is identical, up to a sign and a temperature factor, to the entropy S_esc held in escrow by the binding. The escrow is redeemed at the local Unruh temperature T whenever the binding is altered. Forces felt by an observer are gradients of escrowed entropy in that observer's frame; trajectories are paths along which the gradient is extremized.*

Formally: `S_esc(r) = |U(r)| / T(r)` and `F = T · ∇S_esc`, with `T(r) = ℏa(r)/(2πck_B)` the local Unruh temperature.

The paper claims **no priority on individual derivations**. The mathematical machinery is due to Bekenstein, Hawking, Unruh, Jacobson, Padmanabhan, Verlinde, and van Putten. The contribution is **interpretive**: a single physical picture under which the disparate results of those authors describe one phenomenon — that **gravity is the universe's accounts-receivable system for entropy held off the books in bound configurations.**

## What gets recovered under the picture

| Regime | Recovered result | How |
|--------|------------------|-----|
| Newtonian | `F = GMm/r²` | Verlinde's derivation, exact, no free parameters (§4) |
| Black hole horizons | Bekenstein–Hawking entropy `S = k_B A / 4ℓ_p²` | Escrow at `r_s = 2GM/c²` evaluated with Hawking temperature (§5) |
| Deep MOND / Tully–Fisher | `v⁴ = GM_b · a_0` | de Sitter floor `T_dS = ℏc√(Λ/3)/(2πk_B)` as Carnot floor on escrow exchange (§6) |
| Equivalence principle | Tidal forces as irreducible differential of escrow | Frame-dependence of entropy gradients (§3) |

## Empirical anchors developed in the paper

- **Five-case test on Genzel et al. (2017) high-z galaxies (§6.1).** Five `a_0` prescriptions × two interpolation functions, evaluated against the six high-redshift disk galaxies from Genzel. **Constant `a_0` cases pass at `|Δ| ≲ 0.05 dex`; both `H(z)`-tracking and `(1+z)^(3/2)`-tracking fail by margins of 0.10–0.18 dex.** The framework's structural commitment to `Λ` rather than `H(z)` is supported by this test.
- **SPARC reanalysis (§8.4).** 175 disk galaxies; deep-MOND `a_0` derived globally and per-galaxy. **Global median: 1.24 × 10⁻¹⁰ m/s²**, agreeing with Milgrom's canonical 1.20 × 10⁻¹⁰ m/s² within ~4%. The framework's bare Λ-form prediction is `9.0 × 10⁻¹¹ m/s²` — about 25% below the empirical value, accounted for by an order-unity coefficient `α ≈ 1.39` whose derivation is identified as the central technical task remaining.
- **Cross-redshift consistency (§8.5).** SPARC at z ≈ 0 and Genzel at z ≈ 0.85–2.4 are mutually consistent with a single time-independent `a_0` ∈ (1.08, 1.25) × 10⁻¹⁰ m/s². No statistically resolved evolution across ~11 Gyr.

## What the paper honestly does not claim

- **No new mathematical machinery.** The framework is interpretive; it claims a physical picture, not a derivation of new equations.
- **No precise value of `a_0`.** The bare Λ-form prediction is off by ~25%; the order-unity coefficient `α` is a structural placeholder awaiting derivation (§8.4.3).
- **No transition functional form.** The deep-MOND asymptote is recovered by a family of interpolation functions (§10); selecting a unique one from horizon thermodynamics is open.
- **No closed dynamical system.** The relativistic extension (§7) identifies the structurally correct form of modified field equations as `G_μν + Λ_eff(τ) g_μν = (8πG/c⁴) T_μν^(total)`, but `Λ_eff(τ)` has not been derived. The Bianchi-incompatible naive multiplicative form is explicitly rejected.
- **The cluster-cores problem.** The framework predicts cluster cores (high `T_local`) should be firmly Newtonian. The data show the largest discrepancies precisely in cores. **This is a real difficulty the framework cannot dissolve in its present form** (§8.2). Flagged honestly rather than dressed up.

## Read the Paper

- **[paper.pdf](paper.pdf)** — full v0.6.11 manuscript
- **[paper/Paper11-v0.6.11-draft.md](paper/Paper11-v0.6.11-draft.md)** — markdown source
- **[Website article](https://windstorminstitute.org/articles/gravitational-entropy-escrow.html)** — long-form companion

## Empirical analysis code (SPARC + Genzel)

Two numerical analyses are referenced in the paper:
- **Genzel five-case test** (§6.1, Table 1): residuals over 6 galaxies × 5 a_0 prescriptions × 2 interpolation functions
- **SPARC global deep-MOND `a_0`** (§8.4): median of `g_obs²/g_bar` over ~1,400 deep-MOND points in ~140 galaxies
- **SPARC interpolation comparison** (§10): smoke test of simple-μ, McGaugh-ν, and quadrature interpolations on ~200 radial points across ~14 galaxies

Reproducible scripts and raw outputs:
**[Windstorm-Labs/gravitational-entropy-escrow](https://github.com/Windstorm-Labs/gravitational-entropy-escrow)**

Current authoritative archive: **[Zenodo (10.5281/zenodo.20032023)](https://doi.org/10.5281/zenodo.20032023)**.

---

## Discuss this paper

- **Discuss the paper's ideas** → [Comments on the website article](https://windstorminstitute.org/articles/gravitational-entropy-escrow.html#comments) (powered by GitHub Discussions on the website repo)
- **Typo, citation issue, or paper-content correction?** → [Open an Issue on this repo](../../issues)
- **Bug in the analysis code, or a reproduction question?** → [Issue](https://github.com/Windstorm-Labs/gravitational-entropy-escrow/issues) or [Discussion](https://github.com/Windstorm-Labs/gravitational-entropy-escrow/discussions) on the Labs repo

---

## The Windstorm Institute — Two Research Tracks

### Track 1 — The Throughput Basin · 9 papers (Papers 1–9 globally; 1st through 9th in this track; arc complete)

| # | Paper | DOI |
|---|-------|-----|
| 1 | [The Fons Constraint](https://github.com/Windstorm-Institute/fons-constraint) | [10.5281/zenodo.19274048](https://doi.org/10.5281/zenodo.19274048) |
| 2 | [The Receiver-Limited Floor](https://github.com/Windstorm-Institute/receiver-limited-floor) | [10.5281/zenodo.19322973](https://doi.org/10.5281/zenodo.19322973) |
| 3 | [The Throughput Basin](https://github.com/Windstorm-Institute/throughput-basin) | [10.5281/zenodo.19323194](https://doi.org/10.5281/zenodo.19323194) |
| 4 | [The Serial Decoding Basin τ](https://github.com/Windstorm-Institute/serial-decoding-basin) | [10.5281/zenodo.19323423](https://doi.org/10.5281/zenodo.19323423) |
| 5 | [The Dissipative Decoder](https://github.com/Windstorm-Institute/dissipative-decoder) | [10.5281/zenodo.19433048](https://doi.org/10.5281/zenodo.19433048) |
| 6 | [The Inherited Constraint](https://github.com/Windstorm-Institute/inherited-constraint) | [10.5281/zenodo.19432911](https://doi.org/10.5281/zenodo.19432911) |
| 7 | [The Throughput Basin Origin](https://github.com/Windstorm-Institute/throughput-basin-origin) | [10.5281/zenodo.19498582](https://doi.org/10.5281/zenodo.19498582) |
| 8 | [The Vision Basin](https://github.com/Windstorm-Institute/vision-basin) | [10.5281/zenodo.19672827](https://doi.org/10.5281/zenodo.19672827) |
| 9 | [The Hardware Basin](https://github.com/Windstorm-Institute/hardware-basin) | [10.5281/zenodo.19672921](https://doi.org/10.5281/zenodo.19672921) |

### Track 2 — Entropic Bounds in Analog Systems · 3 papers (Papers 10–12 globally; 1st through 3rd in this track; line of inquiry active)

| # | Paper | DOI |
|---|-------|-----|
| 10 | [Phonon Extraction Bound (BEC Analog Gravity)](https://github.com/Windstorm-Institute/phonon-extraction-bound) *(1st in track)* | [10.5281/zenodo.20014391](https://doi.org/10.5281/zenodo.20014391) |
| 11 | [Gravitational Entropy Escrow](https://github.com/Windstorm-Institute/gravitational-entropy-escrow) *(this paper — 2nd in track)* | [10.5281/zenodo.20032023](https://doi.org/10.5281/zenodo.20032023) |
| 12 | [C8 Clarification Note](https://github.com/Windstorm-Institute/c8-clarification-note) *(3rd in track; companion to this paper)* | [10.5281/zenodo.20041992](https://doi.org/10.5281/zenodo.20041992) |

**Website:** [windstorminstitute.org](https://windstorminstitute.org)

---

*License: MIT (code) and CC BY 4.0 (data, figures, paper text). See [LICENSE](LICENSE).*
