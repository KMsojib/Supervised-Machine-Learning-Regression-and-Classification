# Logistic Regression in Machine Learning

## Logistic Regression

Logistic regression is a supervised machine learning algorithm primarily used for binary classification tasks. It predicts the probability that an instance belongs to a particular class. By employing the sigmoid function, logistic regression converts the input of independent variables into a probability value between 0 and 1.

### The Logistic Regression as follows:
* If the sigmoid function's output is greater than 0.5, the instance is classified as class 1.
* If the output is less than or equal to 0.5, the instance is classified as class 0.

Logistic regression is fundamentally used for classification problems, distinguishing it from linear regression.

### Key Points:
1. **Classification Algorithms:** Logistic Regression (LR) is primarily used for binary classification tasks.
2. **Probability Prediction:** It predicts the probability that an instance belongs to a particular class.
3. **Sigmoid Function:** The sigmoid function is used to convert the input of independent variables into a probability value between 0 and 1.
4. **Threshold Value:** A threshold value (commonly 0.5) is used to determine the class of the instance. If the probability is greater than the threshold, the instance is classified as one class; otherwise, it is classified as the other class.
5. **Extension of Linear Regression:** Logistic regression is an extension of linear regression but is mainly used for classification problems, not regression.

## Types of Logistic Regression

There are different types of logistic regression. The main types of logistic regression are:
1. Binary Logistic Regression
2. Multinomial Logistic Regression
3. Ordinal Logistic Regression

### 1. Binary Logistic Regression

Binary logistic regression is used when the dependent variable has only two possible outcomes.
e.g., Yes/No, 0/1, Good/Bad, Success/Failure, etc. It is mostly used in logistic regression.

**Example:**
* Predicting whether an email is spam or not.
* Classifying a tumor as malignant or benign.

### 2. Multinomial Logistic Regression

Multinomial logistic regression is used when the dependent variable can have three or more unordered categories. Unlike binary logistic regression, there is no natural ordering of the categories.

**Example:**
* Classifying types of fruits (e.g., apple, orange, banana).
* Predicting the choice of transportation (e.g., car, bus, train).

### 3. Ordinal Logistic Regression

Ordinal logistic regression is used when the dependent variable has three or more ordered categories. In this type, the order of the categories is significant.

**Example:**
* Rating a product (e.g., poor, fair, good, excellent).
* Classifying levels of education (e.g., high school, bachelor's, master's, doctorate).

## Mathematical Foundation

### Logistic Function (Sigmoid Function)

It is a mathematical function that maps any real-valued number into a value between 0 and 1. Its characteristic “S”-shaped curve makes it particularly useful in scenarios where we need to convert outputs into probabilities.

Mathematically, the sigmoid is represented as:
	σ(x) = 1 / (1 + e^(-x))

Where, 
	* σ is the sigmoid function
	* x is the input value
	* e is Euler's number (≈2.718)

### Logit Function

The logit function is the inverse of the sigmoid function and is used to model the relationship between the dependent binary variable and one or more independent variables. It is defined as the natural logarithm (log) of the odds of the dependent event occurring.

Mathematically, the logit function is represented as:

logit(p) = log(p / (1 - p))

Where:
* \(p\) is the probability of the event occurring
* \(\ln\) is the natural logarithm
* * p / (1-p) = corresponding odds

## Logistic Regression Model

The logistic regression model is built on the logistic function. The logistic regression equation can be written as:


Where:
* \(p\) is the probability of the event occurring
* \(\beta_0\) is the intercept term
* \(\beta_1, \beta_2, \ldots, \beta_k\) are the coefficients of the independent variables \(x_1, x_2, \ldots, x_k\)

The probability \(p\) can be derived from the logit function as:
\[ p = \frac{1}{1 + e^{-(\beta_0 + \beta_1x_1 + \beta_2x_2 + \ldots + \beta_kx_k)}} \]

### Model Training

To train a logistic regression model, we use a dataset with known outcomes (labels). The model learns the coefficients (\(\beta\)) that best fit the data by maximizing the likelihood of the observed outcomes. This process is called Maximum Likelihood Estimation (MLE).

### Model Evaluation

Once the model is trained, it can be evaluated using various metrics such as accuracy, precision, recall, F1-score, and the Area Under the Receiver Operating Characteristic Curve (AUC-ROC).

**Example Metrics:**
* **Accuracy:** The ratio of correctly predicted instances to the total instances.
* **Precision:** The ratio of correctly predicted positive instances to the total predicted positive instances.
* **Recall:** The ratio of correctly predicted positive instances to the total actual positive instances.
* **F1-Score:** The harmonic mean of precision and recall.
* **AUC-ROC:** A curve that plots the true positive rate against the false positive rate, providing a single measure of overall performance.

## Conclusion

Logistic regression is a powerful and widely-used algorithm for binary classification tasks. Its ability to predict probabilities and handle different types of classification problems makes it a valuable tool in the machine learning toolkit. By understanding the mathematical foundation and key concepts behind logistic regression, practitioners can effectively apply this algorithm to a variety of real-world problems.
```` ▋
