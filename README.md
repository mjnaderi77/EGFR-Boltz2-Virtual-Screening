# EGFR-Boltz2-Virtual-Screening
Deep learning-based EGFR–ligand structural prediction and virtual screening
# EGFR–Erlotinib Structural Prediction and Validation Using Boltz-2

## Project Overview

This project investigates the application of Boltz-2, a deep learning-based biomolecular modeling framework, for predicting protein–ligand complexes and evaluating ligand-binding interactions.

The initial phase focuses on the EGFR–Erlotinib complex, using an experimentally determined crystallographic structure as a reference for structural validation.

The long-term objective is to establish a computational workflow for evaluating Boltz-2 predictions and extending the framework to virtual screening of larger ligand libraries.

## Target Protein

- Protein: Epidermal Growth Factor Receptor (EGFR)
- Sequence length: 312 amino acids
- Target: EGFR kinase domain
- Reference ligand: Erlotinib

## Computational Framework

- Boltz-2: Protein–ligand complex prediction
- Python: Data processing and structural analysis
- RDKit: Ligand preparation and chemical validation
- Structural alignment: Comparison of predicted and experimental structures

## Current Progress

### Phase 1: Input Preparation
- EGFR protein sequence preparation.
- Erlotinib ligand preparation and SMILES validation.
- Boltz-2 YAML input generation.

### Phase 2: Boltz-2 Prediction
- Low-MSA prediction workflow.
- Protein–ligand complex prediction.
- Generation of structural and confidence-related outputs.
- Binding affinity prediction.

### Phase 3: Structural Validation
Preliminary protein structural alignment produced the following results:

| Alignment region | RMSD (Å) |
|---|---:|
| Residues 1–312 | 11.344 |
| Residues 1–250 | 0.651 |
| Residues 20–260 | 0.635 |
| Residues 30–250 | 0.614 |
| Robust alignment | 0.527 |

The results indicate strong structural agreement across the main aligned region, while substantial deviations were observed in the C-terminal region.

**Important:** Ligand pose validation and ligand RMSD analysis are still pending. Protein RMSD alone does not establish accurate ligand-binding pose prediction.

## Repository Structure

- `notebooks/`: Google Colab notebooks.
- `data/`: Protein and ligand input data.
- `results/`: Prediction outputs and structural analyses.
- `scripts/`: Analysis and processing scripts.
- `docs/`: Project methodology and documentation.

## Upcoming Work

1. Ligand binding pose validation.
2. Ligand RMSD calculation.
3. Analysis of protein–ligand interactions.
4. Evaluation of Boltz-2 binding affinity predictions.
5. Benchmarking against additional EGFR inhibitors.
6. Extension to large-scale virtual screening.

## Reproducibility

Google Colab notebook: [Add Colab Link]

## Project Status

Ongoing research project. Results are preliminary and further validation is required.

## License

To be determined.
