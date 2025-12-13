## Team Project: Applying computer vision methods to data

# 🌿 Plant Disease Classification with EfficientNet and XAI  
### Leaf Segmentation · Domain Gap Reduction · Explainable AI

## 🔍 Overview
This repository implements a complete pipeline for plant-disease image preprocessing, classification, and interpretability.  
We use two widely adopted datasets—**PlantVillage** and **PlantDoc**—and propose a **class-dependent leaf segmentation** pipeline that reduces domain discrepancy between clean laboratory images and real-world field images.

We train **EfficientNet** models on the processed datasets and provide **XAI-based interpretation** using Grad-CAM and related attribution methods.

---

## 📁 Project Structure
├── data/
│ ├── PlantVillage/
│ └── PlantDoc/
├── preprocessing/
│ └── segmentation_final.ipynb/
├── models/
│ ├── efficientnet_train.py
│ ├── efficientnet_eval.py
│ └── xai/
│ ├── gradcam.py
│ └── visualization.py
├── experiments/
│ ├── training_logs/
│ ├── results/
│ └── xai_maps/
└── README.md

## Contributors
Minji Kim
Gayoung Kim
Seun Kim
