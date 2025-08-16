# 🧠 SVM Classification on Breast Cancer Dataset

This project demonstrates the use of **Support Vector Machines (SVMs)** with both **Linear** and **RBF kernels**.  
It also visualizes decision boundaries on a toy dataset and performs **hyperparameter tuning** using `GridSearchCV`.

---

## 📂 Dataset
- **Breast Cancer Dataset** from `sklearn.datasets`
- Features: 30 numeric features from digitized images of breast masses
- Target:  
  - `0` = Malignant  
  - `1` = Benign  

---

## ⚙️ Steps
1. **Load Dataset** – Breast Cancer dataset from scikit-learn  
2. **Preprocess** – Standardized features with `StandardScaler`  
3. **Train Models** –  
   - Linear SVM (`kernel="linear"`)  
   - RBF SVM (`kernel="rbf"`)  
4. **Toy Dataset Visualization** – Used `make_moons` to visualize linear vs. non-linear decision boundaries  
5. **Hyperparameter Tuning** – `GridSearchCV` over C and gamma  
6. **Cross-validation** – Compared model performance using `cross_val_score`  
7. **Evaluation** – Accuracy, Classification Report  

---

## 📊 Results
- **Linear SVM Accuracy (Test)**: ~95.6%  
- **RBF SVM Accuracy (Test)**: ~96.5%  
- **Best Parameters (GridSearchCV)**: `C=10, gamma=0.01, kernel=rbf`  
- **Best Cross-validation Score**: ~97.1%  
- **Classification Report (RBF)**:  
markdown
Copy
Edit
           precision    recall  f1-score   support
Malignant 0.95 0.95 0.95 43
Benign 0.97 0.97 0.97 71
Accuracy 0.96
