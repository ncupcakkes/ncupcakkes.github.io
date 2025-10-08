---
layout: post
title: "Logistic Regression on Titanic Dataset: A Practical Walkthrough"
date: 2024-04-27 10:00 +0000
last_modified_at: 2024-04-27 10:00 +0000
tags: [machine learning, logistic regression, data science, titanic]
toc: true

---

Understanding how logistic regression works in practice is essential for any aspiring data scientist. In this post, we walk through a hands-on project using the Titanic dataset to predict passenger survival.

## Data Preparation

The dataset includes passenger details such as age, class, fare, and family connections. Missing values in the `Age` and `Fare` columns were imputed using group averages based on `Sex` and `Pclass`. This avoids data leakage and ensures the model isn't biased by survival outcomes.

## Feature Engineering

Categorical variables like `Sex` and `Embarked` were converted into numerical dummy variables. A new feature, `FamilySize`, was created by summing `SibSp` and `Parch`, capturing the impact of traveling with family.

## Model Training

A logistic regression model was trained using features such as `Pclass`, `Age`, `Fare`, `FamilySize`, and encoded categorical variables. The dataset was split into training and testing sets to evaluate performance.

## Evaluation

The model achieved an accuracy of approximately 86.7%, with a confusion matrix showing strong predictive power. Feature importance analysis revealed that `Fare`, `Sex_male`, and `Pclass` were among the most influential predictors.

## Final Thoughts

This project demonstrates the importance of thoughtful data preprocessing and feature selection. Logistic regression, while simple, can be powerful when applied correctly. Always validate your model and understand the impact of each feature.

