---
name: High-Pressure Superconductor Research Contribution
about: Submit experimental, computational, or protocol improvements for La–Y–H systems
title: '[CONTRIBUTION] Brief description of changes'
labels: 'needs-review, pressure-transparent'
assignees: ''
---

## Required Metadata (YAML Block)

**⚠️ PRs lacking this metadata block will be closed pending completion.**

```yaml
contribution_type: [experimental_data|computational_results|protocol_improvement|documentation|analysis_tools]
measurement_type: [experimental|computational|hybrid|not_applicable]
pressure_range: [min_GPa, max_GPa, or "not_applicable"]
temperature_range: [min_K, max_K, or "not_applicable"]
sample_composition: "La_x Y_y H_z or not_applicable"
measurement_techniques: [list_techniques_or_not_applicable]
controls_performed: [field_suppression, isotope_effect, pressure_dependence, or "not_applicable"]
data_availability: [raw_data_link_or_repository_or_not_applicable]
pressure_calibration: [method_and_standards_or_not_applicable]
computational_method: [DFT_package, SSCHA_implementation, or "not_applicable"]
validation_status: [preliminary|validated|peer_reviewed|not_applicable]
```

---

## Pull Request Type
<!-- Select the type of contribution by putting an 'x' in the appropriate box -->

- [ ] Experimental Data Contribution
- [ ] Computational Results
- [ ] Protocol Improvement/Enhancement
- [ ] Documentation Update
- [ ] Analysis Tools/Scripts
- [ ] Bug Fix
- [ ] Reproducibility Study
- [ ] Literature Review/Analysis

---

## Summary
<!-- Provide a clear and concise description of your contribution -->

---

## Pressure-Transparent Compliance
<!-- All boxes must be checked for research contributions -->

- [ ] **Pressure Requirements Acknowledged**: My contribution acknowledges that superconductivity requires sustained pressures of 120–180 GPa
- [ ] **No Ambient Claims**: I am not claiming or supporting ambient-pressure superconductivity or pressure quenching
- [ ] **Thermodynamic Consistency**: My results/analysis respect fundamental thermodynamic stability constraints
- [ ] **Proper Controls**: For experimental claims, I have performed required control measurements (field suppression, isotope effect, pressure dependence)

---

## Detailed Description
<!-- Provide a detailed description of what you've changed and why -->

## Motivation and Context
<!-- Why is this change required? What problem does it solve? -->
<!-- If it addresses an open issue, please link to the issue here -->

Addresses issue #(issue_number)

---

## Changes Made

### Files Added
- 
- 
- 

### Files Modified
- 
- 
- 

### Files Removed
- 
- 
- 

---

## Experimental Validation
<!-- For experimental data contributions -->

### New Experimental Data
- **Data Type**: 
- **Measurement Conditions**: 
- **Sample Information**: 
- **Validation Method**: 

### Reproducibility Testing
- [ ] Results reproduced in same laboratory (minimum 3 samples)
- [ ] Results reproduced by independent group
- [ ] Statistical analysis performed
- [ ] Error analysis included
- [ ] Control measurements completed

**Reproducibility Details**: 

### Required Control Measurements
- [ ] **Field Suppression**: Magnetic field suppresses superconducting transition
  - Applied Field Range: 
  - Tc Suppression Rate: 
- [ ] **Isotope Effect**: H/D substitution affects Tc
  - Isotope Substitution: 
  - Tc Shift Observed: 
- [ ] **Pressure Dependence**: Tc varies systematically with pressure
  - Pressure Range: 
  - dTc/dP: 

---

## Computational Validation
<!-- For computational contributions -->

### DFT Calculations
- [ ] Structure optimization converged
- [ ] Phonon stability confirmed (no imaginary modes)
- [ ] Electronic structure validated
- [ ] Pressure dependence calculated

### SSCHA Phonon Calculations
- [ ] Self-consistent convergence achieved
- [ ] Temperature effects included
- [ ] Anharmonic corrections applied
- [ ] Superconducting properties calculated

### Validation Results
- **Tc Prediction**: 
- **Pressure Range**: 
- **λ Parameter**: 
- **ωlog**: 

---

## Data Quality and Availability

### Data Attachments
- [ ] Raw experimental data
- [ ] Processed data and analysis
- [ ] Computational input/output files
- [ ] Analysis scripts and procedures
- [ ] Error analysis and statistics
- [ ] Pressure calibration data

### Data Repository
- **Primary Repository**: 
- **Backup Location**: 
- **Access Instructions**: 
- **File Formats**: 

### Data Quality Metrics
- **Signal-to-Noise Ratio**: 
- **Measurement Uncertainty**: 
- **Statistical Significance**: 
- **Reproducibility Score**: 

---

## Protocol Changes
<!-- For protocol modifications -->

### Modified Procedures
- **Section**: 
- **Change**: 
- **Rationale**: 
- **Impact**: 

### Safety Considerations
- [ ] No new safety risks introduced
- [ ] New safety measures added where needed
- [ ] Safety documentation updated
- [ ] Safety review completed

**Safety Assessment**: 

---

## Testing and Validation

