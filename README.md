# SpatialGRN

**An integrative workflow for spatial gene regulatory network (GRN) analysis using snMultiome and spatial transcriptomics data.**

## Overview

SpatialGRN is a computational workflow integrating single-nucleus multiome (snRNA-seq and snATAC-seq) and spatial transcriptomics data to characterize spatially resolved gene regulatory networks.

## Workflow

The workflow consists of five major steps:

1. **Spatial Transcriptomic Imputation:** Map snRNA-seq profiles onto Xenium spatial data using Tangram.
2. **GRN Inference:** Construct enhancer-driven gene regulatory networks using SCENIC+.
3. **Spatial GRN Imputation:** Project inferred regulatory programs into spatial coordinates.

## Repository Structure

```text
SpatialGRN/
│── 00.Input_data_format.ipynb
│── Tutorial_1.Spatial_Imputation_Using_Tangram.ipynb
│── Tutorial_2a.GRN_pycisTopic.ipynb
│── Tutorial_2b.GRN_pycisTarget.ipynb
│── Tutorial_2c.GRN_SCENIC+.ipynb
│── Tutorial_3.Impute_spatial_RAS.ipynb
└── README.md
```

## Requirements

- Python
- Scanpy
- AnnData
- Tangram
- pycisTopic
- pycisTarget
- SCENIC+

See individual notebooks for implementation details and dependencies.

## Input Data

- snMultiome data (gene expression and chromatin accessibility)
- Xenium spatial transcriptomics data
- Genome annotation and regulatory motif databases

See `00.Input_data_format.ipynb` for input data preparation.

## Citation

Please cite the relevant software packages and associated publications when using this workflow.


For questions or suggestions, please open a GitHub issue.
