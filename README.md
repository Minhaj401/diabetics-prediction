# 🩺 Diabetes Prediction System using SVM

This project uses a Support Vector Machine (SVM) classification model to predict whether a person is diabetic or not based on various medical attributes. It involves data preprocessing, model training, evaluation, and deployment of a simple predictive system.

---

## 📁 Dataset

The dataset used is the **PIMA Indian Diabetes Dataset**, which contains information about female patients. It includes 768 records with 8 medical features and an outcome column:
- **Pregnancies**
- **Glucose**
- **Blood Pressure**
- **Skin Thickness**
- **Insulin**
- **BMI**
- **Diabetes Pedigree Function**
- **Age**
- **Outcome** (0 → Non-Diabetic, 1 → Diabetic)

---

## 🛠️ Libraries Used

- `numpy`
- `pandas`
- `sklearn` (StandardScaler, train_test_split, svm, accuracy_score)

---

## 🔍 Workflow

### 1. Importing Dependencies
All necessary libraries for data processing, model building, and evaluation are imported.

### 2. Data Collection and Exploration
- Load dataset using `pandas.read_csv()`
- Display the first few rows and get statistical summaries using `describe()` and `mean()`
- Analyze class distribution using `value_counts()` and grouped mean using `groupby()`

### 3. Data Preprocessing
- Separate features (`X`) and label (`y`)
- Standardize feature values using `StandardScaler`

### 4. Model Training
- Split the data using `train_test_split` with stratification
- Train an SVM classifier with a linear kernel using the training data

### 5. Model Evaluation
- Evaluate model performance on both training and test sets using `accuracy_score`

### 6. Prediction System
- Make predictions using new input data
- Data is preprocessed and passed to the trained model to determine if the person is diabetic

---

## 🔮 Sample Input

```python
input_data = (8, 183, 64, 0, 0, 23.3, 0.672, 32)
```

**Output**:  
> The person is diabetic

---

## 🧠 Model Used

SVM Classifier with a linear kernel.

Chosen for its robustness in binary classification problems with clear margins of separation.

---

## ✅ Accuracy

- **Training Accuracy**: ~79%
- **Testing Accuracy**: ~77% (depending on dataset split)

---

## 📌 How to Run

1. Clone the repository or copy the code into a Jupyter Notebook or Python script.
2. Ensure you have all the required dependencies installed.
3. Download the dataset (`diabetes.csv`) and place it in the appropriate directory.
4. Run the notebook or script.
