# 🎬 MovieLens Case Study — Movie Rating Prediction & Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-green?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

This project performs an end-to-end **Exploratory Data Analysis (EDA)** and **Machine Learning** study on the **MovieLens dataset** — one of the most widely used datasets in the field of recommendation systems and movie analytics.

The goal is to understand user behaviour, explore movie rating patterns, engineer meaningful features, and develop classification models to **predict movie ratings** based on user demographics and movie attributes.

---

## 🗂️ Dataset Description

The MovieLens dataset consists of three interconnected files:

| File | Description |
|------|-------------|
| `movies.dat` | Movie ID, Title, and Genre |
| `ratings.dat` | User ID, Movie ID, Rating (1–5), Timestamp |
| `users.dat` | User ID, Gender, Age, Occupation, Zip Code |

> **Source:** [GroupLens Research — MovieLens Dataset](https://grouplens.org/datasets/movielens/)

---

## 🎯 Objectives

- Import and merge all three datasets into a unified **Master Dataset**
- Perform **Exploratory Data Analysis** through visualisations
- Analyse user demographics and their influence on movie ratings
- Apply **Feature Engineering** (genre one-hot encoding, movie age, gender encoding)
- Train and compare **9 Machine Learning classifiers** to predict ratings

---

## 🔍 Analysis Highlights

### 📊 Exploratory Data Analysis
- **User Age Distribution** — Bar chart analysis of different age groups
- **Toy Story Ratings** — Rating distribution breakdown for a specific movie
- **Top 25 Movies by Viewership** — Horizontal bar chart of most-viewed titles
- **User-specific Ratings** — Detailed view of all movies rated by a specific user

### ⚙️ Feature Engineering
- Extracted all **18 unique genres** and applied **one-hot encoding**
- Parsed **release year** from movie titles and computed **Movie Age**
- Encoded **Gender** as binary (Female = 1, Male = 0)
- Analysed how Gender, Age, Occupation, and Movie Year affect ratings

---

## 🤖 Machine Learning Models

Nine classification algorithms were trained and compared on features `[MovieID, Age, Occupation]`:

| Model | Algorithm |
|-------|-----------|
| Logistic Regression | Linear classifier |
| Support Vector Machine (SVC) | Kernel-based classifier |
| Linear SVC | Linear SVM |
| K-Nearest Neighbours | Distance-based classifier |
| Gaussian Naive Bayes | Probabilistic classifier |
| Perceptron | Neural-inspired linear classifier |
| Stochastic Gradient Descent | Online linear classifier |
| Decision Tree | Tree-based classifier |
| Random Forest | Ensemble tree classifier |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.8+ | Core programming language |
| Pandas | Data loading, merging, manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Scikit-learn | Machine learning models |

---

## 📁 Project Structure

```
movielens-case-study/
│
├── movielens-case-study.ipynb   # Main Jupyter Notebook (EDA + ML)
└── README.md                    # Project documentation
```

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/homeshwarnelakurthi/movielens-case-study.git
cd movielens-case-study
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib scikit-learn
```

### 3. Download the dataset
Download the MovieLens 1M dataset from [GroupLens](https://grouplens.org/datasets/movielens/1m/) and place the following files in the project directory:
- `movies.dat`
- `ratings.dat`
- `users.dat`

### 4. Run the Notebook
```bash
jupyter notebook movielens-case-study.ipynb
```

---

## 📈 Key Insights

- Age group **25–34** has the highest number of active raters
- **Toy Story** received predominantly high ratings (4–5 stars)
- Movie **genre** is a significant feature in rating behaviour
- **Random Forest** achieved the highest training accuracy among all classifiers
- User **demographics** (Age, Occupation, Gender) measurably influence rating patterns

---

## 👨‍💻 Author

**Homeswar Rao Nelakurthi**  
[![GitHub](https://img.shields.io/badge/GitHub-homeshwarnelakurthi-181717?style=flat&logo=github)](https://github.com/homeshwarnelakurthi)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
