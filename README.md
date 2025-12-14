## Team Project: Applying computer vision methods to data

# 🌿 Plant Disease Classification with EfficientNet and XAI  
### Leaf Segmentation · Domain Gap Reduction · Explainable AI

## 🔍 Overview
This repository implements a complete pipeline for plant-disease image preprocessing, classification, and interpretability.  
We use two widely adopted datasets—**PlantVillage** and **PlantDoc**—and propose a **class-dependent leaf segmentation** pipeline that reduces domain discrepancy between clean laboratory images and real-world field images.

We train **EfficientNet** models on the processed datasets and provide **XAI-based interpretation** using Grad-CAM and related attribution methods.

---

## 📁 Project Structure
├── demo.ipynb
├── preprocessing/
│ └── segmentation_final.ipynb/
├── checkpoints/
│ ├── doc_model_best.pt
│ └── village_model_best.pt
├── samples/
│ ├── Potato_Early_blight.JPG
│ └── Tomato_leara_late_blight.jpg
├── results/
│ ├── PlantDoc-Result/
│ |  └── Demo_Tomato_leaf_late_blight.jpg
│ └── PlantVillage-Result/
│    └── Demo_Potato_Early_blight.JPG
├── requirements.txt
└── README.md

## Contributors
- Minji Kim
- Gayoung Kim
- Seun Kim
