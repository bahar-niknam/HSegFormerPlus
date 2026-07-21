# HSegFormer+

> **A Hybrid CNN–Transformer model with Stage-wise Cross-Attention for Brain Tumor MRI Segmentation**

HSegFormer+ is a hybrid deep learning model for automatic brain tumor segmentation in magnetic resonance imaging (MRI). The proposed architecture integrates convolutional neural networks and vision transformers through a stage-wise cross-attention mechanism to jointly exploit local anatomical details and global contextual representations.

The associated manuscript is currently under peer review. The source code, pretrained models, and training scripts will be released after the review process is completed.

---

## Overview

HSegFormer+ is a hybrid CNN–Transformer framework developed for brain tumor MRI segmentation. The proposed architecture integrates a SegFormer-B5 transformer encoder and a ResNet-50 CNN encoder through progressive stage-wise cross-attention, allowing complementary local and global feature representations to be learned across multiple encoding stages.

The fused features are further refined using lightweight residual refinement blocks and progressively decoded through an attention-guided decoder with ASPP-based multi-scale contextual aggregation. The framework supports both binary and multi-class segmentation and has been evaluated on the BraTS 2021, Figshare, and BRISC 2025 datasets.

---

## Framework

<p align="center">
<img src="Proposed-Model.png" width="95%">
</p>

The proposed framework consists of the following components:

- **Dual-Path Encoder**
  - SegFormer-B5 Transformer encoder
  - ResNet-50 CNN encoder

- **Stage-wise Cross-Attention Fusion**
  - Progressive interaction between CNN and Transformer features at multiple encoding stages

- **Feature Refinement Block (FRB)**
  - Lightweight residual refinement of fused feature representations

- **Attention-Guided Decoder**
  - Progressive multi-scale feature reconstruction with attention gates

- **ASPP Module**
  - Multi-scale contextual aggregation before the prediction layer

- **Prediction Head**
  - Supports both binary and multi-class segmentation tasks

For the BraTS 2021 dataset, the framework supports a **2.5D input representation**, while conventional **2D image inputs** are used for the Figshare and BRISC 2025 datasets.

---

## Experimental Evaluation

The proposed framework has been evaluated on three publicly available brain MRI datasets:

- BraTS 2021
- Figshare Brain Tumor Dataset
- BRISC 2025

The manuscript reports quantitative comparisons, ablation studies, qualitative visualizations, and stability analysis across these datasets.

---

## Research Topics

- Brain Tumor Segmentation
- Medical Image Analysis
- Deep Learning
- Hybrid CNN–Transformer Networks
- Cross-Attention
- Medical Vision Transformers
- Multi-scale Feature Learning

---

## Repository Status

The repository currently provides:

- Project overview
- Network architecture
- Framework description

The complete implementation, pretrained weights, training scripts, and usage examples will be released in a future update.

---

## License

The license information will be added when the repository is publicly released.















