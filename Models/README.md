# Genomic Foundation Models for Cross-Modal Prediction

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

A curated collection of state-of-the-art deep learning models for genomic sequence analysis, with a focus on cross-modal learning from DNA to transcriptomic and proteomic data.

## 🧬 Overview

This repository documents and provides resources for foundational machine learning models that process raw DNA sequences. These models learn generalizable representations of genomic language and can be adapted (via fine-tuning or feature extraction) to predict downstream molecular phenotypes like RNA expression or protein abundance—enabling cross-modal prediction across omics layers.

## 📋 Model Catalog

| Model | Key Architecture | Sequence Length | Primary Training Data | Best For |
| :--- | :--- | :--- | :--- | :--- |
| **[DNABERT](https://github.com/jerryji1993/DNABERT)** | BERT Transformer (k-mer tokenization) | ~512 bp | Human genome (hg38) | Regulatory element classification, promoter prediction |
| **[DNABERT-2](https://github.com/MAGICS-LAB/DNABERT_2)** | BERT Transformer (byte-pair encoding) | Up to 10k bp | Multi-species genomes (GUE benchmark) | Efficient long-range context, cross-species tasks |
| **[Nucleotide Transformer](https://github.com/instadeepai/nucleotide-transformer)** | Transformer (various sizes) | Up to 1k bp | Human + 3,500 diverse species | Robust general-purpose genomic embeddings |
| **[HyenaDNA](https://github.com/HazyResearch/hyena-dna)** | Hyena (long convolutional filters) | **Up to 1M bp** | Human genome (hg38) | **Ultra-long context**, single-nucleotide resolution tasks |
| **[Evo](https://github.com/evo-design/evo)** | Striped Hyena (SSM + conv) | Up to 131k bp | Multi-scale (DNA, RNA, protein) | **Joint multi-modal** modeling & generation |

## 📊 Detailed Model Information

| Model | Publication Details | Code / Resources | Key Datasets Used |
| :--- | :--- | :--- | :--- |
| **DNABERT** | **Title:** DNABERT: pre-trained Bidirectional Encoder Representations from Transformers model for DNA-language in genome<br>**Authors:** Yanrong Ji, Zhihan Zhou, Han Liu, Ramana V. Davuluri<br>**Venue/Year:** *Bioinformatics*, 2021<br>**DOI:** [10.1093/bioinformatics/btab083](https://doi.org/10.1093/bioinformatics/btab083) | [GitHub Repository](https://github.com/jerryji1993/DNABERT) | Human reference genome (hg38), regulatory element benchmarks |
| **DNABERT-2** | **Title:** DNABERT-2: Efficient Foundation Model and Benchmark For Multi-Species Genome<br>**Authors:** Zhihan Zhou, Yanrong Ji, Weijian Li, Pratik Dutta, Ramana Davuluri, Han Liu<br>**Venue/Year:** ICLR 2024 (arXiv 2023)<br>**Preprint:** [arXiv:2306.15006](https://arxiv.org/abs/2306.15006) | [GitHub Repository](https://github.com/MAGICS-LAB/DNABERT_2) | Genomic Understanding Evaluation (GUE) benchmark, 100+ species |
| **Nucleotide Transformer** | **Title:** Nucleotide Transformer: building and evaluating robust foundation models for human genomics<br>**Authors:** InstaDeep Consortium et al.<br>**Venue/Year:** *Nature Methods*, 2025<br>**DOI:** [10.1038/s41592-024-02523-z](https://doi.org/10.1038/s41592-024-02523-z) | [GitHub Repository](https://github.com/instadeepai/nucleotide-transformer) | Human genome + 3,500 species, NCBI RefSeq |
| **HyenaDNA** | **Title:** HyenaDNA: Long-Range Genomic Sequence Modeling at Single Nucleotide Resolution<br>**Authors:** Eric Nguyen et al.<br>**Venue/Year:** NeurIPS 2023<br>**Preprint:** [arXiv:2306.15794](https://arxiv.org/abs/2306.15794) | [GitHub Repository](https://github.com/HazyResearch/hyena-dna) | Human reference genome (hg38) |
| **Evo** | **Title:** Sequence modeling and design from molecular to genome scale with Evo<br>**Authors:** Eric Nguyen et al.<br>**Venue/Year:** *Science*, 2024<br>**DOI:** [10.1126/science.ado9336](https://doi.org/10.1126/science.ado9336) | [GitHub Repository](https://github.com/evo-design/evo) | Multi-modal DNA, RNA, and protein sequences |

