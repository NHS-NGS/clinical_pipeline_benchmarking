# _ACGS GATK4 Reference Implementation_

## Participants

- Product owner: Simon Boardman
- Team: ACGS Bioinformatics
- Stakeholders: ACGS Bioinformatics, NHS Clinical Bioinformaticians
- Other key relationships: GEL Bioinformaticians


## Current Status

Draft 20180112


## Purpose

Validate a set of commands and parameters for running GATK4 in an NHS Clinical Laboratory.
The aim is to provide the minimum level of sensitivity and specificity using GATK4 which must be achievable for all laboratories.
Compare performance to current best practice variant callers (GATK3, DeepVariant, Dragen).


## Project Goals & Objectives

Create a standardised GATK4 variant calling workflow with a known sensitivity and specificity which can be implemented in any NHS Laboratory.
* Variant calling command/workflow.
* Performance statistics for a set of truth variants as per (GA4GH guidelines)[https://www.biorxiv.org/content/early/2018/03/15/270157].
* Comparison with GATK3.
* Comparison with DeepMind.
* Comparison with Dragen.


## Requirements

### Functional

* Process a bam file containing a set of truth variants.
* Produce a standard VCF.
* Calculate sensitivity and specificity.

### Technical (non-functional)

* Incorporate GATK Best Practice as specified by The Broad.
* Portable between UNIX systems.
* Comparison of sensitivity/specificity with GATK3, Dragen, and DeepVariant.

### Usability

- Portable between laboratories.
- Consistent with current bioinformatics standards and guidelines.
