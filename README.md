# Simple Linear Regression: Student Study Hours vs Marks

## Project Overview
This project demonstrates a production-ready, hands-on implementation of a Simple Linear Regression model using Python and Scikit-Learn. The objective is to predict a student's expected marks based on the total number of study hours. 

## Dataset
The dataset contains two continuous variables mapping student performance:
* **Hours (Independent Variable / $X$):** The number of hours spent studying.
* **Marks (Dependent Variable / $y$):** The percentage marks obtained.

| Hours ($X$) | Marks ($y$) |
| :--- | :--- |
| 1 | 45 |
| 2 | 50 |
| 3 | 55 |
| 4 | 60 |
| 5 | 65 |
| 6 | 70 |
| 7 | 75 |
| 8 | 80 |
| 9 | 85 |
| 10 | 90 |

## Technologies Used
* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Scikit-Learn**

## Data Visualization
A linear relationship can be visualized via a scatter plot mapping Hours against Marks. The data shows a perfectly positive linear correlation.

*(Note: Save your generated graph plot as `hours_vs_marks.png` in your repository root and uncomment the line below)*
<!-- ![Hours vs Marks Graph](hours_vs_marks.png) -->

## Model Training & Execution
The model is constructed using Scikit-Learn's `linear_model.LinearRegression`.

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from sklearn import linear_model

# 1. Load Dataset
df = pd.read_csv('student_study_hours.csv')

# 2. Train Linear Regression Model
lr = linear_model.LinearRegression()
lr.fit(df[['Hours']], df.Marks)
