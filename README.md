# Categorical-features-imputation-with-R
## Missing Data Imputation in Car Category Prediction
This project focuses on imputing missing values in the car category variable using different imputation methods. The car category variable represents the category of cars owned by individuals, such as "Economique," "Luxe," or "Standard." The missing values in this variable can be imputed using various techniques, including conditional mode imputation, AFD (Analysis Factorial Discriminant), and Logit-Probit imputation.

## Dataset
The project uses a dataset named Demo that contains information about individuals, including their age, income category, and car category. The dataset may contain missing values in the car category variable (carcatNA). The goal is to impute these missing values using different imputation methods and evaluate their effectiveness.

## Implementation
The project is implemented using the R programming language. The following methods are used for missing data imputation:

Conditional Mode Imputation: This method imputes missing values based on the mode of the car category variable given the income category. It calculates the mode for each income category and assigns it to the missing values in the car category.

AFD (Analysis Factorial Discriminant): AFD is a statistical technique used to classify data into different categories based on multiple variables. In this method, the AFD model is trained using the complete data, and the model coefficients are used to calculate the scores for each observation with missing car category values. The scores are then used to determine the most likely car category for each observation.

Logit-Probit Imputation: This method uses logistic regression to impute missing values in the car category variable. It builds a logistic regression model using the available data, considering age and income category as predictors. The model is then used to predict the car category for observations with missing values.

## Evaluation
The imputation methods are evaluated based on their accuracy in predicting the car category for the observations with missing values. The accuracy is calculated by comparing the imputed values to the actual values in the dataset. The evaluation includes the following metrics:

## Confusion Matrix: The confusion matrix shows the distribution of predicted car categories compared to the actual categories.
Accuracy: The accuracy score represents the proportion of correctly predicted car categories out of all the imputed values.
Usage
To use this project, follow these steps:

Prepare your dataset: Make sure your dataset contains the necessary variables, including age, income category, and car category. The car category variable should have missing values denoted as NA.

Install the required dependencies: This project relies on the R programming language and the following packages: MASS, mice. Make sure you have these packages installed.

Import the dataset: Load your dataset into the R environment and assign it to the variable Demo.

Run the code: Execute the provided R code, which includes the implementation of the different imputation methods and the evaluation of their accuracy.

Analyze the results: Examine the confusion matrices and accuracy scores obtained for each imputation method to assess their performance.

Choose the best imputation method: Based on the evaluation results, select the imputation method that yields the highest accuracy score for your specific dataset and requirements.
