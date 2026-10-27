# 🏦 Loan Approval Data Analysis — Python Project

A Python-based exploratory data analysis (EDA) project that examines loan applicant profiles, loan approval outcomes, financial attributes, and potential outliers using **Pandas, NumPy, Matplotlib, and Seaborn**.

## 📌 Project Overview

This project analyzes a dataset of **4,269 loan applications and 13 columns**. The Jupyter Notebook covers data inspection, data-quality checks, descriptive statistics, categorical summaries, visual exploration, CIBIL-score outlier checks using the Interquartile Range (IQR) method, and correlation analysis.

**Project scope:** This is an exploratory data analysis and visualization project. It does not train or evaluate a machine-learning model to predict loan approval.

## 🎯 Project Objectives

* Inspect the dataset structure, data types, distinct values, missing values, and duplicate records.
* Summarize numeric and categorical applicant features.
* Compare approved and rejected applications.
* Visualize financial-feature distributions using histograms and box plots.
* Explore the relationship between annual income and requested loan amount.
* Investigate potential CIBIL-score outliers using the IQR method.
* Examine correlations between numerical features.

## 🗂 Dataset Description

**Dataset:** `loan\\\_approval\\\_dataset.csv`  
**Size:** 4,269 rows × 13 columns

|Column|Description|
|-|-|
|`loan\\\_id`|Unique loan application identifier|
|`no\\\_of\\\_dependents`|Number of dependents|
|`education`|Applicant education category|
|`self\\\_employed`|Whether the applicant is self-employed|
|`income\\\_annum`|Applicant's annual income|
|`loan\\\_amount`|Requested loan amount|
|`loan\\\_term`|Loan term|
|`cibil\\\_score`|Applicant's CIBIL/credit score|
|`residential\\\_assets\\\_value`|Value of residential assets|
|`commercial\\\_assets\\\_value`|Value of commercial assets|
|`luxury\\\_assets\\\_value`|Value of luxury assets|
|`bank\\\_asset\\\_value`|Value of bank assets|
|`loan\\\_status`|Loan outcome: Approved or Rejected|

The notebook standardizes column names by stripping leading and trailing spaces before analysis.

## 🛠 Tools \& Technologies

* **Python** — analysis workflow
* **Pandas** — loading, inspecting, and preparing tabular data
* **NumPy** — numerical operations
* **Matplotlib** — plotting
* **Seaborn** — statistical visualizations
* **Jupyter Notebook** — documenting and running the analysis

## 🔄 Project Workflow

1. Load the CSV dataset into a Pandas DataFrame.
2. Inspect the dataset shape, column names, data types, missing values, and duplicates.
3. Standardize column names and review distinct values.
4. Generate descriptive statistics and categorical value counts.
5. Create histograms, count plots, box plots, and a scatter plot.
6. Investigate potential CIBIL-score outliers using the IQR method, including iterative filtering for a comparison.
7. Generate a correlation heatmap and review relationships between numerical features.

## 📊 Key Findings

The following findings are reported by the notebook and project presentation:

* **Loan applications:** 4,269 records.
* **Approved applications:** 2,656 (62.22%).
* **Rejected applications:** 1,613 (37.78%).
* **Data-quality checks:** The notebook reports no missing values and no duplicate rows in the original dataset.
* **Income and loan amount:** The scatter plot and correlation analysis show a strong positive relationship between annual income and requested loan amount (approximately 0.93 correlation).
* **CIBIL-score outliers:** The initial group-wise IQR check flags 42 potential outliers. The notebook then applies iterative IQR filtering, leaving 4,221 rows for a filtered comparison.

IQR flags identify observations for investigation; they do not automatically mean the values are erroneous. The original dataset is retained for the main analysis, and filtering is explored separately.

## 📈 Visualizations

The notebook includes:

* Histograms with KDE curves for numerical features
* Loan approval status count plot
* Box plots comparing income, loan amount, and CIBIL scores by loan status
* Scatter plot of annual income versus loan amount, colored by loan status
* Correlation heatmap for numerical features

The accompanying PowerPoint presentation summarizes the project overview, objectives, workflow, visualizations, and conclusion. Separate screenshot files are not required for this README.

## 📁 Repository Structure

Recommended repository layout:

```text
Python-Loan-Approval-Analysis/
├── README.md
├── Loan approval python project.ipynb
├── Loan\\\_approval\\\_dataset.csv
└── Loan approval python project presentation.pptx
```



## ▶️ How to Run the Project

1. Install Python and Jupyter Notebook, or use Visual Studio Code with the Jupyter extension.
2. Install the required libraries if they are not already available:

```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Keep `loan\\\_approval\\\_analysis.ipynb` and `loan\\\_approval\\\_dataset.csv` in the same project folder.
4. In the notebook, update the CSV loading cell to use a relative path.
5. Open the notebook and run the cells in order.
6. Review the printed summaries and generated charts.

## 👩‍💻 Skills Demonstrated

* Data loading and inspection with Pandas
* Data-quality checks and column-name standardization
* Descriptive statistics and categorical summaries
* Exploratory data analysis (EDA)
* Data visualization with Matplotlib and Seaborn
* IQR-based potential outlier detection
* Correlation analysis
* Communicating findings through a Jupyter Notebook and presentation

## 👤 Author

**Priyanka Asalekar**  
**Project:** Loan Approval Data Analysis  
**Tools:** ·Python · Pandas · NumPy · Matplotlib · Seaborn · Jupyter Notebook

\---

⭐ This project demonstrates a structured Python EDA workflow for examining applicant characteristics and loan approval patterns.

