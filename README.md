
# Bank Application Prediction with XGBoost and SageMaker
This project demonstrates how to train and deploy an XGBoost model for predicting outcomes in a bank application dataset using Amazon SageMaker. It covers data preparation, model training, deployment, and evaluation.

## Project Structure

### 1. Setting up the Environment:
- Install necessary dependencies using !pip install --upgrade numexpr.
- Import required libraries, including sagemaker and boto3.
- Create an S3 bucket.
  
### 2. Loading and Preparing Data:
- Download the dataset from a the URL and loaded it into a Pandas DataFrame.
- Perform a train-test split on the data.
  
### 3. Saving Data to S3:
- Save train and test data into CSV files.
- Upload data to S3 bucket for training.
  
### 4. Setting up XGBoost Estimator:
- Retrieve the XGBoost container image URI for the specified region and version.
- Initialize hyperparameters for XGBoost.
- Construct a SageMaker estimator for training.
  
### 5. Training the Model:
- Fit the estimator using the training and validation datasets.
  
### 6. Deploying the Model:
- Deploy the trained model to a SageMaker endpoint for making predictions.
  
### 7. Making Predictions:
- Use the deployed model to make predictions on the test data.
  
### 8. Evaluating Model Performance:
- Calculate the confusion matrix and classification rates to evaluate model performance.
