# House-Price-Prediction

This repository contains a Flask-based web application that predicts house prices using a trained linear regression model. The application takes basic details about a house as input and provides a predicted price as output.

# Features
Data Preprocessing: The dataset is preprocessed to include features such as GrLivArea, BedroomAbvGr, and TotalBath (calculated from FullBath and HalfBath).

Model Training: A linear regression model is trained on the provided dataset to predict house prices.

Web Interface: A simple and interactive web interface allows users to input house features and get price predictions.

Rupee Conversion: The predicted price is converted into Indian Rupees (INR).

# Requirements
The project uses the following Python libraries:

Flask

Joblib

Numpy

Pandas

Scikit-learn

# Files in the Repository
app.py: Contains the Flask application and prediction logic.

train.csv: The dataset used for model training (not included; replace with your dataset).

house_price_model.pkl: Serialized model file (generated after training).

scaler.pkl: Serialized scaler for feature normalization.

templates/: Folder containing the HTML templates for the web interface.

# Running the Application
Clone the repository: 

git clone https://github.com/Shreyabhelekar/PRODIGY_ML_01.git

Navigate to the project directory:

cd PRODIGY_ML_01

Ensure all dependencies are installed: 

pip install -r requirements.txt

Place your training dataset (train.csv) in the root directory.

Run the Flask application: python app.py

Open your browser and go to: http://localhost:5001/


# How It Works
Input: Enter the following house details in the form:

GrLivArea: Above-ground living area in square feet.

BedroomAbvGr: Number of bedrooms above ground.

TotalBath: Total number of bathrooms (calculated as full baths + 0.5 × half baths).

Prediction: The application preprocesses the inputs, scales them using the pre-trained scaler, and predicts the price using the trained linear regression model.

Output: The predicted house price is displayed in Indian Rupees.

# Model Details
Algorithm: Linear Regression

Features Used:
GrLivArea

BedroomAbvGr

TotalBath

The model was trained on a sample dataset (train.csv) and evaluated using the Mean Squared Error metric.


Dataset : - https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data 
