# HealthHub: Personalized Wellness Navigator

## Overview
This Jupyter Notebook implements a Health Disease Predicting System, which predicts diseases based on symptoms provided by the user. It utilizes a machine learning algorithm, Random Forest, to make predictions. The notebook also includes a feature to find hospitals based on the predicted disease.

## Features
- Predicts diseases based on symptoms provided by the user.
- Utilizes Random Forest algorithm for disease prediction.
- Provides recommendations for hospitals based on the predicted disease.
- Allows users to input patient information and symptoms for prediction.

## Requirements
- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, tkinter

## How Random Forest Algorithm Works for Disease Prediction
The Random Forest algorithm is an ensemble learning technique that constructs multiple decision trees during training and outputs the mode of the classes (classification) or the mean prediction (regression) of the individual trees. Here's how it works for disease prediction in this system:
1. **Data Preparation**: The dataset containing symptoms and corresponding diseases is prepared for training. Each row represents a patient's symptoms, and the target variable is the disease.
2. **Training the Model**: The Random Forest classifier is trained on the dataset. During training, the algorithm builds multiple decision trees, each trained on a random subset of the data and using a random subset of the features.
3. **Making Predictions**: When a new set of symptoms is provided, the trained Random Forest model predicts the most likely disease based on the input symptoms. It combines the predictions from each decision tree to make the final prediction.
4. **Evaluating Accuracy**: The accuracy of the model is evaluated using testing data to assess its performance in predicting diseases accurately.

## How Hospitals are Recommended Based on Predicted Disease
After predicting the disease using the Random Forest algorithm, the system recommends hospitals based on the predicted disease category. A mapping between diseases and hospital categories is predefined, associating each disease with a specific type of hospital or medical facility. This mapping is used to recommend the appropriate hospital category based on the predicted disease.

The disease is predicted like this:

<img width="686" alt="Screenshot 2024-04-24 at 11 00 22 PM" src="https://github.com/Ana4506/HealthHub/assets/89125989/7c4a9815-fad1-47b1-a4f2-e532ab447733">


The hospitals recommended to cure that disease are shown like this:

<img width="427" alt="Screenshot 2024-04-24 at 11 03 18 PM" src="https://github.com/Ana4506/HealthHub/assets/89125989/3aed7f35-f859-4d4b-bad6-8e3174eeee78">


## Usage
1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Make sure you have the required libraries installed by running:
```bash
   pip install -r requirements.txt
```
4. Open the notebook using Jupyter Notebook or JupyterLab.
5. Run each cell in the notebook sequentially.
6. Fill in the patient's name and select symptoms from the dropdown menus.
7. Click the "Predict" button to predict the disease.
8. The predicted disease will be displayed on the prompted GUI system, along with a scatter plot showing the relationship between symptoms and the predicted disease-curing hospital on the terminal.
9. Optionally, you can reset inputs or exit the system using the respective buttons.

## Additional Information
- The dataset used for training and testing the model is located in the `Dataset` directory.
- The model training and testing are based on the dataset provided.
- The application is developed using Python's tkinter library for the graphical user interface.
- For further details on the code implementation, refer to the notebook.

## Contribution by Ananya Gupta 
