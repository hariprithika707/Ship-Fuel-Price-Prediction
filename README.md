Ship Fuel Consumption Prediction (SIH)
Overview
This project focuses on predicting ship fuel consumption based on the mean draft of the ship. A machine learning model is trained using Lasso regression to provide accurate predictions.

Table of Contents
Project Structure
Features
Installation
Usage
Model Details
Dataset
Results
License
Project Structure
php
Copy code
ship_fuel_sih/
├── app/
│   ├── templates/
│   │   └── index.html
│   ├── static/
│   ├── model/
│   │   └── lasso_model.sav
│   ├── app.py
│   └── requirements.txt
├── notebooks/
│   └── ship_fuel_sih.ipynb  # Jupyter notebook for model development
└── README.md
Features
Fuel Consumption Prediction: Predicts fuel consumption based on the ship’s mean draft using a Lasso regression model.
Flask Interface: Provides a basic interface for interacting with the model (not yet deployed).
Installation
Prerequisites
Python 3.12.7 or higher
Flask
Scikit-learn
Pandas
Numpy
Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/ship_fuel_sih.git
cd ship_fuel_sih
Install Dependencies
bash
Copy code
pip install -r requirements.txt
Usage
Run Locally
Ensure the Lasso regression model (lasso_model.sav) is in the model/ folder.
Start the Flask application:
bash
Copy code
python app.py
Open your web browser and go to http://localhost:5000. Enter the meanDraft to predict the fuel consumption of the ship.
Use the Jupyter Notebook
Open notebooks/ship_fuel_sih.ipynb and run the cells to train the model, explore the dataset, and make predictions.

Model Details
Input: meanDraft
Output: Predicted fuel consumption
Model: Lasso regression model trained using Python’s Scikit-learn library.
Training Process
The model was trained using a dataset that contains records of ship drafts and corresponding fuel consumption. Lasso regression was chosen for its ability to handle overfitting by penalizing less important features.

Dataset
The dataset used for training contains ship draft measurements and corresponding fuel consumption values. This dataset is not included in this repository for privacy and proprietary reasons.

Results
The Lasso regression model provides accurate predictions of fuel consumption based solely on the ship’s mean draft. Additional features (e.g., ship speed, cargo weight) can potentially improve the model's accuracy.

License
This project is licensed under the MIT License - see the LICENSE file for details.
