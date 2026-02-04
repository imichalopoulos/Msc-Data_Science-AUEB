# Ioannis Michalopoulos - MSc Data Science, Athens University Of Economics And Business Department of Informatics
# Advanced Customer Analytics – Explainability & Counterfactuals

This repository contains a Jupyter Notebook developed as part of the **Advanced Customer Analytics** course for the **MSc in Data Science**.  
The notebook demonstrates how to build a binary classification model and how to interpret its predictions using **model explainability** and **counterfactual analysis** techniques.

The project uses a real-world movie recommendation context to illustrate how explainability tools can be applied to customer-related decision systems.

---

## Learning Objectives

By working through this notebook, students will:

- Understand how to preprocess and engineer features from a real-world dataset
- Train a **binary classification model** for customer preference prediction
- Apply **local explainability techniques** to interpret individual predictions
- Generate and analyze **counterfactual explanations**
- Gain intuition on how explainability supports transparency and trust in ML systems

---

## Dataset

The analysis is based on **The Movies Dataset**, which includes metadata about movies such as:

- Genres  
- Runtime  
- Language  
- Release decade  
- User ratings and reviews  

The dataset is publicly available on Kaggle:  
*The Movies Dataset* – Rounak Banik

---

## Notebook Structure

The notebook is organized as follows:

1. **Data Loading**  
   Importing and inspecting the movie metadata and user ratings.

2. **Preprocessing & Exploratory Data Analysis (EDA)**  
   - Genre encoding  
   - Runtime bucketing  
   - Language categorization (English vs Non-English)  
   - Decade-based grouping  
   - Feature selection  

3. **Label Construction**  
   - Aggregation of user reviews  
   - Conversion of ratings into a binary target variable  

4. **Binary Classification Model**  
   - Preparation of model inputs  
   - Model training  
   - Performance evaluation (confusion matrix and metrics)

5. **Explainability**  
   - Local explanations using **LIME**
   - Interpretation of feature contributions for individual predictions

6. **Counterfactual Analysis**  
   - Generation of counterfactual examples using **DiCE**
   - Exploration of minimal feature changes required to flip a prediction

7. **Final Function**  
   - End-to-end function combining prediction, explanation, and counterfactual generation for a given movie profile

---

## Explainability & Counterfactuals

This notebook introduces two key interpretability concepts:

- **Explainability (LIME)**  
  Helps answer *“Why did the model make this prediction?”* by identifying influential features.

- **Counterfactuals (DiCE)**  
  Helps answer *“What would need to change for the prediction to be different?”*, offering actionable insights.

These techniques are particularly relevant in customer analytics, recommender systems, and decision-support applications.

---

## Requirements

To run the notebook, you will need:

- Python 3.x
- Jupyter Notebook or JupyterLab
- Common data science libraries:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - lime
  - dice-ml

Install dependencies with:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn lime dice-ml
