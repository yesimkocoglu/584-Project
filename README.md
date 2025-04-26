# 584-Project

# Aspect-Enhanced Transformer Models for Predicting Peer Review Acceptance

## Project Overview

This project investigates the use of transformer-based models, particularly SciBERT, for predicting paper acceptance decisions based on peer review texts. By incorporating aspect annotations such as originality, soundness, clarity, and motivation, we aim to enhance prediction accuracy over baselines that use raw review text alone.

The work is conducted as part of the final project for IS 584: Deep Learning for Text Analytics at METU Graduate School of Informatics.

## Research Questions

- **RQ1**: Does incorporating fine-grained aspect annotations into transformer-based models significantly improve the prediction accuracy of peer-review acceptance decisions?
- **RQ2**: Which specific review aspects are the strongest indicators influencing the acceptance decision?

## Dataset

We use the Aspect-Enhanced Peer Review dataset, which includes:

- Reviews and meta-reviews from ICLR (2017-2020) and NIPS (2016-2019).
- Acceptance decisions (Accept/Reject).
- Aspect annotations for review sentences (Summary, Originality, Soundness, Clarity, etc.).

Data is stored under `data/` (not uploaded to GitHub due to size restrictions).

## Methodology

- Fine-tune **SciBERT** on review texts with aspect information.
- Compare performance with baseline BERT models.
- Address long review sequences using techniques inspired by **Longformer**.
- Evaluate using Accuracy, F1-Score, and ROC-AUC.

## Structure

584-Project/ ├── README.md ├── requirements.txt ├── data/ │ ├── raw/ # Raw downloaded data │ └── processed/ # Preprocessed datasets ├── notebooks/ │ ├── 01_EDA.ipynb # Exploratory data analysis │ └── 02_Modeling.ipynb # Model training and evaluation ├── src/ │ ├── data_loading.py # Scripts for loading and preprocessing │ ├── modeling.py # Model definition and training scripts │ └── utils.py # Utility functions ├── reports/ │ └── phase1_proposal.pdf # Submitted reports └── figures/ # Visualizations and figures



