# Prediction of Polo-Like Kinase 1 (PLK1) Inhibitor Bioactivity Using Transformer-Based Models

## Overview

This repository accompanies the study:

"Prediction of Polo-Like Kinase 1 Inhibitor Bioactivity as Anticancer Agent"

The study evaluates several Transformer-based architectures for predicting PLK1 inhibitor bioactivity using SMILES representations and compares their performance against an LSTM baseline.

## Dataset

The dataset consists of 3,248 compounds represented as canonical SMILES sequences with corresponding IC50 values.

The data were obtained from a publicly available GitHub repository containing compounds compiled from:

- ChEMBL
- PubChem

Dataset source:
[https://github.com/az09tuan/PLK1)]

## Models

### Baseline Model
- LSTM

### Transformer Models
- BERT-SMILES 1
- BERT-SMILES 2
- ChemBERTa 3
- PharmBERT 1
- PharmBERT 2

## Experimental Environment

Experiments were conducted using:

- Google Colab
- NVIDIA Tesla T4 GPU
- PyTorch
- Hugging Face Transformers
- Optuna

## Hyperparameter Optimization

Hyperparameter tuning was performed using Optuna GridSampler.

The search space included:

- Learning Rate
- Weight Decay
- Batch Size

A total of 18 parameter configurations were evaluated.

## Results

The best-performing model was ChemBERTa 3, achieving:

- Accuracy: 0.90625
- F1-score: 0.90397

## Reproducibility

This repository is provided to support transparency and reproducibility of the reported experiments. The dataset source, model configurations, and evaluation procedures are documented to facilitate future studies.

## Citation

[Paper citation]
