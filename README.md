# Startup Classifier

> Code and documentation for the startup classifier for Viktor Kozhuharov's internship in Vela Partners.

---

## Description

A startup classifier that decides whether a given startups will be successful. Uses two datasets of successful and unsuccessful companies that Vela Partners have provided.

---

## Methodology

The model uses logistic regression. K-nearest neighbours and random forests were also tested but performed worse. The data we use excludes any startups for which there is no information from a certain sheet in the dataset. The features *'name'* and *'country_code'* are removed because they are irrelevent ('country_code' is always USA). *'founded_year'* is also excluded, as it is very hard to extrapolate patterns about specific past years to the current year. A new feature 'number_of_founders' is added.
Other than being able to predict a startup's success, the model also output a sorted list of features by importance. 