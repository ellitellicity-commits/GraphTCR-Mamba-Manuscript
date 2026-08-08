# GraphTCR-Mamba: Manuscript and References

This repository holds the manuscript for "GraphTCR-Mamba: heterogeneous graph learning with Mamba for TCR-epitope binding prediction."

Authors: Ellison Naz, Adam Fan, Wenjun Lin, and Ping Luo.
Ellison Naz, Wenjun Lin, and Ping Luo are with the Department of Computer Science and Mathematics at Algoma University in Brampton, Ontario, Canada. Adam Fan is with Bayview Secondary School in Richmond Hill, Ontario, Canada.
Corresponding author: Ping Luo, ping.luo@algomau.ca

## Overview

T-cell receptor recognition of peptide epitopes is central to adaptive immunity, yet only a small fraction of potential TCR-epitope interactions can be characterized experimentally. This work introduces GraphTCR-Mamba, a heterogeneous graph framework that represents TCRs and epitopes as distinct node types, integrates sequence-similarity and observed-interaction edges, and incorporates a Mamba selective state-space branch for global information propagation.

## Key Results

| Dataset    | AUROC | AUPR  |
|------------|-------|-------|
| IEDB       | 0.938 | 0.925 |
| McPAS-TCR  | 0.943 | 0.947 |
| VDJdb      | 0.993 | 0.992 |

Cold-start evaluation across TCR-cold, epitope-cold, and both-cold settings showed the model generalizes well to unseen TCRs, though performance declines when epitopes or both interaction partners are unseen. This gap between random pair-level and cold-start performance underscores the importance of cold-start evaluation for assessing generalization to unseen interaction partners.

## Repository Structure

    GraphTCR-Mamba-Manuscript/
    ├── manuscript/     # Draft versions of the paper (docx or tex)
    ├── figures/        # Figure 1 through 4 source files
    ├── tables/         # Table 1 and 2 source data
    └── references/     # Citation files (bib)

## Related Repository

The model implementation and code are maintained separately at [GraphTCR-Mamba](https://github.com/GenTensor/GraphTCR-Mamba).

## Keywords

T cell receptor, heterogeneous graph, TCR-epitope prediction, Mamba, Laplacian positional encoding

## Funding

This work is supported by the Algoma University Research Fund.
