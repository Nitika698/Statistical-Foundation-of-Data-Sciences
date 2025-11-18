📘 Practical 9 – K-Nearest Neighbors (KNN) Classification on Iris Dataset

This practical demonstrates how to perform classification using the K-Nearest Neighbors (KNN) algorithm on the popular Iris dataset.
It covers data preprocessing, exploratory data analysis, scaling, model training, evaluation, and finding the best K value.


1. Importing Required Libraries

pandas

numpy

scikit-learn (datasets, scaling, model_selection, neighbors, metrics)

matplotlib (for visualization)

2. Loading the Iris Dataset

Load dataset using load_iris()

Convert to pandas DataFrame

Add target labels (setosa, versicolor, virginica)

3. Exploratory Data Analysis (EDA)

Display first 5 rows using head()

Summary statistics using describe()

Grouping by species to compute mean values

4. Feature Scaling

Use StandardScaler() to normalize features

Fit and transform the dataset for efficient KNN performance

5. Train-Test Split

Split dataset into 80% training and 20% testing using train_test_split()

6. Training the KNN Model

Build KNN classifier using KNeighborsClassifier()

Fit the model on training data

Predict results on test data

7. Evaluating the Model

Confusion Matrix

Accuracy Score

Classification Report (Precision, Recall, F1-score)

8. Finding the Best K Value

Loop through K values from 1 to 20

Calculate error rate for each K

Identify the value of K with the lowest error

9. Error Rate Plot

Visualize how the error rate changes with K

Helps in selecting the optimal K value

10. Visualizing KNN Decision Boundary (2D)

Encode labels

Train a 2D KNN classifier (using selected features)

Plot the decision regions (if implemented in your final cells)
