

# BloodMNIST Classification Project

This repository contains the final project for the *Machine Learning for Human Data* course at the University of Padova, focused on developing and evaluating custom deep learning models for blood cell image classification using the BloodMNIST dataset.

---

##  Project Structure
```
├── models/ # Model definitions (Baseline CNN, U-Net encoder)
├── notebooks/ # Jupyter/Colab notebooks
├── results/ # Plots, confusion matrices, model summaries
├── report/ # Final LaTeX report and figures
├── README.md # This file
└── requirements.txt # Environment dependencies
```


---

## Dataset

- **Source**: [MedMNIST v2 – BloodMNIST](https://zenodo.org/records/10519652)
- **Image Sizes**: 64x64, 128x128 (RGB)
- **Classes**: 8 blood cell types
- **Format**: `.npz` files with pre-split train/val/test sets

---

## Models

| Model Variant         | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| **Baseline CNN**      | A standard convolutional network with 3–4 Conv2D layers, BatchNorm, MaxPooling, and Dropout layers. Serves as a foundational model. |
| **Custom Encoder CNN**| A deeper model inspired by the encoder path of U-Net, adapted for image classification with global average pooling and dense output layers. |
| **Enhanced CNN (SE)** | The custom encoder model augmented with **Squeeze-and-Excitation (SE) blocks** to capture channel-wise attention and improve feature discrimination. |


---

## Evaluation

- Accuracy, precision, recall, F1-score
- Confusion matrix
- Training vs. validation loss/accuracy curves
- Training time, model complexity (#params)

---

## 📦 How to Run

You can open and run the notebook directly in **Google Colab**:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/isikaykarakus/BloodMNIST_C4/blob/main/notebooks/bloodmnist_main.ipynb)

Or clone the repo locally and run it:

```bash
git clone https://github.com/isikaykarakus/BloodMNIST_C4.git
cd BloodMNIST_C4
pip install -r requirements.txt
```
## Author
- Işıkay Karakuş 2071938 


