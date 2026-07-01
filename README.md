# 🧠 Explainable AI for Alzheimer's MRI Classification

An industry-grade deep learning diagnostic tool built to classify stages of Alzheimer's disease from MRI scans. This project prioritizes clinical trust by featuring mathematically weighted loss functions and visual interpretability using HiResCAM.

## 📌 Project Overview
In medical AI, the "black box" problem prevents clinicians from trusting neural networks. This project tackles that issue by not only diagnosing the stage of dementia but also generating high-resolution heatmaps that prove the AI is focusing on anatomical brain structures (like the hippocampus and ventricles) rather than background noise.

### ⚙️ Key Engineering Features
* **Architecture:** ResNet-18 feature extractor fine-tuned specifically for medical imaging matrices.
* **Explainability (XAI):** Implemented HiResCAM (High-Resolution Class Activation Mapping) to generate element-wise pixel visualizations of model decision-making.
* **Imbalance Handling:** Utilized a Class-Weighted Cross-Entropy loss function to prevent the network from artificially inflating standard accuracy by ignoring minority classes.
* **Advanced Evaluation:** Validated using standard Accuracy alongside Macro F1-Score, Recall, and ROC-AUC for robust clinical validity.

## 📊 The Dataset
The model was trained on a standardized Alzheimer's MRI dataset encompassing 4 distinct progressive classifications:
1. `Non_Demented`
2. `Very_Mild_Demented`
3. `Mild_Demented`
4. `Moderate_Demented`

## 👁️ HiResCAM Interpretability
Below is a visual representation of the model's diagnostic focus. The generated heatmap confirms that the network accurately targets localized brain tissue atrophy rather than arbitrary image artifacts or empty space.

*(Upload your heatmap image here)*

## 🚀 How to Run Locally
1. Clone the repository: 
   ```bash
   git clone [https://github.com/codewithadityard/Alzheimers-MRI-Classification.git](https://github.com/codewithadityard/Alzheimers-MRI-Classification.git)
