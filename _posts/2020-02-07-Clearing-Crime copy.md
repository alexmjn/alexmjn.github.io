---
title: Predicting Clearance Rates of Serious Crimes
---

# Predicting Clearance Rates

## Goals

The goal of this project was to apply predictive modeling to a real-world problem; in this case,
predicting whether or not a given crime would be cleared by police.

## Summary

I used data from The Trace on 747,000 criminal incidents to investigate what factors were associated clearance rate. I cleaned the
messy data set, explored its characteristics, and used that information to guide modeling decisions including
feature selection and feature engineering. Finally, I tested a variety of predictive modeling techniques to
maximize accuracy in predicting whether a crime would be cleared.

## Analysis

I found that the two biggest factors in prediction were whether a crime involved firearms and what city the crime occurred in.
Gun crime is dramatically less likely to be cleared. And, even controlling for higher rates of gun crime, struggling cities seem to suffer both from a high rate of crime and a low rate of clearing each individual crime.
[I wrote up analysis in more detail here.](https://medium.com/@ajenkneary/clearing-out-crime-4b1267f7274d).

## Code

Code, analysis, and commentary can be found in [This Jupyter Notebook](https://github.com/alexmjn/Predicting-Arrests/blob/master/Crime_Data.ipynb).
Analysis can be replicated using the data in [the repo](https://github.com/alexmjn/Predicting-Arrests).
