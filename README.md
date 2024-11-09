# GlucoSense- AI-Powered Diabetes Detection for Early Intervention

## Project Overview

**Project_Diabetes** aims to develop a machine-learning model to predict diabetes status based on healthcare data. The primary objective is to understand the relationship between lifestyle factors and diabetes risk. This project will utilize various machine-learning techniques for data analysis, feature selection, model development, and evaluation.

### Key Features:
- **Data Preprocessing**: Handling missing values, data discrepancies, and outlier management.
- **Feature Engineering**: Identifying key features and relationships within the data to enhance model performance.
- **Machine Learning Models**: Implementing and evaluating various algorithms, including classification models, to predict diabetes risk.
- **Evaluation Metrics**: Precision, recall, F1 score, AUC, and classification accuracy.

## Table of Contents

1. [Getting Started](#getting-started)
2. [Installation Instructions](#installation-instructions)
3. [Usage](#usage)
4. [Project Structure](#project-structure)
5. [Data Description](#data-description)
6. [Model Building](#model-building)
7. [Evaluation Metrics](#evaluation-metrics)
8. [License](#license)
9. [Acknowledgements](#acknowledgements)

## Getting Started

To get started with the project, you’ll need to set up the necessary environment and dependencies. The following instructions will help you run the code on your local machine.

### Prerequisites
- Python 3.5
- Required Python libraries (listed below)

### Installation Instructions

1. **Clone the repository:**

   ```bash
   git clone https://github.com/rahulthota21/RahulThota-GlucoSense-Infy-Nov24.git

2. **Navigate to the project directory:**
   ```bash
   cd RahulThota-GlucoSense-Infy-Nov24
3. **Install dependencies:**
   It’s recommended to create a virtual environment before installing the dependencies.
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'
   pip install -r requirements.txt

3. **Run the code:**
   Once the environment is set up, you can start by running the main.py file or exploring individual scripts for data preprocessing, feature selection, and model building.
   ```bash
   python main.py


## Usage

After setting up the environment and installing dependencies, you can use this project to predict diabetes status. The repository includes scripts for:

- **Data Preprocessing**: `preprocessing.py`
- **Feature Selection**: `feature_selection.py`
- **Model Building and Training**: `model_building.py`
- **Model Evaluation**: `model_evaluation.py`

You can execute each of these scripts to follow through the project steps or modify them as needed for your own research or applications.

## Project Structure

  ```bash
  Project_Diabetes/
├── data/
│   └── diabetes_dataset.csv       # Raw and cleaned data
├── notebooks/
│   └── exploratory_analysis.ipynb # Jupyter notebook for data exploration and analysis
├── src/
│   ├── preprocessing.py           # Data preprocessing script
│   ├── feature_selection.py       # Feature selection script
│   ├── model_building.py          # Model building and training script
│   └── model_evaluation.py        # Model evaluation script
├── main.py                        # Main script to run the entire pipeline
├── requirements.txt               # List of dependencies
└── README.md                      # Project documentation
```

## Data Description

The dataset used in this project includes healthcare statistics of individuals, with features like age, gender, BMI, glucose level, blood pressure, and insulin levels. The goal is to predict whether an individual has diabetes based on these features.

Key columns in the dataset:
- `Pregnancies`: Number of pregnancies the patient has had
- `Glucose`: Plasma glucose concentration
- `BloodPressure`: Diastolic blood pressure (mm Hg)
- `SkinThickness`: Skinfold thickness (mm)
- `Insulin`: 2-hour serum insulin (mu U/ml)
- `BMI`: Body mass index (kg/m²)
- `Age`: Age of the individual
- `Outcome`: Target variable (1 indicates diabetes, 0 indicates no diabetes)

## Model Building

### Algorithms Used:

- **Logistic Regression**: For binary classification based on a linear combination of features.
- **Random Forest Classifier**: A robust ensemble model for classification.
- **SVM (Support Vector Machine)**: For high-dimensional classification.
- **K-Nearest Neighbors (KNN)**: A non-parametric method for classification.
- **XGBoost**: A gradient-boosting model known for high performance.

### Feature Selection:

We perform feature selection to identify the most important variables and eliminate noise. This process includes:
- **Correlation matrix analysis**: Analyzing relationships among features to identify collinear variables.
- **Feature importance from models**: Using model-specific techniques to rank features by importance.
- **Recursive Feature Elimination (RFE)**: Iteratively removing less important features to find the optimal set of predictors.

### Feature Selection

Feature selection is crucial for enhancing model performance and reducing computational complexity. In this project, we use the following methods to select the most informative features:

- **Correlation Matrix Analysis**: Identifying relationships between features to detect multicollinearity and remove redundant variables.
- **Feature Importance**: Utilizing models like Random Forest and XGBoost to rank features by their importance based on predictive power.
- **Recursive Feature Elimination (RFE)**: Iteratively removing less significant features to optimize the model's performance and select the most impactful predictors.

## Evaluation Metrics

The models are evaluated using the following metrics to ensure a comprehensive performance assessment:

- **Accuracy**: Measures the proportion of correct predictions out of total predictions.
- **Precision**: Calculates the proportion of true positive predictions out of all positive predictions made by the model, highlighting the relevance of predictions.
- **Recall**: Measures the model's ability to identify all relevant positive cases, showing sensitivity towards actual positives.
- **F1 Score**: The harmonic mean of precision and recall, providing a balanced measure of performance, especially in cases of class imbalance.
- **AUC (Area Under the Curve)**: Evaluates the model's ability to distinguish between positive and negative classes across different threshold settings.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


## Acknowledgements

This project utilizes various tools and libraries that greatly contributed to its development. Special thanks to:

- **[Scikit-learn](https://scikit-learn.org/)**: For providing a robust suite of machine learning algorithms and utilities.
- **[Pandas](https://pandas.pydata.org/)** and **[NumPy](https://numpy.org/)**: For data manipulation and statistical analysis.
- **[Matplotlib](https://matplotlib.org/)** and **[Seaborn](https://seaborn.pydata.org/)**: For enabling clear and informative data visualizations.
- **[XGBoost](https://xgboost.readthedocs.io/en/latest/)**: For high-performance gradient boosting.
  
Additionally, thank you to all open-source contributors and the data providers who made this project possible.
