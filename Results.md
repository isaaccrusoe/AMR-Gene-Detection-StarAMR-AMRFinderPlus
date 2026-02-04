StarAMR summary output
data/results/staramr/staramr_all_results/summary.tsv
| Isolate ID                        | Genotype | Predicted Phenotype |
| --------------------------------- | -------- | ------------------- |
| GCF_000005845.2_ASM584v2_genomic  | None     | Sensitive           |
| GCF_000008865.2_ASM886v2_genomic  | None     | Sensitive           |
| GCF_000013305.1_ASM1330v1_genomic | None     | Sensitive           |
ResFinder output
data/results/staramr/staramr_all_results/resfinder.tsv
In this dataset, no AMR genes were detected under default thresholds.

Notes / Interpretation
StarAMR predictions are microbiological resistance predictions based on gene detection and curated databases.
They are not the same as clinical resistance interpretation, which depends on host, drug dosing, breakpoints, and phenotype testing.

Troubleshooting Log (Important!)
StarAMR + NumPy/Pandas compatibility issues
During testing, StarAMR produced errors due to modern library changes:
np.unicode_ removed in NumPy 2.0
DataFrame.append removed in pandas
Some output files were still generated successfully (summary + resfinder).

AMRFinderPlus database download issue
Database update failed due to SSL/network errors:
AMRFinderPlus database download issue

Database update failed due to SSL/network errors:
