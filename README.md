# AMR Gene Detection Pipeline (StarAMR + AMRFinderPlus)

## 📍 Project Overview
This project demonstrates a small antimicrobial resistance (AMR) gene detection workflow using:
- **StarAMR** (ResFinder database search)
- **NCBI BLAST**
- (Attempted) **AMRFinderPlus** database installation

The goal is to detect known AMR genes from downloaded bacterial genomes (`.fna`) and summarize resistance predictions.

---

## 🧪 Tools Used
- StarAMR v0.4.0
- BLASTN v2.17.0+
- Biopython
- Conda (Miniconda)
- Linux/WSL environment

---

## 📂 Dataset
Genomes were downloaded from NCBI as `.fna` files and stored in:


Example genomes:
- `GCF_000005845.2_ASM584v2_genomic.fna`
- `GCF_000008865.2_ASM886v2_genomic.fna`
- `GCF_000013305.1_ASM1330v1_genomic.fna`

---

## ⚙️ Workflow Summary

### 1 Activate environment
```bash
conda activate staramr_env

2. staramr db update -d
staramr db info

3. cd data/raw_genomes
staramr search -o ../../data/results/staramr/staramr_all_results *.fna

