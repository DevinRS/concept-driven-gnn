# Concept-Driven Disentanglement for Interpretable SC-FC Coupling

[cite_start]This repository contains the code for the paper: **"A Concept-Driven Disentanglement Framework for Interpretable Graph Neural Networks in Structure-Function Coupling"**[cite: 617].

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](LINK_TO_YOUR_NOTEBOOK)

## 📄 Abstract
Graph Neural Networks (GNNs) excel at predicting brain functional connectivity (FC) from structural connectivity (SC) but often lack interpretability. [cite_start]We propose a **Concept-Driven Disentanglement Framework** that uses an ensemble of architecturally biased GNN branches[cite: 625]. [cite_start]This design enforces disentangled embeddings (e.g., "Strong vs. Weak" connections) and allows for quantitative hypothesis testing using SHAP[cite: 627].

## 🧠 Framework
The model filters the input SC matrix based on predefined neuroscientific concepts before passing them to specialized GNN branches.

![Framework Overview](figures/framework_diagram.png)
[cite_start]*(Note: Upload Figure 1 from your PDF here [cite: 733])*

## 🧪 Experiments
We provide notebooks to replicate the three core experiments from the paper:
1. [cite_start]**Weak vs. Strong Connections:** Demonstrating that strong connections (the "backbone") drive static FC prediction[cite: 866, 1000].
2. [cite_start]**Short vs. Long Range:** Investigating the impact of fiber length on predictive accuracy[cite: 902].
3. [cite_start]**Normal vs. Outlier:** Assessing the role of rare, high-deviation edges[cite: 908].

## 📂 Dataset
[cite_start]This project uses the **MICA-MICS dataset**[cite: 668]. 
- [cite_start]We provide the processing scripts to generate the $116 \times 116$ Schaefer parcellated matrices used in the study[cite: 670].
- Raw data must be requested/downloaded from the [MICA-MICS repository](https://data.mics.mcgill.ca/).

## 📦 Requirements
* `torch`
* `torch_geometric` (for GCNConv layers)
* `shap`
* `numpy` / `pandas`

## 📚 Citation
[Insert Citation Here once published]
