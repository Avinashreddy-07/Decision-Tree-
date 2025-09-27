# Decision-Tree-
Decision Tree Classifier on Iris Dataset

Author: Avinash k 700771195

Project Overview

This project demonstrates the use of Decision Trees for classification using the Iris dataset.
We train models with different max_depth values (1, 2, 3) and compare their performance on both training and testing sets.
The goal is to understand underfitting and overfitting in decision trees.

Technologies Used

Python 3

scikit-learn

pandas

numpy

Dataset

Iris Dataset (available in scikit-learn)

150 samples, 4 features: sepal length, sepal width, petal length, petal width

3 classes: Setosa, Versicolor, Virginica

Steps Performed

Loaded the Iris dataset using load_iris().

Split the data into training (80%) and testing (20%) sets with train_test_split.

Trained DecisionTreeClassifier with max_depth values 1, 2, and 3.

Predicted on training and testing data, calculated accuracy.

Stored results in a pandas DataFrame and compared the performance.

Results
Max Depth	Train Accuracy	Test Accuracy
1	0.666667	0.666667
2	0.966667	0.933333
3	0.983333	0.966667
Observations

Depth = 1: Too simple → Underfitting, low accuracy on both train & test.

Depth = 2: Balanced performance, captures key patterns, good generalization.

Depth = 3: High training and testing accuracy, still generalizes well.

Increasing depth beyond this can lead to overfitting (model memorizes training data).
