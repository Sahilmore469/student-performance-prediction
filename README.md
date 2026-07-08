<div align="center">

# 📊 Student Performance Analysis & Prediction

**Uncovering what drives exam performance — and predicting it — using EDA and Linear Regression.**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

</div>

---

## 🔍 Overview

This project analyzes a real-world dataset of **6,600+ students** to understand the factors that shape academic performance, and builds regression models to **predict final exam scores**. It combines exploratory data analysis with model comparison — going beyond study hours and attendance to test whether contextual factors like parental involvement, motivation, and peer influence add real predictive power.

**Key questions explored:**
- How do study hours and attendance relate to exam performance?
- Is there a meaningful gender-based performance gap?
- Do parental involvement, motivation, and peer influence matter — and by how much?
- How well can a simple linear model predict a student's final score?

---

## 🗂️ Dataset

| | |
|---|---|
| **File** | `StudentPerformanceFactors.csv` |
| **Rows** | 6,607 students |
| **Features** | 19 (numeric + categorical) |
| **Target** | `Exam_Score` |

**Feature categories:**
- **Study habits:** `Hours_Studied`, `Attendance`, `Tutoring_Sessions`, `Previous_Scores`
- **Lifestyle:** `Sleep_Hours`, `Physical_Activity`, `Extracurricular_Activities`
- **Home & school context:** `Parental_Involvement`, `Family_Income`, `Access_to_Resources`, `Parental_Education_Level`, `School_Type`, `Teacher_Quality`, `Distance_from_Home`
- **Personal factors:** `Motivation_Level`, `Peer_Influence`, `Internet_Access`, `Learning_Disabilities`, `Gender`

---

## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn` · `Jupyter Notebook`

---

## 📈 Workflow

1. **Data Cleaning** — handled missing values in categorical columns and removed an invalid outlier score
2. **Exploratory Data Analysis** — score distributions, attendance impact, gender-wise comparison, and contextual-factor breakdowns
3. **Correlation Analysis** — heatmap of numeric feature relationships
4. **Modeling** — two Linear Regression models built and compared:
   - **Core model** — `Hours_Studied`, `Attendance`, `Previous_Scores`
   - **Extended model** — all 19 features, one-hot encoded
5. **Evaluation** — R², MAE, RMSE, predicted-vs-actual plots, and residual analysis

---

## 📊 Results

| Model | Features | R² Score | MAE | RMSE |
|---|---|---|---|---|
| Core | 3 (study hours, attendance, previous scores) | **0.655** | 1.33 | 2.13 |
| Extended | 19 (all available features) | **0.825** | 0.42 | 1.52 |

**Takeaway:** Study habits alone explain a moderate share of exam performance. Adding contextual factors — parental involvement, motivation, and peer influence in particular — meaningfully improves prediction, confirming that academic outcomes are shaped by more than just hours studied.

---

## 📂 Repository Structure

```
├── Student_Performance_Analysis.ipynb   # Full analysis notebook (EDA + modeling)
├── StudentPerformanceFactors.csv        # Dataset
└── README.md                            # Project overview
```

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/<your-username>/student-performance-analysis.git
cd student-performance-analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch the notebook
jupyter notebook Student_Performance_Analysis.ipynb
```

---

## 🔮 Future Improvements

- Try non-linear models (Random Forest, XGBoost) to capture relationships a linear model misses
- Rank feature importance across contextual factors
- Build an interactive "what-if" dashboard for individual student predictions

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

<div align="center">

**⭐ If you found this project useful, consider giving it a star!**

</div>
