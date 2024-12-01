
# Brain Tumor Detection using Classical and Quantum Models

## Overview

This repository contains two notebooks that demonstrate the detection of brain tumors using MRI images. The approaches implemented include:
1. **Classical CNN-based Model**
2. **Quantum Convolutional Neural Network (QuantumCNN)**

Additionally, the repository explores a hybrid quantum-classical approach using the `ingenii-quantum-hybrid-networks` library.

---

## Results

### 1. **Classical CNN-based Model**
- **Validation Accuracy**: 94.07%
- **Test Accuracy**: 88.24%
- **Test Loss**: 0.3371

#### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| No    | 0.98      | 0.84   | 0.90     | 98      |
| Yes   | 0.91      | 0.99   | 0.94     | 155     |
| **Overall Accuracy** | **93%** |

### 2. **QuantumCNN Model**
- **Validation Accuracy**: 96.44%
- **Test Accuracy**: Not explicitly stated but inferred to be **96.44%**.

#### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| No    | 0.97      | 0.94   | 0.95     | 98      |
| Yes   | 0.96      | 0.98   | 0.97     | 155     |
| **Overall Accuracy** | **96%** |

### 3. **Hybrid Quantum-Classical Model (Ingenii)**
- **Overall Accuracy**: 89%

#### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| No    | 0.84      | 0.87   | 0.85     | 98      |
| Yes   | 0.91      | 0.90   | 0.91     | 155     |
| **Overall Accuracy** | **89%** |

---

## Files in the Repository

- `brain_tumor_detection.ipynb`: Implementation of both Classical CNN and QuantumCNN approaches.
- `ingenii_brain_tumor_detection.ipynb`: Hybrid quantum-classical approach using Ingenii's quantum libraries.

---

## Observations

1. **QuantumCNN** achieves the highest accuracy (96%), outperforming both the Classical CNN (93%) and the Hybrid Quantum-Classical approach (89%).
2. The classical model performs reasonably well, with strong performance metrics but slightly lower than the QuantumCNN.
3. The hybrid model demonstrates potential but requires further optimization to match QuantumCNN's performance.

---

## Future Work

- Improve the hybrid model's accuracy by tuning hyperparameters and exploring advanced quantum circuit designs.
- Experiment with other quantum architectures to further push performance metrics.
- Evaluate computational efficiency and resource requirements of each approach.

---

## Dependencies

- Python
- PyTorch
- Ingenii Quantum Hybrid Networks Library

---