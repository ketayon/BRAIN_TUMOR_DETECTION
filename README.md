# Brain Tumor Detection Models - Comparative Analysis

## Overview
This repository contains various machine learning and quantum-based approaches for brain tumor detection. The goal is to compare the performance of these models based on accuracy, precision, recall, F1-score, ROC AUC, and confusion matrices.

The models include classical machine learning techniques, hybrid quantum-classical methods, and fully quantum machine learning algorithms.

---

## Models Implemented

1. **classical_brain_tumor_detection.ipynb**  
   **Type:** Classical Machine Learning  
   **Tools:** Traditional classifiers (e.g., SVM, Logistic Regression, etc.)

2. **FidelityQuantumKernel_qiskit_brain_tumor_detection.ipynb**  
   **Type:** Quantum Kernel-Based Machine Learning  
   **Tools:** Qiskit Fidelity Quantum Kernel

3. **ingenii_brain_tumor_detection.ipynb**  
   **Type:** Classical Machine Learning  
   **Tools:** Custom Classical Techniques

4. **pennylane_brain_tumor_detection.ipynb**  
   **Type:** Quantum Machine Learning  
   **Tools:** PennyLane Framework

5. **piqture_brain_tumor_detection.ipynb**  
   **Type:** Quantum/Hybrid Quantum  
   **Tools:** Piqture Quantum Techniques

6. **qiskit_hybrid_brain_tumor_detection.ipynb**  
   **Type:** Hybrid Quantum-Classical Model  
   **Tools:** Qiskit Hybrid ML Framework

7. **qiskit_ml_brain_tumor_detection.ipynb**  
   **Type:** Quantum Machine Learning  
   **Tools:** Qiskit ML Libraries

8. **qml_torch_brain_tumor_detection.ipynb**  
   **Type:** Quantum Torch-Based Model  
   **Tools:** PyTorch and Quantum ML Integration

9. **quantum_torch_brain_tumor_detection.ipynb**  
   **Type:** Hybrid Quantum Torch ML  
   **Tools:** PyTorch + Quantum Methods

10. **QuantumKernelTrainer_qiskit_brain_tumor_detection.ipynb**  
    **Type:** Quantum Kernel Training  
    **Tools:** Qiskit Quantum Kernel Trainer

11. **Pegasos_qsvc_qiskit_brain_tumor_detection.ipynb**  
    **Type:** Quantum Kernel-Based Machine Learning  
    **Tools:** Qiskit Fidelity Quantum Kernel

---

## Performance Comparison

Below is a summary of all models with their respective performance metrics:

| Model                                         | Accuracy (%) | Precision (0/1) | Recall (0/1) | F1-Score (0/1) | ROC AUC Score | Notes                         |
|---------------------------------------------|-------------|----------------|--------------|----------------|---------------|--------------------------------|
| **classical_brain_tumor_detection**          | 80.0        | 0.76 / 0.84    | 0.84 / 0.76  | 0.80 / 0.80    | 0.8621        | Balanced, strong performance  |
| **FidelityQuantumKernel_qiskit**             | 62.74       | 1.0 / 0.58     | 0.21 / 1.0   | 0.34 / 0.73    | 0.6944        | High recall imbalance         |
| **ingenii_brain_tumor_detection**            | 80.0        | 0.76 / 0.84    | 0.84 / 0.76  | 0.80 / 0.80    | 0.8020        | Similar to classical          |
| **pennylane_brain_tumor_detection**          | 77.5        | 0.81 / 0.75    | 0.68 / 0.86  | 0.74 / 0.80    | 0.7707        | Balanced performance          |
| **piqture_brain_tumor_detection**            | 44.62       | -              | -            | -              | -             | Low accuracy                  |
| **qiskit_hybrid_brain_tumor_detection**      | 85.0        | 0.93 / 0.80    | 0.73 / 0.95  | 0.82 / 0.87    | 0.8446        | Best performance overall      |
| **qiskit_ml_brain_tumor_detection**          | 38.06       | -              | -            | -              | -             | Low accuracy                  |
| **qml_torch_brain_tumor_detection**          | 75.0        | 0.68 / 0.87    | 0.89 / 0.62  | 0.77 / 0.72    | 0.7568        | Good for class 0              |
| **quantum_torch_brain_tumor_detection**      | 80.39       | 0.93 / 0.74    | 0.63 / 0.96  | 0.75 / 0.83    | N/A           | High precision for class 0    |
| **QuantumKernelTrainer_qiskit**              | 60.78       | 0.83 / 0.58    | 0.21 / 0.96  | 0.33 / 0.72    | 0.6635        | Imbalanced recall             |
| **Pegasos_qsvc_qiskit_brain_tumor_detection**| 52.94       | 0.50 / 0.56    | 0.50 / 0.56  | 0.50 / 0.56    | 0.3812        | Moderate performance          |

---

## Key Observations

1. **Best Performing Model**:
   - `qiskit_hybrid_brain_tumor_detection` achieved the highest accuracy of **85%** with balanced precision, recall, and F1-scores.

2. **Classical Approaches**:
   - `classical_brain_tumor_detection` and `ingenii_brain_tumor_detection` performed consistently well with **80% accuracy**.

3. **Quantum and Hybrid Approaches**:
   - Hybrid models like `qiskit_hybrid_brain_tumor_detection` and `quantum_torch_brain_tumor_detection` showed competitive performance.
   - Pure quantum models (e.g., `QuantumKernelTrainer_qiskit` and `FidelityQuantumKernel_qiskit`) had lower accuracies, indicating challenges in generalization.

4. **Low Performing Models**:
   - `piqture_brain_tumor_detection` and `qiskit_ml_brain_tumor_detection` had accuracies below **50%**, indicating limitations in these implementations.

5. **Imbalance Challenges**:
   - Several quantum models showed high recall for class `1` but poor recall for class `0`. Balancing techniques may improve these results.

---

## Conclusion

- **Hybrid quantum-classical models** outperform pure quantum models in brain tumor detection tasks.
- Classical models remain strong contenders, with robust and reliable results.
- Further improvements in quantum models could focus on balancing class performance and tuning hyperparameters.

---

## Results Summary

| Metric                    | Best Model                           | Score     |
|---------------------------|-------------------------------------|-----------|
| **Accuracy**              | qiskit_hybrid_brain_tumor_detection | 85.0%     |
| **F1-Score**              | qiskit_hybrid_brain_tumor_detection | 0.87 / 0.82 |
| **ROC AUC Score**         | classical_brain_tumor_detection     | 0.8621    |
| **Balanced Performance**  | classical_brain_tumor_detection     | High      |

---

## Acknowledgements
- **Frameworks Used**: Qiskit, PennyLane, PyTorch, Scikit-Learn
