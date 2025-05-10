# Heart Disease Prediction using Logistic Regression

This project explores the relationship between maximum heart rate and heart disease using the **Cleveland Heart Disease dataset**. Through a combination of statistical tests and logistic regression, I identify key predictors of heart disease and build a simple, interpretable model to predict its presence.

---

## Project Structure

- `Cleveland_hd.csv`: The dataset used in the analysis
- `notebook.ipynb`: Jupyter Notebook containing the entire analysis
- `README.md`: Project overview and results summary

---

## 📊 Dataset Summary

The dataset contains medical records of patients, including:
- Demographics (age, sex)
- Clinical features (blood pressure, cholesterol, ECG results)
- Exercise results (maximum heart rate, angina)
- Diagnosis (`class`: 0 = no disease, 1–4 = increasing severity)

I converted the `class` column into a binary variable:
- `0`: No heart disease
- `1`: Presence of heart disease

---

## Feature Selection

Two types of statistical tests were applied:

- **T-test**: For continuous features to detect mean differences between classes
- **Chi-square test**: For categorical features to assess the independence with the target

### Top 3 Statistically Significant Features:
- `thal`: Thalassemia (categorical)
- `cp`: Chest pain type (categorical)
- `thalach`: Maximum heart rate achieved (continuous)

---

## Model Used: Logistic Regression

I trained a logistic regression model using the three selected features. This approach was chosen for its simplicity and interpretability.

### Model Performance:

| Metric       | Value    |
|--------------|----------|
| Accuracy     | 82.42%   |
| Precision    | 78.72%   |
| Recall       | 86.05%   |
| F1 Score     | 82.22%   |

## Project Availability

This project is present in [DataCamp Projects](https://projects.datacamp.com/projects/2077).


While the DataCamp version guides users through the project in R, I independently implemented the entire workflow in Python, from data analysis to model evaluation.