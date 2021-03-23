---
title: Exploratory Data Analysis - NBA Injuries
subtitle: Exploring NBA injuries and rest, 2010-2018
---

# Exploratory Data Analysis: NBA Injuries

## Summary

This project was a demonstration of the analysis that can be done using just exploration
and visualization of data without predictive modeling. I took a messy list of 2010-2018 NBA injury
reports from Kaggle, cleaned the data, and analyzed patterns across teams, across injury categories,
and through the time period in question.

## Analysis

A writeup of what I found can be seen in [my Medium article](https://medium.com/@ajenkneary/injuries-and-rest-in-the-nba-2c39a8bd261c).
Some nuggets for those interested:

* Players missed more than twice as many days with left ankle sprains as right.
* Players were injured 22% more frequently in the lockout-shortened 2012 season.
* Injury rates increase monotonically until the All-Star break. The break resets injury rates, but from there they increase around twice as quickly until the end of the season.
* The San Antonio Spurs rested players more than twice as frequently as the next-highest team.

## Code

The analysis and fully annotated code, along with commentary, can be found in [this Jupyter notebook](https://github.com/alexmjn/NBA-Injuries/blob/master/NBA_Injuries.ipynb).
Data can be found in [the associated repo](https://github.com/alexmjn/NBA-Injuries). Analysis and visualization was done using `numpy`, `pandas`, `matplotlib`, `seaborn`, and `scipy`.
