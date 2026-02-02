# 🧠 SVM – Breast Cancer Classification Model

## 📌 Problem Statement
The objective of this project is to build a machine learning classification model that can accurately predict whether a breast tumor is malignant or benign based on clinical features extracted from breast mass images.

Early and accurate classification is crucial for effective diagnosis and treatment planning.

---

## 📊 Dataset Overview
- The dataset contains numeric features computed from digitized images of fine needle aspirates (FNA) of breast masses.
- Each record is labeled as:
  - Malignant (1)
  - Benign (0)
- The features represent characteristics such as radius, texture, smoothness, concavity, symmetry, and related statistical measurements.

---

## ⚙️ Model Used
A Support Vector Machine (SVM) classifier is used due to its strong performance in high-dimensional feature spaces and effectiveness in binary classification problems.

The following kernels are evaluated:
- Linear Kernel – used as a baseline model
- RBF (Radial Basis Function) Kernel – used to model non-linear decision boundaries

---

## 🔧 Feature Scaling
- StandardScaler is applied to normalize feature values.
- Feature scaling ensures that all input variables contribute equally to distance-based calculations in SVM.

---

## 🧪 Model Training Strategy
1. The dataset is split into training (80%) and testing (20%) sets using stratified sampling.
2. A machine learning pipeline is created combining:
   - Feature scaling
   - SVM classifier
3. A baseline model is trained using a linear kernel.
4. A more complex model is trained using an RBF kernel to improve performance.

---

## 🔍 Hyperparameter Tuning
GridSearchCV is used to optimize key SVM hyperparameters:
- C (regularization parameter)
- gamma (kernel coefficient)

Cross-validation ensures that the selected model generalizes well and avoids overfitting.

---

## 📈 Model Evaluation
The final tuned model is evaluated using:
- Accuracy Score
- Confusion Matrix
- Precision, Recall, and F1-Score
- ROC Curve
- AUC (Area Under the Curve)

These metrics provide a comprehensive assessment of classification performance.

---

## 📊 ROC Curve Analysis
- The ROC curve visualizes the trade-off between the True Positive Rate and False Positive Rate.
- A higher AUC value indicates stronger discriminatory capability between malignant and benign cases.

---

## 💾 Model Persistence
- The optimized model is saved as a single pipeline containing:
  - StandardScaler
  - Tuned SVM classifier
- This allows seamless reuse of the model for future predictions without retraining.

---

## ✅ Final Outcome
- The model achieves high classification accuracy with strong generalization performance.
- Demonstrates effective use of kernel-based learning and hyperparameter optimization.
- Suitable for real-world binary classification tasks in healthcare analytics.

---

## 👨‍💻 Author
Utkarsh Kohli
