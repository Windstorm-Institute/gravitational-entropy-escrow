# Submission scaffold — Physical Review D

**Title:** Gravitational Entropy Escrow: An Interpretive Synthesis of Thermodynamic Approaches to Gravity

**Author:** Grant Lavell Whitmer III, The Windstorm Institute, Fort Ann, NY 12827, USA · grantwhitmer3@gmail.com

**PACS / PhySH:** Entropic gravity · Bekenstein–Hawking entropy · Modified Newtonian dynamics · Cosmological constant · Foundations of general relativity · Thermodynamics of spacetime

**Suggested section:** Section IV — General Relativity, Cosmology, and Astrophysics → Foundations of General Relativity. Alternative: Sec. III if treated as a thermodynamics-of-gravity submission.

---

## Cover-letter abstract

We propose a physical reframing under which gravity and entropy are revealed as the same phenomenon viewed through different vocabularies. Gravitational binding energy is entropy held in escrow against the local Unruh temperature; the universe attracts because the books want to balance. The mathematical machinery is due to Bekenstein, Hawking, Unruh, Jacobson, Padmanabhan, Verlinde, and van Putten; we claim no priority on individual derivations. What is offered here is the picture that connects them: under the escrow postulate, Newton's law (Verlinde 2011), Bekenstein–Hawking entropy at horizons, the equivalence principle (as frame-dependence of escrow gradients), and the deep-MOND Tully–Fisher relation with `a_0` set by the de Sitter floor temperature, all follow from one principle. We sketch a covariant extension that identifies the structurally correct form of the modified field equations as `G_μν + Λ_eff(τ) g_μν = (8πG/c⁴) T_μν^(total)` (the Bianchi-incompatible naive multiplicative form is explicitly rejected). We engage quantitatively with the empirical literature, including a five-case extension of Milgrom's (2017) test on the Genzel et al. (2017) high-redshift galaxies that independently disfavors `H(z)`-tracking of `a_0` alongside the `(1+z)^(3/2)` exclusion, and a SPARC reanalysis yielding global deep-MOND `a_0 ≈ 1.24 × 10⁻¹⁰ m/s²`. The framework's bare Λ-form prediction lies ~25% below the empirical value; the residual is identified honestly as an order-unity coefficient awaiting derivation, and the paper is explicit about what it does not yet derive.

---

## What's in this repo

- `paper.pdf` — full manuscript (v0.6.11)
- `paper/Paper11-v0.6.11-draft.md` — markdown source
- `paper-arxiv.tex` — arXiv submission scaffold (gr-qc)
- `article.html` — long-form companion article (also at windstorminstitute.org)

## Reviewer reproducibility statement

The Genzel five-case test (Table 1, §6.1), the SPARC reanalysis (§8.4), and the interpolation comparison (§10) are reproducible from the Python analysis scripts at `Windstorm-Labs/gravitational-entropy-escrow`. The full SPARC mass-models table (Lelli, McGaugh & Schombert 2016) is publicly available; the deposited code uses the standard cuts and ϒ_disk = 0.5 / ϒ_bul = 0.7 fiducials adopted by Lelli et al.

## Note on scope and posture

The paper is interpretive. It does not present new mathematical machinery. The relativistic extension (§7) identifies the structural form of the modified field equations and the Bianchi-respecting Λ_eff(τ) sector but does not derive Λ_eff(τ); this and the cluster-cores difficulty (§8.2) are flagged honestly as open problems rather than dressed up. The submission posture is that of a synthesis article, not a derivation article.
