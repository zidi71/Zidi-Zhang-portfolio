---
title: "Predictive Analytics for Student Wellbeing — Building a Bullying Risk Model"
categories: ["Data Science in Education"]
excerpt: "Practical application of predictive modeling and machine learning to identify patterns and risk factors of bullying victimization in K-12 student data."
tags: ["Predictive Analytics", "R", "Machine Learning", "Student Wellbeing", "Data Visualization"]
header:
  image: /assets/images/bullying-model-thumbnail.jpg
  caption: "Predictive Modeling for Education"
---

![Bullying Risk Model thumbnail](/assets/images/bullying-model-thumbnail.jpg)

## Overview

- Developed and validated a **predictive analytics workflow** to assess bullying risk among K-12 students using survey and behavioral data.
- Applied **data cleaning, feature engineering, imputation, and aggregation** to transform raw educational survey data for robust analysis.
- Built and tuned multiple regression and classification models (**linear regression, logistic regression, decision trees**) in **R** to predict both bullying frequency and high-risk status.
- Engineered an interpretable pipeline for **variable importance, student risk scoring, and actionable insights** for educators and school leaders.
- Communicated findings with clear impact visualizations and policy recommendations focused on preventative interventions.

**Key Highlights**
- Processed and recoded 20+ survey variables into thematic factors (e.g., school safety, support, social belonging, parental involvement).
- Achieved high accuracy in predicting student bullying risk, identifying key drivers such as perceived physical/emotional safety, school support level, and peer dynamics.
- Designed clear, publication-ready data visualizations (see below) to aid stakeholder understanding and evidence-informed interventions.

---

### Model Performance & Optimization Visualizations

#### Regularization Tuning for Regression Model

![RMSE vs Regularization Parameter](/assets/images/bullying-regularization-rmse.jpg)

*Figure 1. Cross-validated Root Mean Squared Error (RMSE) as a function of the regularization parameter in a penalized regression model. This plot illustrates how appropriately tuning the regularization strength helps control overfitting and improve generalization to new, unseen data. Lower RMSE values indicate better predictive accuracy.*

#### Random Forest Hyperparameter Optimization

![Random Forest Tuning](/assets/images/bullying-rf-rmse.jpg)

*Figure 2. Random Forest hyperparameter tuning results. RMSE trends are shown for both training and validation sets as the number of variables considered at each split (`mtry`) increases. The vertical line marks the optimal `mtry` value selected on the basis of lowest validation RMSE, helping maximize model performance while mitigating overfitting.*

#### Variable Importance from Random Forest Model

![Variable Importance Plot](/assets/images/bullying-feature-importance.jpg)

*Figure 3. Feature importance plot from the optimized random forest model. Higher values on the IncNodePurity axis indicate greater predictive contribution toward bullying risk identification. Key drivers included reported experiences of discrimination (`disc_all`), perceptions of emotional safety (`esafe`), clarity of school rules, and a sense of school belonging. These insights informed targeted recommendations for improving student wellbeing and intervention strategies.*
---

## Skills & Tools

**Tech stack:**  
- R (tidyverse, glm, rpart, ggplot2, dplyr, tidyr)
- Data cleaning, aggregation, and feature engineering  
- Modeling (regression, classification, risk scoring)
- Data visualization & interpretability

---

## Impact
- Provided **data-driven suggestions for early identification and prevention strategies** in student wellbeing and safety.
- Demonstrated **practical value of analytics for education practitioners** seeking to understand at-risk groups and design targeted support.
