# E-Shopping Data Analysis and Machine Learning

## 📌 Project Overview

This project focuses on analyzing e-shopping data and applying machine learning classification algorithms to predict outcomes based on shopping-related features. It uses Python libraries for data analysis, visualization, preprocessing, feature selection, and model evaluation.

The project compares three machine learning algorithms: Logistic Regression, Decision Tree Classifier, and Random Forest Classifier to evaluate their performance using different classification metrics.

## 🎯 Objectives

* Analyze and understand the e-shopping dataset.
* Identify missing values and duplicate records.
* Explore relationships between numerical features using correlation analysis.
* Visualize data using boxplots and heatmaps.
* Prepare the dataset for machine learning.
* Handle class imbalance using SMOTE.
* Select important features using SelectKBest.
* Apply data transformation and standardization.
* Train and compare different classification models.
* Evaluate model performance using classification metrics.

## 🛠️ Technologies Used

* **Python** – Programming language
* **NumPy** – Numerical operations
* **Pandas** – Data manipulation and analysis
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical data visualization
* **Scikit-learn** – Machine learning algorithms and evaluation
* **Imbalanced-learn** – Handling imbalanced data using SMOTE
* **Jupyter Notebook** – Development environment

## 📂 Dataset

The project uses a dataset named `e-shopping.csv`.

The notebook examines shopping-related features, including:

* Price
* Order
* Page information
* Session ID
* Year
* Other available dataset attributes

The column `price 2` is renamed to `target` for use as the target variable in the classification workflow.

**Note:** The exact meaning of the target variable should be confirmed from the dataset's documentation.

## ⚙️ Project Workflow

### 1. Data Loading and Exploration

* Load the dataset using Pandas.
* Display the first and last records.
* Check the dataset's shape and column names.
* Examine data types and descriptive statistics.

### 2. Data Cleaning

* Check for missing values.
* Identify duplicate records.
* Remove rows containing missing values before model preparation.

### 3. Exploratory Data Analysis

* Calculate correlations between numerical features.
* Visualize correlations using heatmaps.
* Identify potential outliers using boxplots.

### 4. Data Preprocessing

* Separate the target variable from the input features.
* Split the data into training and testing sets.
* Use an 80:20 training-testing split.
* Apply SMOTE to address class imbalance in the training data.

### 5. Feature Selection

Use **SelectKBest** with the ANOVA F-test (`f_classif`) to select eight features for the preprocessing workflow.

### 6. Data Transformation and Scaling

* Apply the Yeo-Johnson Power Transformation to reduce skewness.
* Use StandardScaler to standardize the selected features.

### 7. Model Training

The project implements three classification algorithms:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

### 8. Model Evaluation

The models are evaluated using the following metrics:

* **Accuracy:** Measures the proportion of correct predictions.
* **Precision:** Measures how many predicted positive or class assignments are correct, depending on the averaging method.
* **Recall:** Measures how many actual class instances are correctly identified.
* **F1 Score:** Combines precision and recall into a single metric.

A comparison table is created to compare the performance of all three models.

## 📊 Machine Learning Models

| Model                    | Purpose                                            |
| ------------------------ | -------------------------------------------------- |
| Logistic Regression      | Classification using a logistic model              |
| Decision Tree Classifier | Classification using decision rules                |
| Random Forest Classifier | Classification using an ensemble of decision trees |

## 🚀 How to Run the Project

### Prerequisites

Install Python and Jupyter Notebook.

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Navigate to the Project Folder

```bash
cd YOUR_PROJECT_FOLDER
```

### Step 3: Install the Required Libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn jupyter
```

### Step 4: Add the Dataset

Place `e-shopping.csv` in the same folder as the Jupyter Notebook.

### Step 5: Open Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells in order.

## 📈 Results

The notebook generates performance metrics for Logistic Regression, Decision Tree, and Random Forest.

The results are organized into a comparison table containing:

* Accuracy
* Precision
* Recall
* F1 Score

The model with the best performance can be identified by comparing these metrics after executing the notebook.

*Note: Actual model scores are not included here because they need to be obtained from the notebook's execution results.*

## 🔮 Future Enhancements

* Improve model performance through hyperparameter tuning.
* Compare additional classification algorithms.
* Create more visualizations to understand shopping patterns.
* Add confusion matrices and classification reports.
* Develop an interactive dashboard to present model results.

## 👩‍💻 Author

**Mizba Tabasum**

BCA Student | Aspiring Data Science and Machine Learning Enthusiast

## 📄 License

This project is intended for educational and learning purposes.
