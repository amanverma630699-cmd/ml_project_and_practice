# 🎓 Student Performance Prediction using Multiple Linear Regression

A Machine Learning project that predicts a student's **Performance Index** using **Multiple Linear Regression**. This project demonstrates the complete machine learning workflow, from data preprocessing to model evaluation.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikitlearn)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📖 Project Overview

The goal of this project is to predict a student's **Performance Index** using various academic and lifestyle factors.

The project covers:

- Data Loading
- Data Preprocessing
- Feature Encoding
- Train-Test Split
- Multiple Linear Regression
- Prediction
- Model Evaluation using R² Score

---

## 📊 Dataset

The dataset contains the following features:

| Feature | Description |
|---------|-------------|
| Hours Studied | Number of hours studied |
| Previous Scores | Previous examination scores |
| Extracurricular Activities | Whether the student participates in extracurricular activities (Yes/No) |
| Sleep Hours | Average daily sleep hours |
| Sample Question Papers Practiced | Number of sample papers solved |

### 🎯 Target Variable

- Performance Index

---

## ⚙️ Data Preprocessing

Before training the model:

- Checked for missing values
- Converted categorical values into numerical values

```python
cond = {
    "Yes": 1,
    "No": 0
}

df["Extracurricular Activities"] = df["Extracurricular Activities"].map(cond)
```

- Split the dataset into:

```
Training Data : 80%

Testing Data : 20%
```

using

```python
train_test_split(
    test_size=0.2,
    random_state=42
)
```

---

## 🤖 Machine Learning Model

This project uses

# Multiple Linear Regression

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(x_train, y_train)
```

---

## 📈 Model Evaluation

The trained model is evaluated using the **R² Score**.

```python
from sklearn.metrics import r2_score

score = r2_score(y_test, y_predict)
```

A higher R² score indicates better prediction performance.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

---

## 📂 Project Structure

```
Student-Performance-Prediction/

│── Student_Performance.csv
│── Student_Performance_Prediction.ipynb
│── README.md
```

---

## 🚀 Installation

Clone this repository

```bash
git clone https://github.com/amanverma630699-cmd/Student-Performance-Prediction.git
```

Move into the project folder

```bash
cd Student-Performance-Prediction
```

Install the required libraries

```bash
pip install numpy pandas scikit-learn
```

Run the notebook using Jupyter Notebook or VS Code.

---

## 💻 Code Workflow

```
Load Dataset
        │
        ▼
Check Missing Values
        │
        ▼
Encode Categorical Data
        │
        ▼
Split Dataset
        │
        ▼
Train Multiple Linear Regression Model
        │
        ▼
Predict Test Data
        │
        ▼
Evaluate using R² Score
```

---

## 📚 Machine Learning Concepts Used

- Supervised Learning
- Regression
- Multiple Linear Regression
- Feature Engineering
- Train-Test Split
- Model Training
- Model Prediction
- Model Evaluation

---

## 🔮 Future Improvements

- Feature Scaling
- Cross Validation
- Feature Importance Analysis
- Data Visualization
- Hyperparameter Tuning
- Deploy using Streamlit
- Compare with other Regression Models

---

## 👨‍💻 Author

### Aman Verma

🎓 B.Tech CSE (Artificial Intelligence)

🏫 Babu Banarasi Das University (BBDU)

🐍 Python Developer

🤖 Machine Learning Enthusiast

🌐 GitHub

https://github.com/amanverma630699-cmd

---

## ⭐ Support

If you found this project useful, please consider giving it a **⭐ Star** on GitHub.

It motivates me to build and share more Machine Learning projects.

---

## 📄 License

This project is open-source and available under the **MIT License**.