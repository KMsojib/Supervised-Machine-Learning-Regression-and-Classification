# Multiple Linear Regression with Multiple Features

## Introduction
In the previous week, we learned that regression in one variable, also known as simple linear regression, is a statistical method used to model the relationship between a dependent variable and one independent variable. Now in week 2, we will learn how to perform linear regression with multiple input variables, vectorization, feature scaling, and feature engineering.

## Multiple Features
In the previous week, we used one feature to predict house price, and that feature was its size. However, there are many other features that can impact the price of a house, such as the number of bedrooms, bathrooms, floors, age, etc. We will be incorporating multiple features into a regression model.

To denote the \( i \)-th feature, we use subscripts. Let's take 4 features as an example:
- \( x_1 \) for Bedrooms
- \( x_2 \) for Bathrooms
- \( x_3 \) for Floors
- \( x_4 \) for Age

## Multiple Linear Regression Model
The model with multiple features can be represented as:
\[ \text{Model} = F_{w,b}(X) = w_1 x_1 + w_2 x_2 + w_3 x_3 + w_4 x_4 + b \]

To write a multiple linear regression model, we take a feature vector and a parameter vector and multiply them using the dot product. For example, \( x_1 \) is multiplied with \( w_1 \), and so on.

\[ F_{w,b}(X) = w_1 x_1 + w_2 x_2 + w_3 x_3 + w_4 x_4 + b \]

Here:
- \( W = [w_1, w_2, w_3, \ldots, w_n] \) is the parameter vector (weights).
- \( b \) (bias) is a number.
- \( X = [x_1, x_2, x_3, \ldots, x_n] \) is the input feature vector.

The model can be compactly written using vector notation as:
\[ F_{w,b}(X) = W \cdot X + b = w_1 x_1 + w_2 x_2 + w_3 x_3 + w_4 x_4 + \ldots + w_n x_n + b \]

## Conclusion
Incorporating multiple features into a linear regression model allows us to consider the simultaneous effect of multiple factors on the dependent variable, providing a more comprehensive analysis and prediction. This week, we also covered vectorization, feature scaling, and feature engineering to further enhance our regression models.