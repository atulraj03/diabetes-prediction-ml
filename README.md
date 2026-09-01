# Diabetes Prediction — Supervised Learning Capstone

Predicting whether a patient has diabetes (1) or not (0) using medical diagnostic data of female patients (Pima Indians Diabetes Dataset).

## 📊 Dataset
- **File:** `diabetes.csv`
- **Features:** Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age
- **Target:** `Outcome` (1 = diabetic, 0 = non-diabetic)

## 🔧 Workflow
1. Loaded data with Pandas, checked shape and basic statistics
2. Checked for missing values
3. Visualized the distribution of `Glucose` with a histogram
4. Split data into features (`X`) and target (`y`)
5. 80-20 train-test split
6. Trained a **Logistic Regression** model
7. Trained a **Decision Tree Classifier**
8. Evaluated both models with accuracy, confusion matrix, and classification report
9. Compared feature importances from the Decision Tree

## 📈 Results

| Model               | Accuracy |
|----------------------|----------|
| Logistic Regression  | 74.7%    |
| Decision Tree         | 74.7%    |

**Classification Report (Logistic Regression):**

| Class | Precision | Recall | F1-score |
|-------|-----------|--------|----------|
| 0 (No Diabetes) | 0.81 | 0.79 | 0.80 |
| 1 (Diabetes)     | 0.64 | 0.67 | 0.65 |

**Top predictive features (Decision Tree feature importance):**
1. Glucose
2. BMI
3. Blood Pressure
4. Age
5. Diabetes Pedigree Function

Glucose level was by far the strongest predictor of diabetes — consistent with clinical understanding.

## 🛠️ Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib
- Scikit-learn (Logistic Regression, Decision Tree, train_test_split, metrics)

## 🚀 How to Run
```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook 01-Atul-ML-CapstoneProject.ipynb
```

## 👤 Author
**Atul Raj**
- GitHub: [atulraj03](https://github.com/atulraj03)
- LinkedIn: [atulraj07](https://linkedin.com/in/atulraj07)
