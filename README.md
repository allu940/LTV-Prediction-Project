# Customer Lifetime Value (LTV) Prediction

This project uses a machine learning model to predict the monetary lifetime value of customers based on their past transaction behavior. It leverages **RFM (Recency, Frequency, Monetary)** analysis and an **XGBoost Regressor** to identify high-value customers, enabling targeted marketing strategies.

---

##  Project Objective

The primary goal is to build a predictive model that can estimate a customer's future monetary value. By segmenting customers into different value tiers (e.g., Low, Medium, High), businesses can:

*  Reward high-value customers to improve retention.  
*  Nurture medium-value customers to increase their spending.  
*  Re-engage low-value customers with targeted campaigns.

---

##  Features

* **Data Simulation**: Generates a realistic customer transaction dataset for demonstration purposes.
* **RFM Feature Engineering**: Automatically calculates Recency, Frequency, and Monetary values for each customer from the raw transaction data.
* **XGBoost Model Training**: Trains a powerful Gradient Boosting model (XGBoost) to predict the monetary value based on recency and frequency.
* **Model Evaluation**: Assesses the model's performance using standard regression metrics like Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
* **LTV Prediction & Segmentation**: Predicts the LTV for all customers and segments them into *Low Value*, *Medium Value*, and *High Value* tiers.
* **Data Visualization**: Includes plots for model performance (Actual vs. Predicted) and customer segment distribution.

---

##  Files in this Repository

* `ltv_prediction_script.ipynb` / `.py`: The main Jupyter Notebook or Python script containing all the code for data processing, feature engineering, model training, and prediction.
* `ltv_xgb_model.joblib`: The pre-trained XGBoost regression model. This saved file can be loaded to make new predictions without needing to retrain the model.
* `ltv_predictions.csv`: The final output file. It contains the `CustomerID`, their `Predicted_LTV`, and their assigned `LTV_Segment`.
* `README.md`: This file, providing a comprehensive overview of the project.

---

##  Technologies Used

* **Python**: The core programming language used for the project.
* **Pandas**: For data manipulation and analysis, especially for handling the transaction data and RFM dataframe.
* **NumPy**: For numerical operations.
* **Scikit-learn**: For splitting the data and evaluating the model (`train_test_split`, `mean_absolute_error`).
* **XGBoost**: The machine learning library used to build the high-performance gradient boosting regression model.
* **Matplotlib & Seaborn**: For creating visualizations.
* **Joblib**: For saving and loading the trained machine learning model.
