 # Sport Outcome Prediction

## Overview

Sport Outcome Prediction is a machine learning project that investigates how well match outcomes can be predicted using only publicly available data. It covers two sports: football (Top 5 European leagues, three possible outcomes) and basketball (NBA, two possible outcomes). For each sport, the project walks through the full pipeline: data collection and cleaning, feature engineering (ELO ratings, form and momentum, home advantage, betting odds), model training, and evaluation.

Three models of increasing complexity are compared: Logistic Regression, Random Forest and XGBoost. They are evaluated using accuracy, F1 score, ROC-AUC and log loss, with SHAP used to interpret which features drive the predictions. Multiple datasets per sport make it possible to measure the effect of betting odds and of the number of seasons on model performance.

Designed with scalability in mind, this repository provides a foundation for future improvements.

## Tech Stack

This project was built using the following tools:

* Language: [Python](https://www.python.org/)
* Data processing: [pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/)
* Machine learning: [scikit-learn](https://scikit-learn.org/), [XGBoost](https://xgboost.readthedocs.io/)
* Interpretability: [SHAP](https://shap.readthedocs.io/)
* Visualization: [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/)
* Environment: [Jupyter](https://jupyter.org/), [Conda](https://docs.conda.io/)

## Getting Started

Create the environment, install dependencies and open the notebooks in order:

```
conda create -n sportbet python=3.11
conda activate sportbet
pip install -r requirements.txt
```

Raw data is not included in the repository. The data collection notebooks download it from public sources.

---
*This project was developed as a master's thesis at the Faculty of Electrical Engineering, Mechanical Engineering and Naval Architecture (FESB), University of Split.*
