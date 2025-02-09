 **ASSIGNMENT - 2 : LOGISTIC REGRESSION** 

-----------------------------------------------------------------------------------------------------------------------------------------------------------

**NAME : SAYANTAN CHAUDHURI**

**ROLL NO.: 2206211**

**SECTION : IT01**

-----------------------------------------------------------------------------------------------------------------------------------------------------------
> **QUESTION**

In this assignment, you need to classify the given dataset using
logistic regression.

> Datasets:
- Independent/Predictor Variable - `logisticX.csv`
- Dependent/Response Variable -`logisticY.csv`

Use the same cost function that we had discussed in class.

> **Answer the following questions based on your observations**

- 1. Use logistic regression to find decision boundary For the
given database. Set your learning rate to 0.1. What is the
cost function value and learning parameter value after
convergence?
- 2. Plot cost function v/s iteration graph for the model trained
in question 1. Plot the line as shown here -
https://pythonguides.com/matplotlib-plot-a-line/#Matplotlib_pl
ot_a_line_chart
Do not use scatter plots for this.
- 3. Plot the given dataset on a graph, use different colours for
different classes and also show the decision boundary you
obtained in question 1. Do not use scatter plot.
- 4. Train your model with a learning rate of 0.1 and 5. Plot the
cost-function v/s iteration curve for both learning rates on
the same graph. For this task, only train your model for 100
iterations.
- 5. Find the confusion matrix for your training dataset. Using the
confusion matrix to calculate the accuracy, precision, recall,
F1-score.

> **Process Overview**

- 1. Import Dependencies

The code utilizes numpy, pandas, and matplotlib.pyplot for numerical operations, data handling, and visualization.
The train_test_split function from sklearn.model_selection is used for data splitting.

- 2. Load and Preprocess Data

Reads `logisticX.csv` and `logisticY.csv` into pandas DataFrames.
Performs standardization by subtracting the mean and dividing by the standard deviation.
Splits the dataset into training and testing sets (80%-20%).
Implement Logistic Regression (Gradient Descent)

- 3. Defines a GDs class that:

Initializes parameters (w for weights, b for bias).
Implements the sigmoid activation function.
Optimizes parameters using gradient descent over a set number of epochs.

- 4. Train the Model

Calls fit(X, Y) on the training data to iteratively update weights and minimize cost.

- 5. Evaluate Performance

Predicts values on test data and assesses accuracy.
