# Appendix — Lessons from Retractions (Concise Playbook)

Version 2.0 — Pressure-Transparent Edition

This one-page appendix distills key lessons from retractions and failed replication attempts in the superconductivity literature, especially for high-pressure hydrides, into an actionable checklist.

## Core Principles

1) Pressure Honesty
- Always declare measurement pressure explicitly (GPa) with calibration method and error bars
- Do not imply ambient-pressure retention; acknowledge rapid decomposition below ~100 GPa at 300 K
- Use pressure-transparent language throughout (no “quenching” or “frozen-in” claims)

2) Multi-Signal Verification
- Electrical: Four-point R(T) with clear zero-resistance transition
- Magnetic: Field suppression of Tc (on the same sample if possible)
- Structural: XRD or Raman under pressure confirming phase at measurement P
- Computational: SSCHA phonons at measurement P; α²F(ω), λ, ωlog linked to observed Tc

3) Data Integrity
- Publish raw data (R(T), susceptibility, Raman/XRD, calibration traces)
- Document background subtraction and all processing steps
- Provide scripts, fits, and parameters (μ*, k-mesh, cutoffs) for computational work

4) Statistics and Replication
- Multiple samples (n ≥ 3) with consistent behavior
- Report uncertainties, error bars, and fit confidence intervals
- Encourage independent replication; share samples or protocols when feasible

5) Controls
- Magnetic field suppression of Tc (magnitude and rate)
- Isotope shift (H → D) consistent with phonon-mediated pairing
- Systematic Tc(P) mapping; report dTc/dP and non-superconducting regions

## Common Pitfalls Behind Retracted Claims

- Ambiguous signals attributed to superconductivity without controls
- Inadequate pressure calibration; single-point or unreliable standards
- Insufficient structural verification at measurement conditions
- Hidden processing steps (undocumented background subtraction, filtering)
- Single-sample or single-run claims with no statistics

## Reporting Standard (YAML)

Include in Issues/PRs:

```yaml
measurement_type: [experimental|computational|hybrid]
pressure_range: [min_GPa, max_GPa]
temperature_range: [min_K, max_K]
sample_composition: "La_x Y_y H_z"
measurement_techniques: [four_point_resistance, ac_susceptibility, raman, xrd]
controls_performed: [field_suppression, isotope_effect, pressure_dependence]
data_availability: [link_to_raw_data_repository]
pressure_calibration: [ruby_R1, diamond_raman, other]
computational_method: [DFT_pkg, SSCHA_impl, Eliashberg_solver]
validation_status: [preliminary|validated|peer_reviewed]
```

## Pre-Submission Checklist (Quick)

- [ ] Pressure stated (GPa) with calibration method and uncertainty
- [ ] R(T) shows clear transition; zero resistance confirmed
- [ ] Field suppression of Tc demonstrated (field range and suppression rate reported)
- [ ] Isotope shift measured (H/D) with consistent Tc change
- [ ] Tc(P) mapped with dTc/dP and non-superconducting regions disclosed
- [ ] Structural confirmation (Raman/XRD) at measurement P
- [ ] Raw data, processing scripts, and parameters published
- [ ] SSCHA phonons at measurement P; α²F(ω), λ, ωlog reported (for comp/hybrid)
- [ ] Replication evidence (multiple samples/runs) and statistics included
- [ ] Language is pressure-transparent; no ambient/quenched claims

## Claim Language Guidance

Use:
- “Superconductivity observed at P = 150 GPa with Tc ≈ 300 K; decomposes below ~100 GPa at 300 K”
- “Field suppression, isotope shift (H→D), and Tc(P) trends are consistent with phonon-mediated pairing”

Avoid:
- “Ambient-pressure superconductivity” (unless unambiguously, reproducibly demonstrated—which contradicts current hydride thermodynamics)
- “Quenched to ambient” without rigorous, reproducible evidence and stability analysis

## References and Further Reading

- Raw data and protocols should be linked in your submission (Zenodo/Figshare/GitHub LFS)
- Cite established hydride high-pressure literature and calibration standards
- Use SSCHA/Eliashberg references appropriate to your toolchain

—

This appendix enforces reproducibility, transparency, and thermodynamic consistency, helping prevent the common failure modes that lead to retractions.
