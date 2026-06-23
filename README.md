# Simple Linear Regression: Student Study Hours vs Marks

## Project Overview

This project demonstrates the implementation of Simple Linear Regression in Python using scikit-learn. The objective is to predict student exam marks based on the number of study hours.

## Dataset

The dataset contains two variables:

* **Hours** (Independent Variable)
* **Marks** (Dependent Variable)

| Hours | Marks |
| ----- | ----- |
| 1     | 45    |
| 2     | 50    |
| 3     | 55    |
| 4     | 60    |
| 5     | 65    |
| 6     | 70    |
| 7     | 75    |
| 8     | 80    |
| 9     | 85    |
| 10    | 90    |

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* Google Colab

## Data Visualization

A scatter plot was created to visualize the relationship between study hours and exam marks.

### Observation

The plot shows a strong positive linear relationship between study hours and marks obtained.

## Model Training

A Simple Linear Regression model was trained using Scikit-Learn.

```python
from sklearn import linear_model

lr = linear_model.LinearRegression()
lr.fit(df[['Hours']], df.Marks)
```

## Model Results

### Coefficient (Slope)

```text
5.0
```

### Intercept

```text
40.0
```

### Regression Equation

Marks = 5 × Hours + 40

## Model Performance

### R² Score

```text
1.0
```

This indicates a perfect linear relationship in the dataset.

## Prediction Example

Prediction for a student studying **9.25 hours**:

```text
86.25 Marks
```

### Calculation

Marks = 5 × 9.25 + 40

Marks = 86.25

## Conclusion

The model successfully learned the relationship between study hours and exam marks. Results indicate that increasing study hours leads to higher exam scores. This project demonstrates the fundamentals of supervised machine learning and simple linear regression.

## Author

Faryad Shah

AI Engineer & Automation Enthusiast

GitHub: https://github.com/faryadshahfs-byte
