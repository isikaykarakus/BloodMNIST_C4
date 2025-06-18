# BloodMNIST Classification Project

This repository contains the final project for the *Machine Learning for Human Data* course at the University of Padova. The project focuses on designing, implementing, and evaluating a series of convolutional neural network (CNN) architectures for blood cell classification using the BloodMNIST dataset.

---

## Project Structure
```
📁 notebook/
└─ BloodMNIST_C4_IsikayKarakus.ipynb – Final Colab notebook with all training, evaluation, and visualisation code
📁 report/
└─ Karakus.pdf – Final LaTeX report with detailed results and analysis
└─BloodMNIST_C4_IsikayKarakus.pdf - Final project presentation
📄 README.md
└─ This file
```

---

## Dataset
- **Source**: [MedMNIST v2 – BloodMNIST](https://zenodo.org/records/10519652)
- **Image Sizes**: 64×64 and 128×128 RGB
- **Classes**: 8 peripheral blood cell types
- **Format**: `.npz` 

---

## Models Implemented
| Model Variant             | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| **Baseline CNN**          | Shallow CNN with 3–4 Conv2D layers, BatchNorm, MaxPooling, Dropout          |
| **Baseline + Augmentation** | Baseline CNN enhanced with data augmentation strategies                    |
| **U-Net Inspired CNN**    | Encoder-based architecture with global average pooling and dense layers     |
| **Inception CNN**         | Multi-scale feature extraction using custom Inception blocks                |
| **Skip Connection CNN**   | Residual CNN inspired by ResNet, offering high generalisation performance   |
| **Inception + Skip CNN**  | Hybrid model combining Inception blocks and skip connections                |

---

## Evaluation Metrics
- Overall test accuracy
- Macro-averaged precision, recall, and F1-score
- Class-wise performance analysis
- Confusion matrix
- Model complexity (parameter count, memory footprint)
- Training and inference time

---

## How to Run
Open in **Google Colab**:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h9BRGG5LXs4-4bFlz_fW9WpD_VR7FGFf?usp=sharing)

Or run locally:
```bash
git clone https://github.com/isikaykarakus/BloodMNIST_C4.git
cd BloodMNIST_C4
pip install -r requirements.txt
```

---

## Author
- Işıkay Karakuş – University of Padova (ID: 2071938)

---

## Final Report
The final report summarising all findings, model comparisons, and class-wise analysis is located under the `report/` directory. It includes:
- Architectural summaries
- Evaluation tables and graphs
- Confusion matrices
- Concluding analysis and future work

