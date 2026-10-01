# Customer Churn Predictor

A machine learning project for customer churn prediction using Python.

This project is intended for experimentation and learning purposes.

## Project Overview

This project demonstrates building, training, and evaluating a model to predict whether a customer will churn based on input features.

## Files

- `customer_churn_system1.py` - Main script that loads data, trains a model, and evaluates predictions.
- `churn setup.ipynb` - Jupyter notebook for exploratory data analysis and modeling workflow.
- `requirements.txt` - Python dependencies for this project.
- `README.md` - This documentation file.

## Setup Instructions

1. Create and activate Python environment (recommended):

```powershell
python -m venv venv
venv\Scripts\Activate.ps1
```

2. Install dependencies:

```powershell
pip install -r requirements.txt
```

3. Run the script:

```powershell
python customer_churn_system1.py
```

4. Open the notebook for interactive exploration:

```powershell
jupyter notebook "churn setup.ipynb"
```

## Expected behavior

- Model training should run and print metrics like accuracy and confusion matrix.
- Prediction output indicates whether individual customers are expected to churn.

## How to contribute

- Add or clean data inputs in the notebook.
- Improve model selection, featurization, preprocessing steps.
- Add tests for data validation and prediction quality.

## License

Add your license details here as needed.

## Future Improvements

- Experiment with additional algorithms such as Random Forest, Gradient Boosting, and XGBoost to compare performance against the baseline model.
- Add hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Handle class imbalance with techniques like SMOTE or class weighting.
- Package the trained model so it can be loaded for predictions without retraining.

## Evaluation Metrics

Beyond accuracy, the model should be assessed with metrics that matter for churn problems:

- **Precision and recall**: to understand how many predicted churners are real, and how many real churners are caught.
- **F1-score**: to balance precision and recall when classes are uneven.
- **ROC-AUC**: to measure how well the model separates churners from non-churners across thresholds.

## Troubleshooting

- If `Activate.ps1` is blocked in PowerShell, run `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass` and try again.
- If a package fails to install, upgrade pip first with `python -m pip install --upgrade pip`.
- If the notebook does not open, confirm Jupyter is installed by running `pip install notebook`.

## Contact

For questions, suggestions, or feedback, feel free to open an issue in this repository.

Dataset (where the data comes from, columns, target variable)
Model Results (the accuracy, precision, recall and ROC-AUC your run produced)
Running the App (the script uses Streamlit, so add streamlit run customer_churn_system1.py if that's how it launches)

Docker (the repo has a Docker build workflow, so how to build and run the image)
Known Issues (e.g. the 30 Ruff lint errors currently failing CI)
License (replace "Add your license details here" with something like MIT)

## Dataset

- **Source:** <where the data comes from, e.g. Kaggle Telco Customer Churn>
- **Rows and columns:** <number of customers> customers, <number> features
- **Target variable:** `Churn` (Yes/No), indicating whether the customer left.
- **Key features:** <e.g. tenure, contract type, monthly charges, payment method>

## Model Results

Results from the latest run of `customer_churn_system1.py`:

| Metric    | Score    |
|-----------|----------|
| Accuracy  | <value>  |
| Precision | <value>  |
| Recall    | <value>  |
| F1-score  | <value>  |
| ROC-AUC   | <value>  |

Scores will vary slightly depending on the train/test split and random seed.

## Running the App

The project includes a Streamlit interface. After installing dependencies, launch it with:

```powershell
streamlit run customer_churn_system1.py
```

Then open the local URL shown in the terminal (usually `http://localhost:8501`).
