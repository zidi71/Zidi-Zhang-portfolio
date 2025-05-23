---
title: "Predictive Analytics for Student Wellbeing — Building a Bullying Risk Model"
categories: ["Data Science in Education"]
excerpt: "Applied machine learning and predictive analytics to identify risk factors and patterns of bullying victimization based on large-scale K-12 survey data."
tags: ["Predictive Analytics", "R", "Machine Learning", "Student Wellbeing", "Data Visualization"]
header:
  image: /assets/images/bullying-model-thumbnail.jpg
  caption: "Applied Machine Learning for K-12 Bullying Risk Assessment"
---

## Overview

Designed and implemented a predictive analytics pipeline to assess student risk of bullying using survey data from over 8,000 K-12 students across multiple Massachusetts school districts.

- Performed **comprehensive data wrangling**: handled missing data via imputation, engineered composite psychosocial features (e.g., perceived school safety, belonging), and prepared high-dimensional datasets for modeling.
- Built, tuned, and evaluated multiple supervised learning models in **R** (including regularized regression, logistic regression, decision trees, and random forests), delivering strong predictive performance for both continuous bullying risk scores and binary high-risk classification.
- Quantified **variable importance** to identify key predictors of victimization, such as perceived discrimination, emotional safety, clarity of school rules, and peer belonging.
- Produced **interpretable risk scores** and actionable insights for school leaders, informing the development of targeted, data-driven prevention and intervention strategies.
- Communicated findings with clear, publication-ready data visualizations and summary reports designed for educators and policy stakeholders.

## Key Highlights

- Constructed and validated indices from 20+ survey items, transforming qualitative responses into meaningful factors for modeling and reporting.
- Achieved robust out-of-sample model accuracy (validation RMSE ≈ 0.39) through rigorous cross-validation and hyperparameter tuning, demonstrating the practical value of predictive analytics for early intervention in student wellbeing.
- Delivered concise policy recommendations for administrators, emphasizing ethical use of predictive models to support at-risk students while mitigating bias and stigmatization.
- Developed an end-to-end data science workflow, from preprocessing and exploratory analysis through interpretability and visualization, enabling reproducibility and scalability for future wellbeing research projects.

---

### Model Performance & Optimization Visualizations

> **Note:** Due to student privacy and data protection requirements, the final report cannot be publicly shared. However, selected visualizations and methodological summaries are available below to illustrate key findings and modeling approaches.
---

#### Regularization Tuning for Regression Model

[View](https://drive.google.com/file/d/1wUadIy3vrIxbBr0AJDjTrTXc_R8dOKbD/view?usp=sharing)

*Figure 1. Cross-validated RMSE as a function of the regularization parameter in penalized regression, illustrating optimal model complexity and generalization trade-offs.*

---

#### Random Forest Hyperparameter Optimization

[View](https://drive.google.com/file/d/1JUuVEYaStLP8A8nAlE5b6MDe1Ly5g_4F/view?usp=sharing)

*Figure 2. Random forest hyperparameter tuning. RMSE trends for training and validation sets guide optimal parameter selection and ensure reliable performance.*

---

#### Variable Importance from Random Forest Model

[View](https://drive.google.com/file/d/1ddDzzgAvZG_mMXbckmkwoUFsU309N1Gm/view?usp=sharing)

*Figure 3. Feature importance from random forest identifies top contributing factors to bullying risk, including reported discrimination, emotional safety, clarity of school rules, and belonging.*

---

## Skills & Tools

- **R** (tidyverse, glm, rpart, randomForest, ggplot2, dplyr, tidyr)
- Data cleaning, feature engineering, missing data imputation
- Predictive modeling: regression, classification, risk scoring
- Cross-validation & hyperparameter optimization
- Data visualization, reporting, interpretability

---

## Impact

- Enabled **early identification of at-risk student groups** to support proactive, equity-oriented wellbeing interventions.
- Provided **actionable, data-driven insights** for educators and administrators, demonstrating real-world impact of advanced analytics in K-12 education.
- Informed ethical considerations around algorithmic bias and stakeholder use of predictive models in sensitive educational contexts.
