# Student Performance Data Analysis

**YuvaIntern -- Data Analyst Internship \| Task 3: Real-World Dataset
Analysis Project**

**Author:** Nandigam Praveen Kumar\
**Programme:** B.Tech -- Artificial Intelligence and Machine Learning

## Project Overview

This project explores a real-world student performance dataset from the
UCI Machine Learning Repository. The analysis uses Python to inspect the
data, check data quality, explore grade distributions, compare student
groups, calculate correlations, and create visualizations.

The main outcome examined is **G3**, the final course grade. Selected
variables include study time, previous failures, absences, sex, and home
address.

## Dataset

-   **Name:** Student Performance
-   **Repository:** UCI Machine Learning Repository
-   **Dataset ID:** 320
-   **Source:**
    https://archive.ics.uci.edu/dataset/320/student-performance
-   **Context:** Student achievement and related demographic, social,
    and school attributes from two Portuguese secondary schools.
-   **Records:** The course dataset used in this analysis contains 649
    student records.

The dataset is retrieved by the notebook using the `ucimlrepo` package.
The raw dataset is not included in this repository; use the official UCI
source above.

## Tools and Libraries

-   Python
-   Google Colab / Jupyter Notebook
-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn
-   `ucimlrepo`

## Project Workflow

1.  Retrieve the dataset from the UCI repository.
2.  Inspect the shape, columns, data types, and sample records.
3.  Check missing values and duplicate records.
4.  Prepare the analysis dataframe.
5.  Explore numerical distributions and categorical groups.
6.  Compare final grades across study-time and previous-failure
    categories.
7.  Examine the relationship between absences and final grades.
8.  Generate visualizations, including histograms, scatter plots, box
    plots, and a correlation heatmap.
9.  Summarize findings and limitations.

## Selected Findings from the Executed Notebook

The following values were observed in the executed notebook outputs:

  Analysis                                          Observed result
  -------------------------------------------- --------------------
  Mean G3 across study-time categories               10.84 to 13.23
  Pearson correlation: absences and G3                       -0.091
  Mean G3 across previous-failure categories          8.07 to 12.51
  Female students: count / mean / median G3      383 / 12.25 / 12.0
  Male students: count / mean / median G3        266 / 11.41 / 11.0
  Rural address: count / mean / median G3        197 / 11.09 / 11.0
  Urban address: count / mean / median G3        452 / 12.26 / 12.0

These are descriptive statistics for this dataset. They do not prove
that a variable causes a change in student performance. In particular,
the observed correlation between absences and G3 is very weak and
negative.

## Repository Structure

``` text
student-performance-data-analysis/
├── notebooks/
│   └── student_performance_analysis.ipynb
├── reports/
│   └── Task3_Report_Praveen.docx
└── README.md
```

## How to Run the Notebook

1.  Open [Google Colab](https://colab.research.google.com/).
2.  Upload `notebooks/student_performance_analysis.ipynb`.
3.  Select **Runtime → Run all**.
4.  Allow the notebook to install the required package and retrieve the
    dataset.
5.  Review the generated tables, charts, and observations.

An internet connection is required to retrieve the dataset from UCI.

## Important Limitations

-   The dataset represents students from two Portuguese secondary
    schools and may not represent all student populations.
-   The analysis is observational; group differences and correlations do
    not establish causation.
-   Correlation measures linear association and may not capture
    non-linear relationships.
-   UCI documentation notes that earlier-period grades G1 and G2 are
    strongly related to final grade G3. Using these variables in a
    predictive model before those grades are available can cause
    information leakage.

## Author

**Nandigam Praveen Kumar**\
B.Tech -- Artificial Intelligence and Machine Learning\
YuvaIntern Data Analyst Internship

## Acknowledgement

Thanks to the UCI Machine Learning Repository for providing the Student
Performance dataset for educational and research use.
