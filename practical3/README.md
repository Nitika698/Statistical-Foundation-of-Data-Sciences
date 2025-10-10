Practical 3 – Statistical Relationships and Data Visualization

This practical focuses on data summarization, duplicate handling, and visual exploration using Python libraries — pandas, matplotlib, and seaborn.
The objective is to study how instructor characteristics such as age, gender, and course division relate to their teaching evaluations.

📘 Questions Overview
Q1. Identifying Duplicates and Computing Summary Statistics

Checked for duplicate entries using the prof column.

Calculated the mean and standard deviation of age using all records.

Filtered the dataset to retain only one record per professor (n = 94) and recalculated the summary statistics.

Compared how removing duplicates impacted the averages.

Key Insight:
Eliminating duplicate entries slightly adjusted the mean and standard deviation, minimizing bias and producing a more accurate summary.

Q2. Teaching Evaluations by Course Division

Created a bar chart comparing the average evaluation scores between lower and upper division courses.

Course Division	Average Evaluation
Lower	4.35
Upper	3.75

Interpretation:
Professors teaching lower-division courses tend to receive slightly higher average evaluations compared to those teaching upper-division courses.

Q3. Relationship Between Age and Teaching Evaluation

Used a regression plot (seaborn.regplot) to explore how teaching evaluations vary with age.

Observed a negative correlation, suggesting that evaluation scores tend to decrease slightly as age increases.

Q4. Gender-Differentiated Scatter Plot

Plotted Age vs Evaluation separately for male and female instructors.

Used distinct colors and markers to highlight gender-based differences.

Observation:
Female instructors appeared to have marginally higher evaluation scores in the simulated dataset, although the difference is minor and may depend on sample size.

Q5. Combined Regression Analysis by Gender

Applied sns.lmplot() to visualize age vs evaluation with separate regression lines for each gender.

Highlighted how linear relationships differ between male and female instructors.

🧰 Libraries Used

pandas — for data cleaning and manipulation

matplotlib — for basic plotting and visualization

seaborn — for advanced statistical visualizations

🧠 Key Insights

Duplicate handling can significantly influence statistical outcomes.

Younger instructors generally receive slightly higher evaluation scores.

Course level and gender may also affect teaching evaluations.

Visualization techniques help uncover meaningful trends and correlations in data.
