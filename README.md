# Plant Disease Prediction & Advisory System

An AI-powered system that detects plant leaf diseases using computer vision and provides explainable, crop-specific treatment recommendations grounded in authoritative agricultural sources.
---

## 📌 Problem Statement

Plant diseases significantly reduce crop yield and farmer income.
Early and accurate detection combined with reliable advisory support is essential for sustainable agriculture.
---
## This project provides:

📷 Disease detection from leaf images

📊 Severity estimation

📖 Evidence-grounded treatment recommendations

🌦 Optional environmental context integration
---
## 🧠 System Overview
Leaf Image
   ↓
CNN Disease Classifier
   ↓
Severity Estimation
   ↓
Advisory Engine (Rule / Retrieval-Based)
   ↓
Farmer-Friendly Recommendation
---
## 🔍 Disease Classification

The system is trained on the PlantVillage dataset, covering:

Apple

Blueberry

Cherry

Corn (Maize)

Grape

Orange

Peach

Pepper (Bell)

Potato

Raspberry

Soybean

Squash

Strawberry

Tomato

Including fungal, bacterial, viral, pest-related, and healthy classes.

Example Classes

Tomato___Early_blight

Potato___Late_blight

Apple___Black_rot

Tomato___Tomato_Yellow_Leaf_Curl_Virus

Grape___Leaf_bligh
---

## 🧠 Model Architecture

Convolutional Neural Network (CNN)

Transfer learning (i used: e.g., MobilenetV2 / EfficientNet)

Softmax multi-class classification

Confidence-based prediction

Severity Estimation

Severity is estimated using:

Leaf segmentation (using HSV in openCv)

Infected region ratio (pixel-based)
---

## 📖 Advisory Engine

The system does not generate random advice.

Instead, it uses:

Curated agricultural guidelines

FAO & ICAR references

Instead of Rule-based logic i implement here RAG Based Chatbot Style Programme
Crop-specific filtering
---
### Why Not Generative AI?

Agriculture is safety-critical.
To ensure reliability and prevent hallucinated recommendations:

Advice is deterministic

Sources are traceable

No free-form generation is used
---
## ⚙️ Technology Stack

Python

TensorFlow 

OpenCV

FastAPI (for inference API)

NumPy / Scikit-learn

FAISS (for retrieval-based advisory used)
---
## Future Prospect
Later i will improve its features and add some Advance Features 
i will inform all about later
---


## Auther
Name - Joydeep Biswas
From - Kalyani Government Engineering College , Nadia , West Bengal