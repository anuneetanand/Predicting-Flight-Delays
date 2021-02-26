# Predicting Flight Delays :airplane:

The growth of the aviation sector has made flight delaysmore common across the world.  They cause inconvenience to the travellers and incur monetary losses to the airlines. We analysed the various factors responsible for flight delaysand applied machine learning models such as **Random Forest, XGBoost, Logistic Regression, Decision Tree, NaiveBayes** to predict whether a given flight would be delayed or not.  The **XGBoost Classifier** performed exceptionally well, giving an Accuracy of 0.88 and an AUC of 0.93.

## Dataset :bar_chart:
We used the 2015 Flight Delays and Cancellations Dataset, collected and published by U.S. DOT’s Bureau of Transportation Statistics. After cleaning, a dataset with dimensions 456697 × 11 was obtained.

- **Categorical Features:** Airline, Origin, Destination
- **Numerical Features:** Distance, Taxi Out, Departure Delay, Day of Week, Arrival Delay
- **Date/Time Features:** Date, Scheduled Departure, Scheduled Arrival

## Exploratory Data Analysis :mag_right:
- We identified the busiest airports and air traffic shares of different airlines and visualised the mean delays in airlines on different days of the week. It was observed that most flights were delayed on Sunday and Monday.  
- Alaska Airlines Inc. and Delta Air Lines Inc. were the best performing airlines whereas Frontier Airlines Inc. and American Eagle Airlines Inc. were often delayed. 
- It was found that the mean delays of flight dropped with an increase in route distance. However, flights travelling distances over 3000Km showed a spike in delays. 
- We also conducted a statistical study of different numerical features in the dataset and derived important insights about their distributions. It was found that almost 68% of the flights had no delay or a delay of less than 3 minutes.

## Methodology :gear:

To validate the performance of our models, we per- formed a train-val-test split of 70:10:20. We trained Random Forest Classifier, XGBoost Classifier, Naive Bayes Classifier, Decision Tree and Logistic Regression, from the Sklearn library, on the training set. Grid Search CV was used to find optimal hyper-parameters for the models. Appropriate graphs and metrics were generated for the analysis and performance of the different models were compared.

## Results :dart:

We can conclude that Random Forest Classifier and XG- Boost Classifier performed significantly well in predicting flight delays. XGBoost Classifier had a slight edge over Random Forest Classifier and fitted the problem statement better with an accuracy score of 0.88 and AUC score of 0.93.

|              |        |       |       |       |       |
|--------------|--------|-------|-------|-------|-------|
|              |  LR    | GNB   | DT    | XGB   | RF    |
| Precision    |  0.88  | 0.79  | 0.72  | 0.89  | 0.88  |
| Recall       |  0.73  | 0.68  | 0.74  | 0.75  | 0.74  |
| F1-score     |  0.79  | 0.73  | 0.73  | 0.81  | 0.80  |

## Usage

### Google Colab

- Open the Notebook.ipynb file on Google Colab
- Copy [this](https://drive.google.com/drive/folders/1HRDxih_6xN0uU2Js3xGF8zp5r_XPSEJc?usp=sharing) folder to your Google Drive
- Mount the Google Drive and modify the folder path in the preprocess method accordingly

### Local System

- Install necessary modules : `pip install -r requirements.txt` 
- Download the datasets from [here](https://drive.google.com/drive/folders/1HRDxih_6xN0uU2Js3xGF8zp5r_XPSEJc?usp=sharing)
- Modify the folder path in the preprocess method accordingly

## Collaborators
[Rhythm Patel](https://github.com/rhythm-patel)      
[Mohnish Agrawal](https://github.com/Mohnish-Agrawal)

