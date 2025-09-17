# IBD Spatial ML Pipeline

This repository hosts the **arXiv preprint** describing our explainable machine learning pipeline for classifying **Inflammatory Bowel Disease (IBD)** using **spatial transcriptomics** data.

> **Engineering Spatial and Molecular Features from Cellular Niches to Inform Predictions of Inflammatory Bowel Disease**  
> [https://arxiv.org/abs/2509.09923](https://arxiv.org/abs/2509.09923)

---

## Description

We introduce a computational framework that leverages spatial transcriptomics to classify IBD subtypes, **Crohn’s disease (CD)** and **ulcerative colitis (UC)**.  
Our approach combines:
- **Cell2location mapping** to assign cell types using scRNA-seq reference data,  
- **Non-negative matrix factorization (NMF)** to identify recurring cellular niches,  
- **Feature engineering** of spatial and molecular signals, and  
- **A multilayer perceptron (MLP)** classifier to predict and explain disease state.

The pipeline transforms complex tissue data into interpretable features, providing insights into both **tissue architecture** and **molecular mechanisms** driving disease.

---

## Abstract

Differentiating between the two main subtypes of Inflammatory Bowel Disease (IBD): Crohn’s disease (CD) and ulcerative colitis (UC) is a persistent clinical challenge due to overlapping presentations. This study introduces a novel computational framework that employs spatial transcriptomics (ST) to create an explainable machine learning model for IBD classification. We analyzed ST data from the colonic mucosa of healthy controls (HC), UC, and CD patients. Using Non-negative Matrix Factorization (NMF), we first identified four recurring cellular niches, representing distinct functional microenvironments within the tissue. From these niches, we systematically engineered 44 features capturing three key aspects of tissue pathology: niche composition, neighborhood enrichment, and niche-gene signals. A multilayer perceptron (MLP) classifier trained on these features achieved an accuracy of $0.774 \pm 0.161$ for the more challenging three-class problem (HC, UC, and CD) and $0.916 \pm 0.118$ in the two-class problem of distinguishing IBD from healthy tissue. Crucially, model explainability analysis revealed that disruptions in the spatial organization of niches were the strongest predictors of general inflammation, while the classification between UC and CD relied on specific niche-gene expression signatures. This work provides a robust, proof-of-concept pipeline that transforms descriptive spatial data into an accurate and explainable predictive tool, offering not only a potential new diagnostic paradigm but also deeper insights into the distinct biological mechanisms that drive IBD subtypes.

---

## Citation

If you use this work, please cite (BibTex):
```
@misc{tan2025engineeringspatialmolecularfeatures,
      title={Engineering Spatial and Molecular Features from Cellular Niches to Inform Predictions of Inflammatory Bowel Disease}, 
      author={Myles Joshua Toledo Tan and Maria Kapetanaki and Panayiotis V. Benos},
      year={2025},
      eprint={2509.09923},
      archivePrefix={arXiv},
      primaryClass={q-bio.GN},
      url={https://arxiv.org/abs/2509.09923}, 
}
```

