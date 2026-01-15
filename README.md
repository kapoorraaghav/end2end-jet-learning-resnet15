End2end-jet-learning-resnet15
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
JetVision is a deep learning research project focused on jet image classification and regression using both supervised learning and self-supervised representation learning.
The project benchmarks a ResNet-15 architecture trained from scratch against self-supervised pretraining approaches, analyzing performance, generalization, and stability on high-energy physics jet datasets.

# This repository is designed as a reproducible research codebase and serves as prior work relevant to GSoC-style projects in scientific machine learning.

# Project Motivation
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Jet images provide a powerful 2D representation of particle jets in high-energy physics.
While self-supervised learning (SSL) has shown promise in reducing reliance on labels, its benefits over strong supervised baselines remain an open research question.

This project aims to:

Study whether SSL improves downstream performance on jet images

Compare scratch vs SSL-pretrained models fairly

Evaluate both classification and regression tasks under identical settings

# Methodology
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Model Architecture

ResNet-15 (lightweight CNN tailored for jet images)

Training Paradigms

Supervised Learning

Trained directly on labelled jet image datasets

Self-Supervised Learning (SSL)

Pretraining on unlabelled jet images using contrastive / representation learning schemes

Fine-tuning on downstream tasks with low learning rate

# Tasks
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Binary Classification (jet tagging)

Regression (continuous jet properties)

# Evaluation Metrics
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Classification

ROC Curve

AUC Score

Regression

# Prediction vs Ground Truth plots
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Error analysis

 Notably, in some experimental settings, the model trained from scratch achieved better ROC/AUC than its SSL-pretrained counterpart — a key insight discussed in this work.
