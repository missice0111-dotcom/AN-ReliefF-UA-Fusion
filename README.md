# AN-ReliefF and UA-Fusion

Adaptive Neighborhood ReliefF and uncertainty-aware probability-level fusion for breast cancer molecular subtyping from mRNA and DNA methylation.

This repository distributes the final main-analysis research code as a complete source archive. The archive preserves the Python package, scientific configurations, frozen partitions, feature identifiers, aggregate reference results, and documentation in their original directory structure.

## Download and installation

Download [release_main_0.3.0.zip](release_main_0.3.0.zip) and its [SHA256 checksum](release_main_0.3.0.zip.sha256). Extract the archive and enter the `release_main_0.3.0` directory. Follow its `README.md` for environment installation, accepted inputs, and the `prepare`, `train`, `summarize`, and `bootstrap` commands. The package version is `0.3.0`.

The source archive contains 59 files. Its `FILE_MANIFEST.tsv` lists the size and SHA256 of the other 58 files. No additional software is installed or any experiment executed by simply downloading this archive.

## Included scope

- Final 738-patient TCGA-BRCA analysis of Luminal A, Luminal B, HER2-enriched, and Basal-like subtypes.
- Fold-fitted preprocessing and ANOVA, Standard ReliefF and AN-ReliefF, omics-specific XGBoost, ordinary stacking and UA-Fusion, and strict base-model out-of-fold construction.
- Three repetitions of five-fold outer cross-validation with three-fold inner cross-validation. The complete final candidate banks and selection rules are retained.
- Frozen cohort/sample mappings and partitions, selected feature identifiers, final parameters, aggregate reference results, and the final paired patient-level Bootstrap implementation.

Historical exploratory model screening and abandoned workflows are excluded. Molecular matrices, the subtype workbook, fitted models, patient-level predictions, private records, and original Git history are not included. Gaussian robustness, PAM50 exclusion, enrichment, and other supplemental analysis code are outside this main-analysis release.

## Data and verification

The author confirms that the study data were downloaded from the UCSC-hosted TCGA Pan-Cancer resource. Exact historical dataset endpoints and some acquisition/export steps remain unresolved; see `DATA_ACCESS.md` inside the source archive for the input contract and remaining provenance gaps.

The package documents installation, build, interface, source-equivalence, and privacy checks. Full experimental reproduction has not been run during release preparation. Existing reference results are supplied without recomputation. Read `VALIDATION.md` inside the archive for the precise check boundaries.

## Associated manuscript

Bing Zheng, Chunli Li, and Xiaoxia He. *Adaptive Neighborhood ReliefF and Uncertainty-Aware Multi-Omics Fusion for Breast Cancer Molecular Subtyping.*

This entry does not assert a published article DOI. Citation information is included in the source archive.

## License

Copyright (c) 2026 Bing Zheng. The primary research code is provided under the [MIT License](LICENSE.md). Separately installed dependencies retain their respective licenses; see `THIRD_PARTY_NOTICES.md` in the source archive. The code license does not assign a license to TCGA data.
