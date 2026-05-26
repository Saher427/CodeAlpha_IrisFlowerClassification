#  Iris Flower Classification
### CodeAlpha Data Science Internship — Task 1

##  Project Overview

This project builds a machine learning classification model to identify the species of an Iris flower based on its physical measurements. The dataset contains **150 samples** across 3 species — **Setosa**, **Versicolor**, and **Virginica** — with 4 features each: sepal length, sepal width, petal length, and petal width.

##  Dataset

- **Source:** [Kaggle — Iris CSV by saurabh00007](https://www.kaggle.com/datasets/saurabh00007/iriscsv)
- **File:** `Iris.csv`
- **Rows:** 150 (50 samples per species)
- **Features:** `SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, `PetalWidthCm`, `Species`
- **Missing Values:** None

##  Tech Stack

| Tool | Purpose |
**Python 3:** Core language 
**Pandas:** Data loading and manipulation 
**NumPy:** Numerical operations
**Matplotlib:** Plotting 
**Seaborn:** Statistical visualizations 
**Scikit-learn:** Model training and evaluation 

##  Project Workflow

1. **Data Loading:** Loaded `Iris.csv`, dropped the `Id` column (no predictive value)
2. **EDA:** Pairplot to visualize species separation, correlation heatmap
3. **Preprocessing:** Label encoded the target species column, stratified 80/20 train-test split
   - Training samples: **120**
   - Testing samples: **30**
4. **Model Training:** Trained 3 classification models and compared accuracy
5. **Evaluation:** Classification report + Confusion Matrix for the best model

##  Models Used & Results

| Model | Accuracy |
|---|---|
| **KNN (k=5)** | **100.00%** |
| Decision Tree | 93.33% |
| Random Forest | 90.00% |

> KNN achieved the highest accuracy on this dataset. Random Forest was used for the final confusion matrix and classification report.

##  Classification Report (Random Forest)

| Class | Precision | Recall | F1-Score | Support |
|---|---|---|---|---|
| Iris-setosa | 1.00 | 1.00 | 1.00 | 10 |
| Iris-versicolor | 0.82 | 0.90 | 0.86 | 10 |
| Iris-virginica | 0.89 | 0.80 | 0.84 | 10 |
| **Overall Accuracy** | | | **0.90** | **30** |

##  Visualizations

- Pairplot showing feature relationships across the 3 species
- Feature correlation heatmap
- Model accuracy comparison bar chart (KNN vs Decision Tree vs Random Forest)
- Confusion matrix for Random Forest classifier

##  Repository Structure

CodeAlpha_IrisFlowerClassification/
├── Iris_Classification.ipynb   # Main notebook with all code and outputs
├── Iris.csv                    # Dataset
└── README.md                   # Project documentation

## How to Run

1. Clone this repository
   
   git clone https://github.com/Saher427/CodeAlpha_IrisFlowerClassification.git
   cd CodeAlpha_IrisFlowerClassification
   
2. Install dependencies
   
   pip install pandas numpy matplotlib seaborn scikit-learn
   
3. Open the notebook
   
   jupyter notebook Iris_Classification.ipynb
  
   Or open directly in [Google Colab](https://colab.research.google.com/)

##  Internship

This project was completed as part of the **CodeAlpha Data Science Internship**.

- 🌐 Website: [www.codealpha.tech](https://www.codealpha.tech)
- 📧 Email: services@codealpha.tech