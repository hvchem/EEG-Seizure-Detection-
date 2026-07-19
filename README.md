# 🧠 Real-Time EEG Seizure Detection with CNN-GRU-Attention

This repository implements a deep learning framework for real-time epileptic seizure detection from scalp EEG recordings. The proposed model combines Convolutional Neural Networks (CNN), Gated Recurrent Units (GRU), and an Attention mechanism to capture both spatial and temporal characteristics of EEG signals.

Unlike many existing approaches that evaluate models on data from the same patients used during training, this project adopts a **patient-independent evaluation protocol** to assess generalization to unseen subjects. The model is trained on two publicly available EEG datasets—**CHB-MIT** and **SEINA**—to improve robustness across different recording environments and patient populations.

## ✨ Features

- CNN-GRU-Attention hybrid architecture
- Dual-dataset training (CHB-MIT + SEINA)
- Patient-independent train/validation/test splits
- Domain-robust data augmentation
- Real-time inference pipeline
- PyTorch model export (`.pth`)
- Comprehensive evaluation using standard classification metrics

## 📊 Datasets

- **CHB-MIT Scalp EEG Database**
- **SEINA EEG Dataset**

## 🏗 Model Pipeline

1. EEG preprocessing
2. Window segmentation
3. Domain-robust augmentation
4. CNN feature extraction
5. GRU temporal modeling
6. Attention mechanism
7. Binary seizure classification

## 🎯 Objective

Develop a robust seizure detection model capable of generalizing across unseen patients by leveraging multi-dataset training and patient-level evaluation, making it more suitable for real-world clinical applications.

## 🛠 Technologies

- Python
- TensorFlow / Keras
- PyTorch (model export)
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

## 📈 Evaluation

The model is evaluated using patient-independent splits, where patients in the test set are never seen during training. Performance is assessed using metrics such as:

- Accuracy
- Precision
- Recall (Sensitivity)
- F1-score
- ROC-AUC
- Confusion Matrix

## 📜 License

This project is intended for research and educational purposes.
