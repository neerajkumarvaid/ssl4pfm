---
layout: default
title: Phase 1
permalink: /phase1/
---

# Phase 1: Foundation Model Development

**Duration**: June - October 2025  
**Objective**: Develop self-supervised learning approaches for pathology foundation models

## MSK-SLCPFM Dataset

The Phase 1 dataset provides participants with unprecedented access to the MSK-SLCPFM collection - the largest pathology dataset ever assembled for competition purposes.

### Dataset Specifications
- **Scale**: ~300 million pathology image tiles
- **Source**: 51,578 whole slide images (WSIs)  
- **Coverage**: 39 cancer types
- **Origins**: TCGA, CPTAC, and MSK repositories
- **Scanner Diversity**: Multiple vendors (Aperio, Hamamatsu, Leica, Parmana, Phillips)

### Data Composition

| Source | Number of WSIs |
|--------|----------------|
| TCGA | 10,438 |
| CPTAC | 6,004 |
| MSK | 34,690 |
| **Total** | **51,132** |

## Multi-Resolution Tile Formats

To capture multi-scale tissue contexts essential for pathological analysis, the dataset includes three distinct tile formats:

1. **224 × 224 pixel tiles** from 20× WSIs (0.5μm²/pixel)
2. **448 × 448 pixel tiles** from 40× WSIs (0.25μm²/pixel)  
3. **1024 × 1024 pixel tiles** from 20× WSIs with independent coordinates

This strategic sampling approach facilitates hierarchical tissue structure learning across varying magnifications, mimicking the multi-resolution examination methodology employed by pathologists.

## Complete Cancer Types Distribution

The dataset spans all 39 cancer types with the following distribution:

| # | Cancer Type | Abbreviation | TCGA | CPTAC | MSK | **Total** |
|---|-------------|-------------|------|-------|-----|-----------|
| 1 | Adrenocortical Carcinoma | ACC | 79 | 0 | 50 | **129** |
| 2 | Anal Squamous Cell Carcinoma | ANSC | 0 | 0 | 50 | **50** |
| 3 | Appendiceal Cancer | APAD | 0 | 0 | 50 | **50** |
| 4 | Bladder Urothelial Carcinoma | BLCA | 412 | 0 | 2,000 | **2,412** |
| 5 | Bone Cancer | BOCA | 0 | 0 | 50 | **50** |
| 6 | Breast Invasive Carcinoma | BRCA | 1,097 | 0 | 3,000 | **4,097** |
| 7 | Cervical Squamous Cell Carcinoma | CESC | 307 | 0 | 200 | **507** |
| 8 | Cholangiocarcinoma | CHOL | 45 | 0 | 1,000 | **1,045** |
| 9 | Colon Adenocarcinoma | COAD | 461 | 0 | 3,000 | **3,461** |
| 10 | Lymphoid Neoplasm Diffuse Large B-cell Lymphoma | DLBC | 58 | 0 | 500 | **558** |
| 11 | Esophageal Carcinoma | ESCA | 185 | 0 | 200 | **385** |
| 12 | Gastrointestinal Stromal Sarcoma | GIST | 0 | 0 | 500 | **500** |
| 13 | Glioblastoma Multiforme | GBM | 528 | 462 | 1,000 | **1,990** |
| 14 | Head and Neck Squamous Cell Carcinoma | HNSC | 478 | 390 | 500 | **1,368** |
| 15 | Kidney Chromophobe | KICH | 113 | 0 | 50 | **163** |
| 16 | Kidney Renal Clear Cell Carcinoma | KIRC | 537 | 783 | 1,000 | **2,320** |
| 17 | Kidney Renal Papillary Cell Carcinoma | KIRP | 292 | 0 | 100 | **392** |
| 18 | Brain Lower Grade Glioma | LGG | 594 | 0 | 1,000 | **1,594** |
| 19 | Liver Hepatocellular Carcinoma | LIHC | 377 | 0 | 200 | **577** |
| 20 | Lung Adenocarcinoma | LUAD | 585 | 1,139 | 2,000 | **3,724** |
| 21 | Lung Squamous Cell Carcinoma | LUSC | 539 | 1,081 | 500 | **2,120** |
| 22 | Mesothelioma | MESO | 87 | 0 | 200 | **287** |
| 23 | Ovarian Serous Cystadenocarcinoma | OV | 439 | 0 | 2,000 | **2,439** |
| 24 | Pancreatic Adenocarcinoma | PAAD | 185 | 557 | 3,000 | **3,742** |
| 25 | Pheochromocytoma and Paraganglioma | PCPG | 179 | 0 | 20 | **199** |
| 26 | Prostate Adenocarcinoma | PRAD | 498 | 0 | 3,000 | **3,498** |
| 27 | Rectum Adenocarcinoma | READ | 170 | 0 | 1,000 | **1,170** |
| 28 | Salivary Gland Cancer | SACA | 0 | 0 | 200 | **200** |
| 29 | Sarcoma (non-GIST) | SARC | 261 | 300 | 2,000 | **2,561** |
| 30 | Skin Cutaneous Melanoma | SKCM | 469 | 404 | 1,000 | **1,873** |
| 31 | Small Bowel Cancer | SBC | 0 | 0 | 50 | **50** |
| 32 | Stomach Adenocarcinoma | STAD | 443 | 0 | 1,000 | **1,443** |
| 33 | Testicular Germ Cell Tumors | TGCT | 150 | 0 | 500 | **650** |
| 34 | Thyroid Carcinoma | THCA | 507 | 0 | 1,000 | **1,507** |
| 35 | Thymoma | THYM | 124 | 0 | 20 | **144** |
| 36 | Uterine Corpus Endometrial Carcinoma | UCEC | 548 | 888 | 2,000 | **3,436** |
| 37 | Uterine Carcinosarcoma | UCS | 57 | 0 | 200 | **257** |
| 38 | Uterine Sarcoma | USARC | 0 | 0 | 500 | **500** |
| 39 | Uveal Melanoma | UVM | 80 | 0 | 50 | **130** |
| | **TOTAL** | | **10,438** | **6,004** | **34,690** | **51,132** |

