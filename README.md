# Customer Churn Prediction

This project uses machine learning to predict customer churn. It utilizes a **Logistic Regression** model and a pipeline for data preprocessing and model training.

---

## The Data

The dataset used in this project is not specified, but it contains customer information and a target variable indicating whether a customer has churned (left the service).

---

## Project Structure

The main script is `customer_churn_predictor.ipynb`. It performs the following steps:
- **Data Loading and Cleaning**: The dataset is loaded, and any necessary data cleaning or preparation is performed.
- **Preprocessing**: Data is prepared for the model, which may include scaling numerical features and encoding categorical features.
- **Model Training**: A `Pipeline` is used to combine the preprocessing steps and a **Logistic Regression** classifier.
- **Hyperparameter Tuning**: The best model is selected through a process of tuning the model's parameters.
- **Evaluation**: The final model is evaluated on a test set, and its performance is reported.

---

## How to Run It Yourself

It's pretty straightforward to get this project running. Just follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/syedaaniba/customer-churn-prediction_.git](https://github.com/syedaaniba/customer-churn-prediction_.git)
    ```

2.  **Go into the project folder:**
    ```bash
    cd customer-churn-prediction_
    ```

3.  **Install the libraries:** Make sure you have **pandas** and **scikit-learn** installed. If not, just run:
    ```bash
    pip install pandas scikit-learn
    ```

4.  **Launch the notebook:**
    ```bash
    jupyter notebook customer_churn_predictor.ipynb
    ```

---

## Final Results

Best parameters found:  {'classifier__C': 1, 'classifier__solver': 'lbfgs'}
Accuracy on test set: 0.8833
Confusion Matrix:
[[32  4]
 [ 3 21]]
Classification Report:
              precision    recall  f1-score   support

           0       0.91      0.89      0.90        36
           1       0.84      0.88      0.86        24

    accuracy                           0.88        60
   macro avg       0.88      0.88      0.88        60
weighted avg       0.88      0.88      0.88        60

After running the notebook, the following results are printed to the console:
