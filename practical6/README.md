# Teaching Evaluation Analysis

## Overview
This Jupyter Notebook analyzes a Teaching Quality Evaluation dataset to answer key questions related to professor demographics, tenure status, and evaluation scores. The dataset includes information on professor age, gender, minority status, teaching tenure, and evaluation ratings.

The analysis covers probability calculations, summary statistics, visualizations, and median score computations. It is designed to demonstrate the application of basic statistical techniques and Python visualization tools in an educational setting.

---

## Dataset
The dataset contains the following relevant columns:

- `eval` : Teacher evaluation score (numeric)
- `age` : Age of the professor
- `tenure` : Tenure status (Yes/No)
- `minority` : Whether the professor is a visible minority (Yes/No)
- `gender` : Gender of the professor
- `students` / `allstudents` : Optional, number of students per professor
- `prof` : Optional, professor identifier

**Number of entries:** Varies depending on dataset version.  
**Format:** CSV file (`ratings.csv` or `TeachingRatings.csv`).

---

## Analysis Tasks

1. **Percentage of visible minorities who are tenured**  
   - Calculates the proportion of minority professors holding tenure.  
   - Provides insight into whether tenure status differs based on minority status.

2. **Average age by tenure**  
   - Computes the mean and standard deviation of age for tenured and non-tenured professors.  
   - Helps understand whether tenure correlates with age.

3. **Probability of receiving certain evaluation scores**  
   - Calculates the probability of evaluation scores above 4.5.  
   - Calculates the probability of evaluation scores between 3.5 and 4.2.

4. **Two-tailed test using evaluation scores**  
   - Performs a z-test to compare sample mean with a historic or benchmark mean.  
   - States null and alternative hypotheses and interprets results.

5. **Gender distribution and plotting**  
   - Explains the difference between `pyplot.bar` and `pyplot.barh`.  
   - Visualizes the distribution of male and female professors.

6. **Median evaluation score for tenured professors**  
   - Computes median to understand central tendency among tenured faculty.

---

## Libraries Used
- `pandas` : Data manipulation and analysis
- `numpy` : Numerical operations
- `matplotlib` : Plotting graphs
- `seaborn` : Enhanced visualization styling
- `scipy.stats` : Statistical computations (z-test, probability calculations)

---

## How to Use
1. Open the `TeachingEvaluationAnalysis.ipynb` notebook in Jupyter.  
2. Ensure the dataset CSV file (`ratings.csv`) is in the same folder.  
3. Run each cell sequentially to view outputs, plots, and calculations.

---

## Notes
- The notebook is written in a human, natural style with step-by-step explanations.  
- Columns like `age`, `tenure`, `minority`, `gender`, and `eval` are essential for the main analysis.  
- Other columns (`students`, `allstudents`, `prof`) are optional and may be used for extra insights.  
- All results are reproducible using the provided dataset.
