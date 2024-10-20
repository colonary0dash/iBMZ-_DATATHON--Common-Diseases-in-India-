**Disease Medication Prediction**
Description : This project is about predicting the right medications for diseases based on the patient's age, disease, symptoms, and the duration of the disease (called Period in the dataset).

We use machine learning to classify diseases and give the medications they need. The main algorithm used is RandomForestClassifier from scikit-learn. It's a simple but powerful classifier.

Dataset
The dataset is a CSV file called IBMz_CommonDisease_Dataset0.csv. 

It has 20,000 rows with the following columns:
 Disease:  The type of illness (e.g., Cold, Stomach Ache).
 Age:      Age of the patient.
 Period:   Number of days the patient has had the disease.
 Symptoms: List of symptoms the patient is experiencing.
 Medications: Recommended medications for the disease.


Installation:
You will need the following libraries to run the code:
pandas
scikit-learn
matplotlib
seaborn
numpy
You can install them using pip:

bash
Copy code
pip install pandas scikit-learn matplotlib seaborn numpy
Usage
Load the dataset:
python
df = pd.read_csv('IBMz_CommonDisease_Dataset0.csv')
Explore the dataset:
python
Copy code
print(df.head())  # Shows the first 5 rows
print(df.tail())  # Shows the last 5 rows
print(df.info())  # Shows the structure of the dataset
Preprocess and split the dataset into training and testing sets.

Train the RandomForestClassifier model and evaluate it using accuracy and classification report.

Output
The model predicts the medications that should be prescribed based on the disease and other input features.
example:
for the code
 Disease_input = 'Cold'   # Example input
Age_input = 12
Period_input = 2  
Symptoms_input = 'Runny Nose' # Example: Time in years
predicted_Med = predict_Medications(Disease_input, Age_input, Period_input, Symptoms_input )
print(f"Predicted Medications: {predicted_Med}")
print("Thank You for Using Avinaash! This is for Primary Consultency Only, We always suggest you to Visit a Doctor!")
 output:
  Predicted Medications: Relent Tablet / Syrup
Thank You for Using Avinaash! This is for Primary Consultency Only, We always suggest you to Visit a Doctor!

Although we are So much sure about our Model Avinaash's Predictions,
We respect and care The User lot More,


Future Work
Add more machine learning models for specific large data 
Do hyperparameter tuning to improve the accuracy.
Add visualization for feature importance.
License
This project is open-source.
