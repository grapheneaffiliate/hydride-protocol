# Contributing to High-Pressure Hydride Protocol Research

**Version 2.0 — Pressure-Transparent Edition**

Thank you for your interest in contributing to the High-Pressure Hydride Protocol research project! This document provides guidelines for contributing to our pressure-transparent superconductor research initiative focused on La–Y–H systems at 120–180 GPa.

## Table of Contents

- [Pressure-Transparent Principles](#pressure-transparent-principles)
- [Required Reporting Standards](#required-reporting-standards)
- [Contribution Types](#contribution-types)
- [YAML Metadata Requirements](#yaml-metadata-requirements)
- [Experimental Contributions](#experimental-contributions)
- [Computational Contributions](#computational-contributions)
- [Quality Standards](#quality-standards)
- [Review Process](#review-process)
- [What We Accept](#what-we-accept)
- [What We Do Not Accept](#what-we-do-not-accept)

---

## Pressure-Transparent Principles

This project is built on **pressure transparency** — honest acknowledgment of the high-pressure requirements for superconductivity in hydride systems. All contributions must adhere to these core principles:

### ✅ Accepted Principles
- **High-pressure requirement**: Superconductivity requires sustained pressures of 120–180 GPa
- **Thermodynamic consistency**: Respect for fundamental stability constraints
- **No ambient retention**: Acknowledgment that superconducting phases decompose below ~100 GPa
- **Proper controls**: Field suppression, isotope effects, and pressure dependence
- **Data integrity**: Complete reporting of all measurements and analysis

### ❌ Rejected Claims
- Ambient-pressure superconductivity or "pressure quenching"
- Metastable superconducting phases at low pressure
- Results without proper pressure calibration
- Selective data reporting or cherry-picking
- Exotic theoretical mechanisms not supported by established physics

---

## Required Reporting Standards

All research contributions (issues and pull requests) **must** include the following YAML metadata block. Contributions lacking this information will be closed pending completion.

### Standard YAML Block

```yaml
measurement_type: [experimental|computational|hybrid]
pressure_range: [min_GPa, max_GPa]
temperature_range: [min_K, max_K]
sample_composition: "La_x Y_y H_z"
measurement_techniques: [list_techniques_here]
controls_performed: [field_suppression, isotope_effect, pressure_dependence]
data_availability: [raw_data_link_or_repository]
pressure_calibration: [method_and_standards_used]
computational_method: [DFT_package, SSCHA_implementation, if_applicable]
validation_status: [preliminary|validated|peer_reviewed]
```

### YAML Field Descriptions

- **measurement_type**: Type of research (experimental, computational, or hybrid)
- **pressure_range**: Pressure range in GPa (must include 120+ GPa for superconducting claims)
- **temperature_range**: Temperature range in Kelvin
- **sample_composition**: Specific stoichiometry of La–Y–H system
- **measurement_techniques**: List of experimental or computational methods used
- **controls_performed**: Required control measurements for superconducting claims
- **data_availability**: Link to raw data repository or dataset
- **pressure_calibration**: Method and standards used for pressure determination
- **computational_method**: Software packages and methods for theoretical work
- **validation_status**: Level of validation (preliminary, validated, peer-reviewed)

---

## Contribution Types

### 1. Experimental Data Contributions

**Requirements:**
- Diamond anvil cell experiments at 120+ GPa
- Proper pressure calibration (ruby fluorescence, Raman)
- Complete control measurements
- Raw data availability
- Statistical analysis of reproducibility

**Mandatory Controls:**
- **Field Suppression**: Magnetic field suppresses superconducting transition
- **Isotope Effect**: H/D substitution affects critical temperature
- **Pressure Dependence**: Systematic variation of Tc with pressure

### 2. Computational Results

**Requirements:**
- DFT structure optimization with phonon stability
- SSCHA phonon calculations at measurement pressures
- Eliashberg theory analysis for superconducting properties
- Convergence testing and validation
- Input/output files provided

**Quality Standards:**
- Converged lattice parameters and electronic structure
- No imaginary phonon modes in superconducting phase
- Proper treatment of anharmonic effects
- λ parameter in reasonable range (2.5–3.5)

### 3. Protocol Improvements

**Requirements:**
- Clear identification of problem being solved
- Detailed methodology changes
- Validation of improvements
- Safety assessment
- Impact on existing protocols

### 4. Reproducibility Studies

**Requirements:**
- Independent replication attempts
- Statistical analysis of success/failure rates
- Identification of critical parameters
- Recommendations for protocol refinement

---

## YAML Metadata Requirements

### For Experimental Contributions

```yaml
measurement_type: experimental
pressure_range: [120, 180]  # GPa
temperature_range: [4, 300]  # K
sample_composition: "La_0.5 Y_0.5 H_3"
measurement_techniques: [four_point_resistance, ac_susceptibility, raman_spectroscopy]
controls_performed: [field_suppression, isotope_effect, pressure_dependence]
data_availability: "https://zenodo.org/record/1234567"
pressure_calibration: "ruby_fluorescence_R1_line"
computational_method: "not_applicable"
validation_status: validated
```

### For Computational Contributions

```yaml
measurement_type: computational
pressure_range: [100, 200]  # GPa
temperature_range: [0, 400]  # K
sample_composition: "La_1 Y_1 H_6"
measurement_techniques: [DFT_optimization, SSCHA_phonons, Eliashberg_theory]
controls_performed: "not_applicable"
data_availability: "https://github.com/user/hydride-calculations"
pressure_calibration: "not_applicable"
computational_method: "VASP_6.3, SSCHA_1.2, EPW_5.4"
validation_status: preliminary
```

### For Protocol Improvements

```yaml
measurement_type: "not_applicable"
pressure_range: "not_applicable"
temperature_range: "not_applicable"
sample_composition: "not_applicable"
measurement_techniques: [protocol_development]
controls_performed: "not_applicable"
data_availability: "not_applicable"
pressure_calibration: "not_applicable"
computational_method: "not_applicable"
validation_status: peer_reviewed
```

---

## Experimental Contributions

### Sample Preparation Standards

- **Precursor Purity**: >99.9% for La and Y metals
- **Hydrogen Loading**: Controlled H₂ pressure during synthesis
- **Phase Formation**: Laser heating or resistive heating protocols
- **Characterization**: XRD confirmation of target phase

### Pressure Generation Requirements

- **DAC Specifications**: Capable of sustained 120+ GPa
- **Anvil Quality**: Diamond anvils with proper culet size
- **Gasket Material**: Rhenium or steel gaskets
- **Pressure Medium**: Appropriate medium for electrical measurements

### Measurement Protocols

- **Electrical Transport**: Four-point resistance measurements
- **Temperature Control**: Calibrated temperature sensors
- **Magnetic Fields**: Capability for field suppression tests
- **Data Acquisition**: High-resolution, low-noise measurements

### Required Documentation

- Complete experimental parameters
- Pressure calibration procedures
- Temperature calibration methods
- Error analysis and uncertainty quantification
- Raw data files in standard formats

---

## Computational Contributions

### DFT Calculation Standards

- **Software**: VASP, Quantum ESPRESSO, or equivalent
- **Functionals**: PBE, PBEsol, or hybrid functionals
- **Pseudopotentials**: PAW or ultrasoft with proper validation
- **Convergence**: k-points, energy cutoff, and force convergence
- **Pressure**: Calculations at experimental pressure conditions

### SSCHA Requirements

- **Implementation**: SSCHA code with proper convergence
- **Supercell Size**: Adequate for anharmonic effects
- **Temperature Range**: Covering experimental conditions
- **Convergence**: Self-consistent harmonic approximation
- **Validation**: Comparison with harmonic results

### Superconducting Property Calculations

- **Eliashberg Theory**: Proper implementation with realistic μ*
- **Electron-Phonon Coupling**: Accurate λ parameter calculation
- **Critical Temperature**: McMillan-Allen-Dynes or full Eliashberg
- **Pressure Dependence**: Systematic variation with pressure

---

## Quality Standards

### Data Quality Requirements

- **Signal-to-Noise**: Adequate for clear identification of transitions
- **Reproducibility**: Multiple samples and measurement runs
- **Statistical Analysis**: Proper error bars and significance testing
- **Control Measurements**: All required controls performed
- **Documentation**: Complete metadata and procedures

### Computational Quality Requirements

- **Convergence Testing**: Systematic convergence studies
- **Validation**: Comparison with experimental data where available
- **Error Analysis**: Uncertainty quantification in predictions
- **Reproducibility**: Input files and procedures provided
- **Physical Consistency**: Results consistent with known physics

---

## Review Process

### Initial Screening

1. **YAML Metadata Check**: Presence and completeness of required metadata
2. **Pressure Transparency**: Compliance with pressure-transparent principles
3. **Data Availability**: Accessibility of raw data and supporting materials
4. **Control Measurements**: Verification of required experimental controls

### Scientific Review

1. **Technical Accuracy**: Correctness of methods and analysis
2. **Statistical Validity**: Appropriate statistical treatment
3. **Reproducibility Assessment**: Likelihood of independent replication
4. **Literature Consistency**: Agreement with established knowledge
5. **Safety Compliance**: Adherence to safety protocols

### Review Timeline

- **Initial Response**: 48-72 hours
- **Technical Review**: 1-2 weeks
- **Scientific Review**: 2-4 weeks
- **Final Decision**: Within 6 weeks

### Review Criteria

- Scientific rigor and validity
- Pressure-transparent compliance
- Data quality and completeness
- Reproducibility potential
- Safety considerations
- Documentation standards

---

## What We Accept

### ✅ Welcomed Contributions

- **High-pressure experimental data** with proper controls and calibration
- **SSCHA phonon calculations** at measurement pressures with convergence testing
- **Improved synthesis protocols** with validation and safety assessment
- **Theoretical analysis** within established BCS-Eliashberg framework
- **Reproducibility studies** with statistical analysis
- **Protocol refinements** based on systematic testing
- **Data analysis tools** with validation and documentation
- **Safety improvements** with risk assessment

### Quality Indicators

- Multiple independent samples/calculations
- Proper statistical analysis
- Complete control measurements
- Transparent data processing
- Comprehensive documentation
- Independent validation attempts

---

## What We Do Not Accept

### ❌ Rejected Contributions

- **Ambient-pressure superconductivity claims** (thermodynamically impossible)
- **Pressure quenching or metastable phases** (not supported by physics)
- **Data without pressure calibration** (essential for high-pressure work)
- **Results lacking control measurements** (field suppression, isotope effect, pressure dependence)
- **Selective data reporting** (cherry-picking favorable results)
- **Exotic theoretical mechanisms** (not supported by established physics)
- **Incomplete computational studies** (lacking convergence or validation)
- **Safety protocol violations** (endangering researchers)

### Red Flags

- Claims contradicting thermodynamics
- Missing or inadequate controls
- Unexplained anomalous behavior
- Insufficient documentation
- Lack of reproducibility data
- Pressure calibration issues
- Statistical inadequacies

---

## Getting Started

### Before Contributing

1. **Read the Documentation**: Familiarize yourself with the protocol and requirements
2. **Review Examples**: Examine accepted contributions for formatting and standards
3. **Prepare Metadata**: Gather all required information for YAML block
4. **Validate Data**: Ensure all quality standards are met
5. **Safety Check**: Confirm compliance with safety protocols

### Contribution Process

1. **Fork the Repository**: Create your own copy for modifications
2. **Create Feature Branch**: Use descriptive branch names
3. **Add Your Contribution**: Include all required files and documentation
4. **Complete YAML Metadata**: Ensure all required fields are filled
5. **Test and Validate**: Verify your contribution meets standards
6. **Submit Pull Request**: Use the provided template
7. **Respond to Reviews**: Address reviewer comments promptly

### Support and Questions

- **GitHub Issues**: Technical questions and bug reports
- **GitHub Discussions**: General questions and collaboration
- **Documentation**: Check existing documentation first
- **Email**: Sensitive matters or private inquiries

---

## Recognition and Attribution

### Contributor Recognition

- **Contributor List**: All contributors acknowledged in repository
- **Publication Credits**: Co-authorship for significant contributions
- **Collaboration Opportunities**: Invitation to research collaborations
- **Community Recognition**: Highlighting valuable contributions

### Publication Policy

- Significant contributors eligible for co-authorship
- All contributors acknowledged in publications
- Data contributors retain rights to original data
- Collaborative publications encouraged

---

## Legal and Ethical Considerations

### Intellectual Property

- Contributors retain rights to original work
- Contributions licensed under project license (CC-BY-SA 4.0)
- Proper attribution required for all work
- Respect for existing patents and IP rights

### Research Ethics

- Follow institutional review board guidelines
- Maintain data integrity throughout
- Report conflicts of interest
- Ensure proper safety protocols
- Respect confidentiality agreements

---

## Conclusion

Your contributions advance the field of high-pressure superconductor research while maintaining the highest standards of scientific rigor. By following these pressure-transparent guidelines, we can work together toward reproducible, reliable research that stands the test of independent validation.

The ultimate goal is not just to achieve room temperature superconductivity, but to do so through research that is honest about its requirements, transparent about its limitations, and rigorous in its methodology.

Thank you for contributing to the High-Pressure Hydride Protocol project!

---

**Questions?** Open an issue with the `question` label or start a discussion in the repository.

**Need Help?** Check our documentation, examples, and don't hesitate to ask for guidance.
