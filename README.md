# Job Forecast : Missing Values Imputation using Machine Learning Predictions

## Project Overview

This project aims to replace missing values in a dataset with predictions generated using machine learning algorithms. In this README, we will provide an overview of the project, explain its objectives, and guide you through the code and its functionalities.

## Getting Started

To get started with this project, follow these steps:

1. **Data Preparation**: The dataset is loaded from a CSV file named 'data.csv'. Make sure to provide your dataset or update the file path accordingly.

2. **Data Exploration and Preprocessing**:
   - The dataset is explored to identify missing values, which are then handled using predictive imputation.
   - The 'Experience' column is preprocessed to replace ',' with '.' and convert it to numeric data.
   - Various statistics, such as mean and median years of experience, are calculated for different job titles ('Metier').

3. **Visualization**:
   - Visualizations are generated to better understand the dataset:
     - Histograms, box plots, and violin plots for 'Experience' by job title.
     - Analysis of the most frequently used technologies.
     - Encoding of 'Entreprise' and 'City' variables.
     - Visualizations related to population size by city.

4. **Machine Learning Models**:
   - The dataset is split into labeled data with job titles ('df_encoded') and unlabeled data with missing job titles ('df_NaN').
   - Classification models, including k-Nearest Neighbors, Multi-layer Perceptron, Support Vector Machine, Gradient Boosting, Random Forest, and Naive Bayes, are trained and evaluated based on accuracy.

5. **Model Selection and Hyperparameter Tuning**:
   - The top-performing models (Gradient Boosting, Multi-layer Perceptron, and SVM) are selected for hyperparameter tuning using GridSearchCV to optimize their performance.

6. **Model Evaluation**:
   - Detailed classification reports are generated for the selected models, including precision, recall, F1-score, and support.

7. **Receiver Operating Characteristic (ROC) Analysis**:
   - ROC curves and Area Under the Curve (AUC) scores are calculated to evaluate model performance further.

8. **Feature Importance**:
   - The top 10 important features for the Gradient Boosting model are visualized.

9. **Missing Value Imputation**:
   - Missing job titles ('Metier') in the unlabeled dataset ('df_NaN') are predicted using the Gradient Boosting model.

## Prerequisites

Ensure you have the following dependencies installed:

- Google Colab (if running the code in a Colab environment)
- Python 3.x
- Pandas
- Matplotlib
- NumPy
- Seaborn
- Scikit-learn

## Usage

To run this project:

1. Clone the repository to your local machine or open it in your preferred Python environment.

2. Replace the 'data.csv' file with your dataset or ensure that it is correctly located in the specified path.

3. Execute the code step by step to explore, preprocess, visualize, and apply machine learning models to the dataset.

4. Follow the instructions provided in the code comments for each section.

## Results

This project provides a comprehensive solution for handling missing data by predicting job titles using machine learning models. The Gradient Boosting model is used for the final prediction, and the missing job titles are imputed based on the model's predictions. The project also includes model evaluation, ROC analysis, feature importance, and detailed visualizations.

## Contributors

- Julien Esposito

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
