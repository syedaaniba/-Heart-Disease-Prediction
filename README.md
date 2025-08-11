# Heart Disease Prediction

This project uses machine learning to predict the presence of heart disease based on patient data. It utilizes a **Logistic Regression** model and a pipeline for data preprocessing and model training.

---

## The Data

The dataset used in this project is the **Cleveland Heart Disease** dataset from the UCI Machine Learning Repository. It contains 14 features, including clinical and demographic information, and a target variable indicating the presence of heart disease.

---

## Project Structure

The main script is `heart_disease_predictor.py`. It performs the following steps:
- **Data Loading and Cleaning**: The dataset is loaded, missing values are handled, and the target variable is prepared.
- **Preprocessing**: A `ColumnTransformer` is used to scale numerical features and leave categorical features untouched.
- **Model Training**: A `Pipeline` combines the preprocessing and a `LogisticRegression` classifier.
- **Hyperparameter Tuning**: A `GridSearchCV` with `StratifiedKFold` is used to find the best hyperparameters for the model.
- **Evaluation**: The final model is evaluated on a test set, and its performance is reported using **accuracy**, a **confusion matrix**, and a **classification report**.

---

## How to Run It Yourself

It's pretty straightforward to get this project running. Just follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [your_repo_url]
    ```

2.  **Go into the project folder:**
    ```bash
    cd heart_disease_prediction
    ```

3.  **Install the libraries:** Make sure you have **pandas** and **scikit-learn** installed. If not, just run:
    ```bash
    pip install pandas scikit-learn
    ```

4.  **Execute the script:**
    ```bash
    python heart_disease_predictor.py
    ```

---

## Result 
## Best parameters found:
`{'classifier__C': 1, 'classifier__solver': 'lbfgs'}`

## Accuracy on test set:
`0.8833`

## Confusion Matrix:
[[32 4]
[ 3 21]]

shell
Copy
Edit

## Classification Report:
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.91      | 0.89   | 0.90     | 36      |
| 1     | 0.84      | 0

## Final Results

After running the script, the following results are printed to the console:
