# Predicting Flight Delays :airplane:

The growth of the aviation sector has made flight delaysmore common across the world.  They cause inconvenienceto the travellers and incur monetary losses to the airlines.We analysed the various factors responsible for flight delaysand applied machine learning models such as **Random Forest, XGBoost, Logistic Regression, Decision Tree and NaiveBayes** to predict whether a given flight would be delayed ornot.  The `XGBoost Classifier` performed exceptionally well, giving an accuracy of `0.88` and an AUC of `0.93`.

## Dataset
We used the 2015 Flight Delays and Cancellations Dataset, collected and published by U.S. DOT’s Bureau of Transportation Statistics. After cleaning, a dataset with dimensions `456697 × 11` was obtained.

- **Categorical Features:** Airline, Origin, Destination
- **Numerical Features:** Distance, Taxi Out, Departure Delay, Day of Week, Arrival Delay
- **Date/Time Features:** Date, Scheduled Departure, Scheduled Arrival

## Usage

### Google Colab

- Open the Notebook.ipynb file on Google Colab
- Copy [this](https://drive.google.com/drive/folders/1HRDxih_6xN0uU2Js3xGF8zp5r_XPSEJc?usp=sharing) folder to your Google Drive
- Mount the Google Drive and modify the folder path in the preprocess method accordingly.

### Local System

- Install necessary modules : `pip install -r requirements.txt` 
- Download the datasets from [here](https://drive.google.com/drive/folders/1HRDxih_6xN0uU2Js3xGF8zp5r_XPSEJc?usp=sharing).
- Modify the folder path in the preprocess method accordingly.
