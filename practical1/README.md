# Practical 1: Statistical Foundation of Data Sciences

**Subject Name:** Statistical Foundation of Data Sciences  
**Subject Code:** CSU1658 Practical  

---

## 📖 Description
This folder contains the Jupyter notebook **Practical-1.ipynb** for Practical 1 of the subject *Statistical Foundation of Data Sciences*.  
The notebook demonstrates the creation and analysis of a synthetic dataset (including *NaN values*), along with various statistical computations, standardization techniques, and array operations using NumPy and Pandas.  

---

## 🎯 Instructions
- Work in either **Google Colab** or **Jupyter Notebook**.  
- Generate a synthetic dataset with some **NaN values**.  
- Use a **random seed = 42** for reproducibility (modify if needed for different scenarios).  

---

## 📝 Objectives
- Apply fundamental statistical concepts through hands-on coding.  
- Handle missing data effectively while performing calculations.  
- Perform statistical measures such as mean, median, weighted mean, and standardization.  
- Explore array operations like reshaping, indexing, broadcasting, and dot product.  
- Gain practical skills in **NumPy** and **Pandas** for data analysis.  

---

## 📌 Problem Statements

### Problem 1: Statistical Measures
- Compute:  
  a) Mean  
  b) Median  
  c) Age-weighted mean of income  
- Ignore NaNs where appropriate.  
- Explain when a **weighted mean** is preferable.  

### Problem 2: Standardization & Outlier Detection
- Standardize income using **z-score**.  
- Identify the number of outliers using the rule |z| > 3.  
- Handle NaNs correctly without dropping entire rows unnecessarily.  

### Problem 3: Age-based Analysis
- Create **age bins**: [18–25), [25–35), [35–45), [45–60).  
- For each bin, compute:  
  - Count of observations  
  - Mean income  
  - Median income  
- Present the results as a **tidy DataFrame** sorted by age bin.  

### Problem 4: NumPy Array Operations
- Create a **multi-dimensional array**.  
- Demonstrate:  
  - **Shape & Resize:** shape, size, transpose, flatten  
  - **Indexing:** negative indexing, slicing errors  
  - **Arithmetic Operations:** broadcasting, dot product  

---

## ⚙️ How to Run
1. Open **Practical-1.ipynb** in *Jupyter Notebook* or *Google Colab*.  
2. Run the cells sequentially to view outputs.  
3. Install required libraries before running:


👩‍💻 Author
Nitika Thakur
B.Tech CSE (2023–2027)
Shoolini University

```bash
pip install numpy pandas matplotlib seaborn


