🩺 Diabetes Prediction using Decision Tree

This project applies a Decision Tree Classifier to predict diabetes using the Pima Indians Diabetes dataset.
Both Entropy and Gini criteria are used to compare model performance and understand impurity reduction.

🔹 Objective

Predict whether a patient is diabetic or not.

Compare Entropy (Information Gain) and Gini Index.

Identify why Glucose becomes the root node.

🔹 Tools & Libraries

Python, Pandas, NumPy

Matplotlib

Scikit-learn

🔹 Steps Performed

Load and explore the dataset

Select features and target variable

Split data into training and testing sets

Build Decision Tree (Entropy & Gini)

Visualize both trees

Measure accuracy and calculate impurity reduction

🔹 Results
Criterion	Accuracy	Root Node
Entropy	71.8%	Glucose
Gini	71.8%	Glucose

 Both models chose Glucose as the root since it provided maximum impurity reduction.

🔹 Conclusion

Both Entropy and Gini criteria gave similar accuracy and structure.

Glucose is the most significant predictor of diabetes.

Decision Trees provide interpretable and effective classification results.
