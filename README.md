# Viniculture: Wine Quality Analysis

A detailed exploratory data analysis and modeling initiative examining factors that influence wine quality. Leveraging the `Viniculture.ipynb` notebook, this repository analyzes physicochemical properties of red and white wines and builds predictive models to estimate quality ratings.

---
![image](https://github.com/user-attachments/assets/2fee9ac9-dcf5-4e15-aa31-8252d794ebbb)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
4. [Feature Engineering](#feature-engineering)
5. [Modeling & Evaluation](#modeling--evaluation)
6. [Notebook](#notebook)
7. [Installation & Usage](#installation--usage)
8. [Dependencies](#dependencies)
9. [Future Work](#future-work)
10. [License](#license)

---

## Project Overview
Analyze the **Wine Quality** dataset to:
- Conduct EDA on red and white wine samples
- Visualize relationships between chemical properties and quality scores
- Engineer and select features for improved model performance
- Train and evaluate classification and regression algorithms for quality prediction

Insights guide winemakers and consumers by highlighting key quality determinants.

## Dataset
- **Source:** UCI Machine Learning Repository
- **Files:**
  - `winequality-red.csv`
  - `winequality-white.csv`
- **Features:** 11 physicochemical attributes (e.g., `fixed acidity`, `pH`, `alcohol`) and quality score (0–10)

## Exploratory Data Analysis
- Compare quality score distributions for red vs. white wines
- Generate correlation heatmaps to identify significant feature interactions
- Use scatter plots and boxplots to detect outliers and examine feature distributions

## Feature Engineering
- Combine red and white datasets with a source indicator
- Bin quality scores into categorical labels (low, medium, high)
- Scale and normalize continuous variables
- Create interaction terms where statistical analysis indicates potential synergy

## Modeling & Evaluation
- **Algorithms:** Logistic Regression, Random Forest, Gradient Boosting, Elastic Net Regression
- **Performance Metrics:**
  - Classification: Accuracy, F1-score, ROC AUC
  - Regression: R<sup>2</sup>, RMSE
- **Validation Strategy:** Stratified k-fold cross-validation for classification; k-fold for regression

## Notebook
All code and analysis reside in `Viniculture.ipynb`, organized into:
1. Data Loading & Cleaning
2. Exploratory Data Analysis
3. Feature Engineering
4. Model Training & Hyperparameter Tuning
5. Model Evaluation & Visualization

## Installation & Usage
```bash
# Clone the repository
git clone https://github.com/akhilesh360/Viniculture.git
cd Viniculture

# Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Lab
jupyter lab
````

## Dependencies

* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn
* jupyterlab

Refer to `requirements.txt` for version details.

## Future Work

* Integrate ensemble and gradient-boosting frameworks (e.g., XGBoost, LightGBM)
* Develop an interactive dashboard for real-time quality prediction
* Incorporate additional metadata (vineyard region, vintage year)

## License

Licensed under the MIT License. See the `LICENSE` file for details.

```
```
