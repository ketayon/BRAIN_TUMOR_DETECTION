
# Brain Tumor Detection using Classical and Quantum Models

## Overview

This repository contains two notebooks that demonstrate the detection of brain tumors using MRI images. The approaches implemented include:
1. **Classical CNN-based Model**
2. **Quantum Convolutional Neural Network (QuantumCNN)**

Additionally, the repository explores a hybrid quantum-classical approach using the `ingenii-quantum-hybrid-networks` library.

---

# Brain Tumor Detection using Classical and Quantum Models

## Results

### 1. **Classical CNN-based Model**
- **Accuracy**: 80%
- **Classification Report**:
  - **Class 0 (No Tumor)**: Precision = 0.76, Recall = 0.84, F1-Score = 0.80
  - **Class 1 (Tumor)**: Precision = 0.84, Recall = 0.76, F1-Score = 0.80
  - **Overall Accuracy**: 80%
- **Confusion Matrix**:
  [[16, 3],
   [5, 16]]
- **ROC AUC Score**: 0.862

### 2. **Hybrid Quantum-Classical Model (Ingenii)**
- **Accuracy**: 80%
- **Classification Report**:
  - **Class 0 (No Tumor)**: Precision = 0.76, Recall = 0.84, F1-Score = 0.80
  - **Class 1 (Tumor)**: Precision = 0.84, Recall = 0.76, F1-Score = 0.80
  - **Overall Accuracy**: 80%
- **Confusion Matrix**:
  [[16, 3],
   [5, 16]]
- **ROC AUC Score**: 0.802

### 3. **QuantumCNN Model (qml_torch)**
- **Accuracy**: 90%
- **Classification Report**:
  - **Class 0 (No Tumor)**: Precision = 1.00, Recall = 0.79, F1-Score = 0.88
  - **Class 1 (Tumor)**: Precision = 0.84, Recall = 1.00, F1-Score = 0.91
  - **Overall Accuracy**: 90%
- **Confusion Matrix**:
  [[15, 4],
   [0, 21]]
- **ROC AUC Score**: 0.895

### 4. **Quantum Kernel Trainer Model (qiskit)**
- **Accuracy**: 60.78%
- **Classification Report**:
  - **Class 0 (No Tumor)**: Precision = 0.83, Recall = 0.21, F1-Score = 0.33
  - **Class 1 (Tumor)**: Precision = 0.58, Recall = 0.96, F1-Score = 0.72
  - **Overall Accuracy**: 60.78%
- **Confusion Matrix**:
  [[5, 19],
   [1, 26]]
- **ROC AUC Score**: 0.664

## Conclusions

- **QuantumCNN** outperforms all other models with an accuracy of **90%**, showing strong potential in detecting brain tumors.
- The **Classical CNN-based Model** and the **Hybrid Quantum-Classical Model (Ingenii)** achieve a solid accuracy of **80%** each. Despite showing potential, these models need further optimization.
- The **Quantum Kernel Trainer Model** shows relatively poor performance with an accuracy of **60.78%**. The performance indicates that quantum models based on kernel methods may require further refinement and optimization.
- The **ROC AUC Score** is highest for the **QuantumCNN** model (0.895), indicating better overall performance in distinguishing between tumor and non-tumor classes.

## Future Directions
- Further optimization of quantum models (especially kernel-based approaches) is necessary to improve performance.
- Experimenting with more advanced hybrid architectures combining quantum and classical computing could lead to even better results.
- More hyperparameter tuning and training data augmentation could help improve the performance of the classical models.

---

## Dependencies

- Python
- PyTorch
- Ingenii Quantum Hybrid Networks Library

---