## 🎯 Your Challenge: Build the Next Generation of Pathology Foundation Models

**This competition is specifically designed for developing novel self-supervised learning algorithms and architectures to create powerful pathology foundation models.**

### What You'll Develop:
- **Self-supervised learning approaches** that can learn meaningful representations from pathology images without requiring labeled data
- **Novel neural network architectures** optimized for the unique characteristics of histopathology data
- **Foundation models** that can serve as powerful feature extractors for diverse downstream clinical tasks

### The Innovation Opportunity:
SLC-PFM focuses on **pre-training methodologies** - giving you the freedom to explore cutting-edge self-supervised techniques like:

- **Contrastive Learning**: SimCLR, MoCo, SwAV, VICReg
- **Self-Distillation**: DINO, DINOv2, BYOL
- **Masked Image Modeling**: MAE, iBOT, BEiT
- **Multi-Scale Learning**: Hierarchical representations across 20× and 40× magnifications
- **Pathology-Specific Innovations**: Novel augmentations, rotation invariance, cross-tile relationship modeling
- **Transformer Architectures**: Vision Transformers (ViTs) optimized for gigapixel pathology images

**No labels. No supervision. Pure algorithmic innovation.**

Design self-supervised learning frameworks that extract clinically meaningful patterns from 300M pathology images to create foundation models that will advance cancer diagnosis worldwide.

## Technical Requirements

### Development Environment
- Participants use their own computational infrastructure
- Self-supervised learning approaches without outcome labels
- Focus on developing generalizable pathology foundation models

### Submission Requirements
By **October 15, 2025**, teams must provide:

1. **Foundation Model Checkpoint**: Trained model weights
2. **Feature Extraction Code**: Python implementation for inference  
3. **Methodology Documentation**: LaTeX-formatted technical description

### Performance Requirements
- Submiited models must run feature extraction (inference) on a **single GPU with ≤80GB memory**
- Efficient feature extraction for downstream task evaluation

## Data Distribution Options
- Secure link will be provided to access Phase 1 dataset after registration verification

### Starting Kit (Available in June 2025 only to registered participants)
The comprehensive Starting Kit will include:
1. **Phase 1 Dataset**: Complete MSK-SLCPFM collection
2. **Data Loading Scripts**: Python code for loading, inspecting, and preprocessing WSI and tile data
3. **Documentation**: Detailed guides on dataset structure and submission requirements
4. **Submission Resources**: Templates for inference code (Python) and algorithm descriptions (LaTeX)

## Unique Challenges of Pathology Data

The MSK-SLCPFM dataset presents unique challenges compared to natural image datasets:

### Limited Color Variation
- H&E staining constrains colors to blue-purple (nuclei) and pink (cytoplasm/matrix)
- Different from rich color variation in natural images

### Rotational Invariance
- Microscopic structures (nuclei, cells, glands) appear in arbitrary orientations
- No canonical orientation unlike objects in natural images

### Non-IID Samples
- Tiles from same WSI are not completely independent samples
- Contrasts with ImageNet where images are Independent and Identically Distributed

### Multi-Resolution Context
- Tissue details vary significantly across magnifications
- Glands appear larger with more cellular details at 40× vs 20× resolution
- Important pathological features may only be visible at specific magnifications


## Data Ethics and Privacy

- All competition data has been de-identified
- Approved for research use under respective institutional IRB protocols
- Complies with HIPAA regulations
- Usage restricted to non-commercial academic research
- No patient overlap between Phase 1 and Phase 2 datasets

---

**Questions about Phase 1?** Contact: [slcpfm2025@gmail.com](mailto:slcpfm2025@gmail.com)
