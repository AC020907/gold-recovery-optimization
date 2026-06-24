# Gold Recovery Prediction using Machine Learning

## Project Description

This project develops a Machine Learning solution to predict gold recovery in an industrial mining extraction process.

Zyfra aims to optimize production through predictive models capable of estimating gold recovery efficiency at different stages of the refining process. To achieve this, real-world data collected from sensors and operational variables within a mining plant were used.

The project includes data cleaning, exploratory data analysis, feature engineering, model training, and evaluation using a custom metric based on sMAPE.

## Objective

Build a model capable of accurately predicting gold recovery during the processing and concentration stages, enabling better operational decision-making and improving production efficiency.

## Dataset

The dataset contains information from different stages of the mining extraction process, including:

- Flotation parameters.
- Metal concentrations.
- Process operational variables.
- Gold recovery measurements.
- Input and output variables from different production stages.

The project uses separate training and testing datasets provided by the company.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Methodology

### 1. Data Preparation

- Initial dataset inspection.
- Missing value treatment.
- Removal of variables unavailable during production.
- Data consistency verification.
- Alignment of training and testing datasets.

### 2. Exploratory Data Analysis

The following analyses were performed:

- Distribution of key variables.
- Metal concentrations across different processing stages.
- Gold recovery behavior.
- Outlier detection and anomalous observations.

### 3. Feature Engineering

- Selection of relevant features.
- Removal of redundant columns.
- Preparation of target variables.
- Construction of the final training datasets.

### 4. Model Training

Several regression algorithms were evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

The models were compared using cross-validation.

### 5. Model Evaluation

The primary evaluation metric was:

**sMAPE (Symmetric Mean Absolute Percentage Error)**

This metric measures the percentage prediction error while giving balanced importance to both high and low values.

Additionally, the final evaluation metric used by Zyfra was implemented to simultaneously assess both stages of the gold recovery process.

## Results

Tree-based models achieved better performance than traditional linear regression.

After hyperparameter optimization and cross-validation, the model with the lowest sMAPE score was selected for the final evaluation.

The results demonstrate that the selected model is capable of capturing meaningful patterns in the industrial process and generating useful predictions for mining operations.

## Conclusions

- A predictive model was successfully developed to estimate gold recovery at different stages of the industrial process.
- Exploratory data analysis identified inconsistencies and critical variables for prediction.
- Machine Learning models outperformed the baseline approaches used for comparison.
- The sMAPE metric proved effective for evaluating prediction quality in an industrial environment.
- The selected model can serve as a decision-support tool for optimizing mining recovery processes.

## Skills Demonstrated

- Industrial data cleaning and preprocessing.
- Exploratory Data Analysis (EDA).
- Feature engineering.
- Supervised regression modeling.
- Cross-validation.
- Hyperparameter optimization.
- Custom metric implementation.
- Machine Learning model evaluation.
- Technical and business results communication.

## Repository Structure

```text
gold-recovery-prediction-ml/
│
├── data/
│   ├── gold_recovery_train.csv
│   ├── gold_recovery_test.csv
│   └── gold_recovery_full.csv
│
├── notebooks/
│   └── proyecto_sprint_12.ipynb
│
├── README.md
└── requirements.txt
```

## Author

**Alejandro Cotes**  
Data Science Student | Machine Learning | Analytics
