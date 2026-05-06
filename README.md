# MDAF++: Noise-Space Adaptive Multi-Domain Filtering

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Journal: Applied Research](https://img.shields.io/badge/Journal-Applied_Research-blue)](https://onlinelibrary.wiley.com/journal/27670163)

This repository contains the official implementation of the framework proposed in:  
**"Noise-Space Adaptive Multi-Domain Filtering: A Unified Framework for Low-Light Urban Surveillance and Medical Retinal Imaging"** (Submitted to *Applied Research*, Wiley).

## 🚀 Overview
MDAF++ is a unified filtering framework designed to handle heterogeneous noise across different imaging domains without retraining. It addresses the gap between urban low-light enhancement and medical anatomical preservation[cite: 1].

### Key Innovations:
*   **Automatic Domain Detection:** Analyzes input imagery to switch between urban and medical pipelines[cite: 1].
*   **Noise-Space Adaptation:** Dynamically adjusts filtering kernels based on wavelet-based noise estimation[cite: 1].
*   **Vessel-Aware Branch:** Specialized preservation for retinal vasculature in medical imaging[cite: 1].
*   **Multi-Scale Frequency Fusion:** Leverages wavelet-domain thresholding for detail conservation[cite: 1].

## 📂 Repository Contents
*   `MDAF.ipynb`: The complete end-to-end pipeline including:
    *   Dataset loading (ExDark, LOL-v2, DRIVE, STARE)[cite: 1].
    *   Proposed MDAF++ core algorithm[cite: 1].
    *   Comprehensive evaluation metrics (PSNR, SSIM, Vessel Sensitivity, ENR)[cite: 1].
    *   Statistical significance testing (ANOVA and Cohen’s d)[cite: 1].

## 🛠️ Requirements
The code is designed to run in **Google Colab** or **Kaggle** environments. Required libraries include:
*   `opencv-python`
*   `PyWavelets`
*   `scikit-image`
*   `torch` (for NIQE metric)
*   `pandas`, `numpy`, `matplotlib`

## 📊 Results Snapshot
| Domain | Key Metric | Result |
| :--- | :--- | :--- |
| **Medical** | Vessel Sensitivity | 0.71 (on DRIVE)[cite: 1] |
| **Urban** | Efficiency | ~45ms per 512x512 image [cite: 1] |

## 📝 Citation
```bibtex
@article{haque2026noise,
  title={Noise-Space Adaptive Multi-Domain Filtering: A Unified Framework for Low-Light Urban Surveillance and Medical Retinal Imaging},
  author={Haque, Md Mominul and Mahamad, Saipunidzam and Sulaiman, Suziah and Balogun, Abdullateef Oluwagbemiga},
  journal={Applied Research},
  year={2026}
}
