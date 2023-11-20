# Salary Prediction Model Based on Job Descriptions

This project focuses on creating a predictive model for estimating salaries based on job descriptions. The model is designed to aid job seekers in understanding salary ranges for different occupations. By leveraging machine learning techniques, the goal is to predict the salaries of various job positions accurately.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Getting Started](#getting-started)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Development](#model-development)
- [Performance Evaluation](#performance-evaluation)
- [Deployment](#deployment)
- [Conclusion](#conclusion)
- [Author](#author)
- [License](#license)

## Project Overview

The primary objective of this project is to build a predictive analytics model capable of estimating salaries for various job positions. It involves the analysis of job descriptions, such as job type, degree, major, industry, years of experience, and distance from metropolis, to predict corresponding salaries. By employing machine learning algorithms, we aim to develop a model that accurately predicts salaries based on these features.

## Dataset

The dataset used for this project consists of multiple CSV files:

- `train_features.csv`: Contains job-related features for training the model.
- `train_salaries.csv`: Includes the corresponding salaries for the training data.
- `test_features.csv`: Contains job-related features for testing the model's predictions.

The dataset contains information such as job ID, company ID, job type, degree, major, industry, years of experience, distance from metropolis, and the associated salary.

## Getting Started

To replicate or run this project on your local machine, follow these steps:

1. Clone this repository to your local machine using `git clone <repository_url>`.
2. Install the required dependencies mentioned in the `requirements.txt` file using `pip install -r requirements.txt`.
3. Download the dataset files (`train_features.csv`, `train_salaries.csv`, `test_features.csv`) and place them in the `data` directory within the cloned repository.

## Data Preparation

The initial step involved loading the dataset into Pandas dataframes and performing data cleaning tasks, including:

- Checking for duplicate entries
- Removing null values and invalid data (salary values <= 0)
- Exploring and visualizing the distributions of features
- Handling outliers and analyzing their impact on the dataset

## Exploratory Data Analysis (EDA)

The EDA phase included:

- Summary statistics of continuous and categorical variables
- Visualizations (boxplots, histograms, and correlation matrices) to understand feature distributions and relationships with the target variable (salary)
- Examining correlations between different features and the target variable

## Model Development

For model development, we experimented with several machine learning algorithms:

- Linear Regression
- Random Forest Regression
- Gradient Boosting Regressor
- XGBoost Regressor

## Performance Evaluation

The models were evaluated using Mean Squared Error (MSE) as the performance metric. The MSE scores were calculated via cross-validation to measure the model's accuracy in predicting salaries.

## Deployment

The chosen Gradient Boosting Regressor model was trained on the entire dataset and utilized to predict salaries for the test dataset (`test_features.csv`). The predictions were stored in a CSV file named `Salary_Predictions.csv`.

## Conclusion

This project successfully built a machine learning model capable of predicting salaries based on job descriptions with a reasonable level of accuracy. Further improvements could involve feature engineering, hyperparameter tuning, or exploring advanced machine learning techniques for better performance.

## Author

- **Author**: Ajuni Sohota
- **Email**: ajunisohota@gmail.com

## License

This project is licensed under the [MIT License](LICENSE).

---
