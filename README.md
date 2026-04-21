# Rainfall Prediction Web App

This repository contains a web application that predicts whether there will be rainfall based on weather-related features. The app uses a machine learning model to make the prediction based on the following features:

1. Pressure
2. Dewpoint
3. Humidity
4. Cloud
5. Sunshine
6. Wind Direction
7. Wind Speed

## Files in the Repository

1. app.py
   
This is the main Python file that runs the Flask web application. It performs the following functions:

Initializes the Flask App: It sets up the basic web framework and routes.
Loads the Model: It connects to MLflow to load the production version of the rainfall prediction model.
Handles Predictions: It captures input data from the user, formats it into a DataFrame, and uses the model to predict whether there will be rainfall.
Prediction Result Display: It shows the result ("Rainfall" or "No Rainfall") to the user on the web page.

2. Rainfall_Prediction.ipynb
   
This Jupyter notebook contains the code and logic to train the machine learning model that predicts rainfall. It involves:

Data Exploration: Analyzing the provided dataset.
Model Training: Using machine learning algorithms to build a model that can predict rainfall based on the provided features.
Model Evaluation: Evaluating the model's performance and saving the trained model for later use.

3. Rainfall.csv
   
This CSV file contains the dataset used for training the machine learning model. The dataset includes multiple weather features like pressure, humidity, and wind speed, along with the target variable (whether there was rainfall).

5. index.html
   
This is the HTML file that provides the frontend interface for the user. The web page allows the user to input the following weather features:

Pressure
Dewpoint
Humidity
Cloud
Sunshine
Wind Direction
Wind Speed
Once the user submits the form, the app sends the data to the backend, which processes it and returns the prediction.

How to Run

01. Ensure that the machine learning model is correctly saved and loaded using MLflow. The model should be available at models:/rainfall-prediction-production@prod.

02. Run the app.py file to start the web server: "python app.py"

03. Open a browser and navigate to http://127.0.0.1:8080/ to access the web application.

04. Enter the weather features in the form and click Predict to get the prediction result.

<img width="1919" height="1038" alt="Screenshot 2026-04-21 224605" src="https://github.com/user-attachments/assets/709dbd4a-fad8-44f3-bb08-0c52db36ae0d" />

<img width="1919" height="1039" alt="Screenshot 2026-04-21 224630" src="https://github.com/user-attachments/assets/eb916326-7ef9-467e-9d51-77d28c0807d7" />

<img width="1919" height="1039" alt="Screenshot 2026-04-21 224653" src="https://github.com/user-attachments/assets/76139b81-5fda-4424-9d7e-201d39e0115c" />

<img width="1919" height="1041" alt="Screenshot 2026-04-22 001658" src="https://github.com/user-attachments/assets/0d62e0e3-233d-4cef-b117-84a7eae089c8" />

<img width="1919" height="1039" alt="Screenshot 2026-04-22 000228" src="https://github.com/user-attachments/assets/f613aad8-9af9-4a8c-a874-3e0f9a3b2bf1" />

<img width="1919" height="1042" alt="Screenshot 2026-04-22 000421" src="https://github.com/user-attachments/assets/203d9718-941a-4c7d-9174-37a444003bd1" />

