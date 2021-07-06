---
title: Predicting Clearance Rates of Serious Crimes
---

# Predicting Crime Clearance

([Annotated Jupyter Notebook](https://nbviewer.jupyter.org/github/alexmjn/Predicting-Arrests/blob/master/Crime_Data.ipynb) with all code from this analysis.)

## Motivation

The goal of this project was to apply predictive modeling to a real-world problem; in this case,
predicting whether or not a given crime would be cleared by police. In a real-world scenario, insights from this analysis could be used to suggest efficient, cost-effective interventions.

## Summary

I used data from The Trace on 747,000 criminal incidents to investigate what factors were associated with clearance rate. I cleaned the
messy data set, explored its characteristics, and used that information to guide modeling decisions including
feature selection and feature engineering. Finally, I tested a variety of predictive modeling techniques to
maximize accuracy in predicting whether a crime would be cleared.

## Analysis

I found that the two biggest factors in prediction were whether a crime involved firearms and what city the crime occurred in.
Gun crime is dramatically less likely to be cleared. And, even controlling for higher rates of gun crime, struggling cities seem to suffer both from a high rate of crime and a low rate of clearing each individual crime.
[I wrote up analysis in more detail here.](https://medium.com/@ajenkneary/clearing-out-crime-4b1267f7274d).

## Technical Overview

I used `pandas` extensively to clean the data. This was a challenging data cleanup, as the data sets were not standardized and filled with missing variables and partially-matching strings.

I used `matplotlib` and `seaborn` to visualize and explore my data, both to guide modeling decisions and to fully understand its contours.

I then set up `scikit-learn` pipelines with encoders, imputers, and a variety of models and did hyperparameter tuning with sklearn's cross-validated randomized search. I did this in conjunction with feature selection and engineering (guided by eli5 and the weights from sklearn) in order to find the best model.

Analysis can be replicated using the data in [the repo](https://github.com/alexmjn/Predicting-Arrests).
