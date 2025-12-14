# 🌿 Plant Disease Classification with EfficientNet and XAI
### Leaf Segmentation · Domain Gap Reduction · Explainable AI

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange)
![EfficientNet](https://img.shields.io/badge/Model-EfficientNet--B1-green)

---

## 🔍 Overview
This repository implements a complete pipeline for **plant disease classification** and **model interpretability**.

We address the domain discrepancy between laboratory images (**PlantVillage**) and real-world field images (**PlantDoc**) by proposing a **class-dependent leaf segmentation** pipeline.

We train **EfficientNet-B1** models on the processed datasets and utilize **XAI (Explainable AI)** methods—**Grad-CAM**, **Score-CAM**, and **Layer-CAM**—to visually verify whether the model focuses on the correct disease lesions.

### Key Features
- **Domain Gap Reduction:** Segmentation-based preprocessing to isolate leaves from complex backgrounds.
- **Efficient Classification:** Fine-tuned EfficientNet-B1 for robust performance on small datasets.
- **Explainability (XAI):** Attention visualization (Grad-CAM / Score-CAM / Layer-CAM) to improve reliability.

---

## 📁 Project Structure

```bash
├── demo.ipynb                     # Demo notebook for running XAI (Grad-CAM, etc.)
├── preprocessing/
│   └── segmentation_final.ipynb   # Preprocessing & segmentation pipeline
├── checkpoints/
│   ├── doc_model_best.pt          # Trained model for PlantDoc
│   └── village_model_best.pt      # Trained model for PlantVillage
├── samples/                       # Test images for demo
│   ├── Potato_Early_blight.JPG
│   └── Tomato_leaf_late_blight.jpg
├── results/                       # Saved XAI results
│   ├── PlantDoc-Result/
│   └── PlantVillage-Result/
├── requirements.txt               # Python dependencies
└── README.md
```

## 🛠️ Installation

### 1) Clone the repository
```bash
git clone https://github.com/YOUR_GITHUB_ID/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```
### 2) Install dependencies (Python 3.8+ recommended)
```bash
pip install -r requirements.txt
```

## 🚀 How to Run Demo
1. Check model & data

	Ensure the .pt model files are located in the checkpoints/ directory.
2. Run the notebook
    ```bash
    jupyter notebook demo.ipynb
    ```
3. 	View results
    After running the notebook, the original image and its corresponding heatmaps (Grad-CAM, Score-CAM, Layer-CAM) will be saved in the results/ directory.

## 👥 Contributors
Minji Kim

Gayoung Kim

Seun Kim