📘 Practical 9 – K-Nearest Neighbors (KNN) Classification on the Iris Dataset

This practical focuses on applying the K-Nearest Neighbors (KNN) algorithm to classify flower species in the well-known Iris dataset.
It includes data preprocessing, exploratory analysis, feature scaling, model training, performance evaluation, and selecting the optimal K value.

1. Importing Required Libraries

pandas – data handling

numpy – numerical operations

scikit-learn – dataset loading, scaling, model creation, evaluation

matplotlib – plotting and visualization

2. Loading the Iris Dataset

Load built-in Iris dataset using load_iris()

Convert it into a pandas DataFrame

Add target labels: setosa, versicolor, and virginica

3. Exploratory Data Analysis (EDA)

Display the first few rows with head()

Generate summary statistics using describe()

Compute mean values for each species using groupby()

4. Feature Scaling

Apply StandardScaler() to standardize the features

Fit and transform the numeric data for better KNN performance

5. Train–Test Split

Split the dataset into 80% training and 20% testing using train_test_split()

6. Training the KNN Model

Create a KNN model using KNeighborsClassifier()

Train the model on the scaled training data

Predict species for the test data

7. Model Evaluation

Generate a Confusion Matrix

Calculate Accuracy Score

Print the Classification Report (Precision, Recall, F1-score)

8. Finding the Best K Value

Test K values from 1 to 20

Calculate error rate for each K

Select the K with the minimum error rate

9. Error Rate Plot

Plot K values vs. error rate

Visualize how accuracy changes with different K values

Helps determine the optimal K

10. Visualizing the KNN Decision Boundary (2D)

Encode categorical labels

Train a 2D KNN classifier using selected feature pairs

Plot the decision boundaries to understand classification regions
