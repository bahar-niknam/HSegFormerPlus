# HSegFormer-
HSegFormer+: Hybrid CNN–Transformer With Stage Attention for Brain Tumor MRI Segmentation

This repository provides the implementation of **HSegFormer+**, a hybrid deep learning framework developed for automatic brain tumor segmentation in contrast-enhanced T1-weighted MRI.

The associated manuscript is currently under submission. Detailed architectural descriptions and experimental analyses will be made publicly available after publication.

---

## Overview

Accurate tumor delineation from MRI is essential for diagnosis, treatment planning, and follow-up assessment. However, segmentation remains challenging due to heterogeneous tumor appearance, weak boundaries, and variability across acquisition settings.

HSegFormer+ adopts a hybrid encoder–decoder segmentation strategy that integrates convolutional representations with transformer-based contextual modeling to improve robustness and segmentation quality while maintaining practical inference efficiency.

---

## Architecture Overview

<p align="center">
  <img src="figures/architecture.png" width="95%">
</p>

The framework combines complementary feature representations within a unified segmentation pipeline to produce accurate tumor masks across diverse MRI data conditions.

---

## Repository Structure