### Experimental Testing
- [ ] New experiments conducted
- [ ] Existing data reanalyzed
- [ ] Literature comparison performed
- [ ] Independent validation obtained

### Computational Testing
- [ ] Convergence tests performed
- [ ] Basis set optimization completed
- [ ] k-point convergence verified
- [ ] Anharmonic effects validated

### Code Testing (if applicable)
- [ ] Unit tests added/updated
- [ ] Integration tests passed
- [ ] Code review completed
- [ ] Documentation updated

---

## Impact Assessment

### Scientific Impact
- **Significance**: Low / Medium / High / Breakthrough
- **Scope**: Single measurement / Multiple systems / General protocol
- **Applications**: 

### Practical Impact
- **Ease of Implementation**: Easy / Moderate / Difficult
- **Resource Requirements**: 
- **Time Savings**: 
- **Cost Implications**: 

### Reproducibility Impact
- **Improves Reproducibility**: Yes / No
- **Standardization**: Yes / No
- **Quality Control**: Enhanced / Maintained / Not Applicable

---

## Compatibility Assessment

- [ ] Backward compatible with existing protocols
- [ ] Requires updates to existing procedures
- [ ] Breaking changes introduced (requires migration guide)
- [ ] Migration guide provided (if applicable)

**Compatibility Notes**: 

---

## Peer Review and Validation

### Internal Review
- [ ] Laboratory peer review completed
- [ ] Supervisor/PI approval obtained
- [ ] Institutional review completed
- [ ] Ethics review completed (if applicable)

### External Review
- [ ] External expert consulted
- [ ] Literature review conducted
- [ ] Community feedback incorporated
- [ ] Independent validation sought

**Review Summary**: 

---

## Documentation Updates

### Documentation Changes
- [ ] README updated
- [ ] Protocol documentation updated
- [ ] Analysis documentation updated
- [ ] Examples added/updated
- [ ] Troubleshooting guide updated

### New Documentation
- [ ] New protocol sections added
- [ ] New analysis methods documented
- [ ] New safety procedures documented
- [ ] New examples provided

---

## Quality Assurance Checklist

### General Requirements
- [ ] I have read and followed the contributing guidelines
- [ ] I have searched existing PRs to ensure this is not a duplicate
- [ ] My changes follow the project's standards
- [ ] I have tested my changes thoroughly
- [ ] All requirements are met

### Scientific Requirements
- [ ] Experimental procedures follow established protocols
- [ ] Data quality meets project standards
- [ ] Statistical analysis is appropriate and complete
- [ ] Results are scientifically sound and reproducible
- [ ] Safety protocols have been followed
- [ ] Pressure calibration is properly documented

### Data Requirements
- [ ] Raw data is preserved and accessible
- [ ] Processing steps are documented
- [ ] Error analysis is performed
- [ ] Statistical significance is assessed
- [ ] Outliers are identified and explained

### Computational Requirements (if applicable)
- [ ] Convergence tests performed
- [ ] Basis set/cutoff optimization completed
- [ ] k-point convergence verified
- [ ] Phonon stability confirmed
- [ ] Anharmonic effects included where relevant

---

## References and Citations

### Supporting Literature
- 
- 
- 

### Related Work
- 
- 
- 

### Methodology References
- 
- 
- 

---

## Legal and Ethical Compliance

### Legal Requirements
- [ ] I have the right to submit this contribution
- [ ] No proprietary information is included
- [ ] Proper attribution is provided for all sources
- [ ] Copyright requirements are met
- [ ] License compatibility confirmed

### Ethical Requirements
- [ ] Research ethics guidelines followed
- [ ] Data integrity maintained throughout
- [ ] No selective reporting or data manipulation
- [ ] Conflicts of interest disclosed
- [ ] Institutional approvals obtained

---

## Collaboration Information

### Contributors
- **Primary Author**: 
- **Co-authors**: 
- **Institutions**: 
- **Funding Sources**: 

### Acknowledgments
- **Technical Support**: 
- **Equipment/Facilities**: 
- **Collaborating Groups**: 

---

## Future Work and Limitations

### Known Limitations
<!-- Describe any known limitations of your contribution -->

### Future Improvements
<!-- Describe potential future developments -->

### Follow-up Studies
<!-- Describe recommended follow-up work -->

---

## Contact Information

- **Primary Contact**: 
- **Institution**: 
- **Email**: 
- **ORCID**: 
- **Preferred Contact Method**: 

---

## Additional Notes

### Special Instructions
<!-- Any special instructions for reviewers -->

### Reviewer Notes
<!-- Specific areas where you'd like focused feedback -->

### Timeline Considerations
<!-- Any time-sensitive aspects of this contribution -->

---

**Review Process**: This PR will undergo rigorous scientific peer review including validation of experimental controls, computational convergence, and data integrity. Please be patient as we ensure the quality and validity of all contributions.

**Data Privacy**: Ensure no confidential or proprietary information is included in this public pull request.

**Artifact Concerns**: Reviewers will specifically check for measurement artifacts, computational convergence issues, and proper control experiments. Please address these proactively in your submission.
