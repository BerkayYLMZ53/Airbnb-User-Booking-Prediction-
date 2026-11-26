# Airbnb User Booking Prediction

A multi-class classification project that explores whether a new Airbnb user's first booking destination can be predicted from demographic information, location preferences, and session activity.

## Project objective

The project investigates how user profile and interaction data can be used to estimate the destination country of a first booking. Potential applications include personalizing recommendations and understanding user preferences.

## Data preparation

The workflow described in this project includes:

- Reviewing missing and incomplete values and applying cleaning or imputation.
- Encoding categorical features with Label Encoding and One-Hot Encoding.
- Scaling continuous features with `StandardScaler`.
- Preparing the data for multi-class model training.

## Models compared

Three classification algorithms are evaluated:

1. **Logistic Regression** — a baseline linear classifier.
2. **Random Forest Classifier** — an ensemble of decision trees.
3. **Gradient Boosting Classifier** — a boosting-based ensemble method.

## Evaluation approach

The project uses classification metrics such as accuracy, precision, recall, and F1-score. A confusion-matrix heatmap is also used to inspect class-level prediction patterns.

Hyperparameter search is explored with `RandomizedSearchCV` and `GridSearchCV`. The current project notes Gradient Boosting Classifier as the best-performing model in the experiment. Consult the notebook outputs for the exact metric values; no numeric score is stated here without a verified result.

## Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Run locally

Clone this repository:

```bash
git clone https://github.com/BerkayYLMZ53/Airbnb-User-Booking-Prediction-.git
cd Airbnb-User-Booking-Prediction-
```

Install the main dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Launch Jupyter:

```bash
jupyter notebook
```

## Notes

This is an educational prediction exercise using a historical dataset. Model results may not generalize to current Airbnb users or real booking behaviour.
