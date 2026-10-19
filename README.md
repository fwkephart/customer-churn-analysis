# Customer Churn Analysis

An individual academic project exploring customer churn and comparing
machine learning models to support customer retention decisions.

[View the full analysis](customer-churn-analysis.ipynb)

## Business Question

Which customer characteristics are associated with churn, and how well
can predictive models identify customers at risk of leaving?

## Data

The course-provided dataset contains 6,000 labeled customer records,
including contract details, billing information, service subscriptions,
and engagement measures. Approximately 9.9% of customers churned.

An additional 1,000 unlabeled customer records were provided for
generating prediction probabilities.

## Tools

Python · pandas · NumPy · scikit-learn · XGBoost · Matplotlib · Seaborn

## Approach

- Explored churn patterns across customer characteristics.
- Built preprocessing pipelines for missing values, scaling, and
  categorical encoding.
- Compared logistic regression, decision trees, random forests,
  Extra Trees, gradient boosting, and XGBoost.
- Tested feature engineering and tuned model hyperparameters.
- Generated churn probabilities for the unlabeled customer dataset.

## Key Findings

- Month-to-month customers had a churn rate of approximately 16.0%,
  compared with 2.2% for one-year contracts and 2.8% for two-year contracts.
- Customers who churned had average monthly charges of approximately
  $89.35, compared with $77.32 for customers who stayed.
- The final tuned logistic regression model achieved a mean five-fold
  cross-validation ROC AUC of approximately **0.797**. This ranked in the top 20% of the class in a modeling competition. 

## Business Implications

The observed patterns suggest that high-bill, month-to-month customers
are worth investigating for targeted retention outreach. Potential
actions include plan reviews and testing offers for longer-term contracts.

These associations do not establish why customers leave or demonstrate
that a particular retention offer will work.

## Evaluation Notes

The notebook includes an initial classification exercise and a later
modeling competition focused on ROC AUC. The final 0.797 score comes from
cross-validation used during model and feature selection; it is not an
independent final test score or an accuracy percentage.

## Project Files

- `customer-churn-analysis.ipynb` — Original analysis, saved outputs,
  model comparisons, and prediction workflow.

Running the notebook requires the course-provided files
`customer_retention_training.csv` and `test_features.csv`, along with
the Python packages imported in the notebook.

## Author

Finnian Kephart  
Business Analytics | University of Cincinnati
