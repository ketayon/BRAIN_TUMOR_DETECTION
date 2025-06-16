# 🧠 Brain Tumor Detection Models - Comparative Analysis

## 📋 Overview
This repository presents a comprehensive comparison of classical, quantum, and hybrid models for brain tumor detection from MRI scans. Each model is assessed using accuracy, precision, recall, F1-score, ROC AUC, and confusion matrices.

---

## 📁 Models Implemented

| Notebook                                          | Type                         | Description                                      |
|--------------------------------------------------|------------------------------|--------------------------------------------------|
| `classical_brain_tumor_detection.ipynb`          | Classical ML                 | Traditional ML classifiers (SVM, LR, etc.)       |
| `FidelityQuantumKernel_qiskit_brain_tumor_detection.ipynb` | Quantum Kernel     | Qiskit Fidelity Quantum Kernel                   |
| `ingenii_brain_tumor_detection.ipynb`            | Classical ML                 | Custom Classical Techniques                      |
| `pennylane_brain_tumor_detection.ipynb`          | Quantum                      | PennyLane Quantum Circuits                       |
| `piqture_brain_tumor_detection.ipynb`            | Quantum                      | Piqture Quantum ML Platform                      |
| `qiskit_hybrid_brain_tumor_detection.ipynb`      | Hybrid Quantum-Classical     | Qiskit Hybrid Pipeline                           |
| `qiskit_ml_brain_tumor_detection.ipynb`          | Quantum                      | Qiskit ML Tools                                  |
| `qml_torch_brain_tumor_detection.ipynb`          | Hybrid (Torch + Quantum)     | PyTorch + PennyLane Integration                  |
| `QuantumKernelTrainer_qiskit_brain_tumor_detection.ipynb` | Quantum Kernel Trainer | Qiskit Trainer Module                            |
| `Pegasos_qsvc_qiskit_brain_tumor_detection.ipynb`| Quantum SVM                  | Qiskit Pegasos QSVC                              |
| `Pegasos_upgrated_qsvc_qiskit_brain_tumor_detection.ipynb`| Quantum SVM         | Upgraded Pegasos QSVC                            |
| `QSNN_QLSTM_MRI_Detector.ipynb`                  | Hybrid Quantum               | **Quantum + CNN + QSNN + QLSTM Architecture** ✅ |

---

## 📊 Performance Comparison

| Model                                       | Accuracy (%) | Precision (0/1)   | Recall (0/1)     | F1-Score (0/1)   | ROC AUC | Notes                         |
|--------------------------------------------|--------------|-------------------|------------------|------------------|---------|-------------------------------|
| classical_brain_tumor_detection            | 74.51        | 0.87 / 0.69       | 0.54 / 0.93      | 0.67 / 0.79      | 0.8241  | Good classical performance    |
| FidelityQuantumKernel_qiskit               | 61.0         | 0.75 / 0.58       | 0.25 / 0.93      | 0.38 / 0.71      | -       | High recall imbalance         |
| ingenii_brain_tumor_detection              | 66.67        | 0.61 / 0.78       | 0.83 / 0.52      | 0.70 / 0.62      | -       | Moderate performance          |
| pennylane_brain_tumor_detection            | 78.43        | 0.84 / 0.75       | 0.67 / 0.89      | 0.74 / 0.81      | -       | High accuracy                 |
| piqture_brain_tumor_detection              | 50.98        | -                 | -                | -                | -       | Poor performance              |
| qiskit_hybrid_brain_tumor_detection        | 86.27        | 1.0 / 0.79        | 0.71 / 1.0       | 0.83 / 0.89      | -       | Best overall performance      |
| qiskit_ml_brain_tumor_detection            | 40.48        | -                 | -                | -                | -       | Very low performance          |
| qml_torch_brain_tumor_detection            | 72.55        | 0.71 / 0.74       | 0.71 / 0.74      | 0.71 / 0.74      | -       | Balanced hybrid model         |
| QuantumKernelTrainer_qiskit                | 60.78        | 0.83 / 0.58       | 0.21 / 0.96      | 0.33 / 0.72      | 0.6636  | Unbalanced recall             |
| Pegasos_qsvc_qiskit                        | 57.0         | 0.56 / 0.58       | 0.42 / 0.70      | 0.48 / 0.63      | -       | Low to moderate performance   |
| Pegasos_upgrated_qsvc_qiskit               | 73.0         | 0.78 / 0.70       | 0.58 / 0.85      | 0.67 / 0.77      | -       | Upgraded quantum SVM          |
| **QSNN_QLSTM_MRI_Detector **        | **83.50**    | **0.78 / 0.91**   | **0.93 / 0.74**  | **0.85 / 0.82**  | **0.9142** | **Strong hybrid quantum model** |

---

## 🧠 Key Insights

- **🏆 Best Model:** `qiskit_hybrid_brain_tumor_detection` with **86.27%** accuracy and robust F1-score.
- **📈 New Model:** `QSNN_QLSTM_MRI_Detector` shows promising hybrid performance with high ROC AUC of **0.91**.
- **⚖️ Balanced Models:** `pennylane_brain_tumor_detection` and `qml_torch_brain_tumor_detection` provide consistent balance.
- **⚠️ Caution:** Some quantum models suffer from poor recall for either class, especially `qiskit_ml_brain_tumor_detection`.

---

## 📌 Summary

| Metric               | Best Model                           | Score       |
|----------------------|--------------------------------------|-------------|
| **Accuracy**         | qiskit_hybrid_brain_tumor_detection  | 86.27%      |
| **F1-Score**         | qiskit_hybrid_brain_tumor_detection  | 0.83 / 0.89 |
| **ROC AUC**          | QSNN_QLSTM_MRI_Detector              | 0.9142      |
| **Balance**          | pennylane_brain_tumor_detection      | High        |

---

## 📚 Acknowledgements

- **Frameworks Used:** Qiskit, PennyLane, PyTorch, Scikit-Learn, OpenCV.
- **Dataset:** [Brain MRI – Brain Tumor Detection (Kaggle)](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection)

