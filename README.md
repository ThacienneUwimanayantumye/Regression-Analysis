# Health Data Regression Analysis

This repository contains a comprehensive analysis of health-related data using linear and logistic regression models. The project investigates the relationships between key health indicators and outcomes, such as high blood pressure (HBP) and coronary heart disease (CHD).

## Purpose of the Analysis

The primary objectives of this analysis are:
1. To explore the relationship between various health-related predictors (e.g., cholesterol, cigarette consumption, weight) and health outcomes (e.g., HBP, CHD).
2. To identify the most significant factors influencing these outcomes.
3. To build predictive models for health outcomes using regression techniques.

## Dataset and V variables

Data from the Framingham Heart study. In 1948, the study was initiated to identify the common
factors or characteristics that contribute to CVD by following its development over time in a group
of participants who had not yet developed overt symptoms of CVD or suffered a heart attack or
stroke. The researchers recruited 5,209 men and women between the ages of 30 and 62 from the
town of Framingham, Massachusetts. Every two years, a series of extensive physical examinations
and lifestyle interviews were conducted. This data set is a subset of the Framingham Heart study
data. The data is stored as 14 columns (variables) and 1394 rows (observations). Each row represents a single subject.
The key variables analyzed include:
- **sCHOL**: Cholesterol levels (standardized).
- **sCIG**: Number of cigarettes smoked daily (standardized).
- **sFRW**: Weight (standardized).
- **sAGE**: Age (standardized).
- **SEX**: Gender (categorical).
- **HIGH_BP**: Binary variable indicating high blood pressure.
- **hasCHD**: Binary variable indicating coronary heart disease.

## Methods

The following methods were employed in the analysis:
1. **Exploratory Data Analysis (EDA)**:
   - Examined distributions, relationships, and potential multicollinearity between variables.
2. **Linear Regression**:
   - Modeled continuous outcomes using predictors such as weight and age.
3. **Logistic Regression**:
   - Modeled binary outcomes (e.g., HIGH_BP and hasCHD) using predictors and interaction terms.
4. **Cross-Validation**:
   - Evaluated model performance using 100-fold cross-validation to ensure robustness.
5. **Visualization**:
   - Plotted scatter plots, logistic curves, and residuals to validate model assumptions and interpret findings.
## Key Conclusions

1. **High Blood Pressure (HBP)**:
   - Significant predictors include weight (`sFRW`), age (`sAGE`), and interactions between these variables.
   - Older individuals with higher weight were more likely to have high blood pressure.

2. **Coronary Heart Disease (CHD)**:
   - Cigarette consumption (`sCIG`) was identified as the most significant predictor of CHD.
   - Interaction terms (e.g., `sCHOL:sCIG`) further highlighted complex relationships between smoking, cholesterol, and CHD risk.

3. **Model Performance**:
   - Logistic regression models showed high accuracy, with cross-validation results indicating stable and reliable predictions.
   - The analysis demonstrated the importance of including interaction terms to capture nuanced effects.

## Repository Structure

- **Data**: Contains the dataset used for analysis.
- **Notebook**: The Jupyter Notebook documenting the entire analysis (`Regression_analysis_Linear_and_logistic_on_health_data.ipynb`).
- **Figures**: Visualizations generated during the analysis.
- **Scripts**: Python scripts for regression modeling and cross-validation.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/ThacienneUwimanayantumye/Regression-Analysis-of-health-data.git
