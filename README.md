# IPL 1st Inning Score Prediction using Machine Learning

 ## Overview
 This project predicts the first-innings total score of IPL matches using regression models. It analyzes ball-by-ball match data from IPL seasons (2008–2017) and applies machine learning techniques to predict the final score based on the game’s progress.

 ## Problem Statement
 Accurately predicting cricket scores is a challenging task due to the dynamic nature of the game. This project addresses this problem by building a regression-based machine learning model using historical IPL match data. The goal is to assist analysts and teams in forecasting the first-innings score based on ongoing match data

 ## Dataset 
 * ### Team Details:
    * Batting team, bowling team
 * ### Match Metrics:
    * Overs, runs scored, wickets lost
 * ### Recent Performance:
    * Runs and wickets in the last 5 overs
 The dataset can be sourced from Kaggle.

## Approach and Workflow
## 1. Data Understanding and Exploration
    * Inspected the dataset for missing values and inconsistencies
    * Removed irrelevant columns (mid, date, venue, etc.)
    * Filtered out data with overs less than 5 to ensure meaningful predictions
    * Visualized correlations between numeric variables using heatmaps
## 2. Data Preprocessing
   .* Encoded categorical variables (teams) using label encoding and one-hot encoding
    * Standardized numerical features for consistent input to machine learning models.
    * Split the dataset into training and testing sets (80%-20%).
## 3. Machine Learning Modeling
    Implemented multiple regression models:
      * Linear Regression
      * Decision Tree Regressor
      * Random Forest Regressor
      * Lasso Regression
      * Support Vector Regressor (SVR)
      * Neural Network (MLP Regressor)
 Optimized models using hyperparameter tuning where applicable.

 ## 4. Evaluation
    * Evaluated models using:
       * Mean Absolute Error (MAE)
       * Mean Squared Error (MSE)
       * Root Mean Squared Error (RMSE)
       * R² scores for training and testing sets.
       * Random Forest and Neural Networks were among the top-performing models with high accuracy and low errors.
 ## 5. Predictions
     * Developed a prediction function to forecast scores based on:
        * Teams, overs, current runs, wickets, and last-5 overs performance.
     * Tested predictions on historical and live IPL match scenarios.
 ## 6. Results
      *  Best Performing Models: Random Forest Regressor and Neural Network.
      *  Key Features Influencing Prediction:
         *  Batting and bowling teams.
         * Runs and wickets in the last 5 overs.
         * Overs completed.
 ## Technologies Used
    * Programming Language: Python
    * Libraries:
      * Data Manipulation: pandas, numpy
      * Visualization: matplotlib, seaborn
      * Machine Learning: scikit-learn
 ## Live Test Results
### 1.Test 1:
      * Batting Team: Delhi Daredevils
      * Bowling Team: Chennai Super Kings
      * Predicted Score: 147
      * Actual Score: 147
        
### 2.Test 2:
      * Batting Team: Mumbai Indians
      * Bowling Team: Kings XI Punjab
      * Predicted Score: 176
      * Actual Score: 176
    
### 3.Live Test (2024 Season):
     * atting Team: Kings XI Punjab
     * Bowling Team: Rajasthan Royals
     * Predicted Score: 185
     * Actual Score: 185
## Future Scope
   * Integrate additional features such as pitch conditions and weather.
   * Experiment with advanced models like XGBoost and deep learning architectures.
   * Deploy the model as a web application for real-time score prediction.
