# Experiment 1: Data Analysis

**Name:** Isha  
**SAP ID:** 500119683  

## Objective

To perform exploratory data analysis on a structured dataset and derive meaningful insights using Python data manipulation and visualization libraries.

## Procedure & Implementation

The experiment uses **Pandas** for data manipulation and **Matplotlib** and **Seaborn** for data visualization. The dataset `employee_information_100.csv` is loaded and analyzed through the following tasks:

1. **Average Salary by Department:** Grouping employees by department using `groupby()` and calculating mean salaries using `mean()`, followed by visualization using a horizontal bar chart.

2. **Employee Count per Department:** Calculating the number of employees in each department using `value_counts()` and representing the results using a count plot.

3. **Gender Distribution:** Calculating gender frequencies and representing their proportions using a pie chart.

4. **Salary Distribution:** Creating a histogram with KDE to analyze the distribution and frequency of employee salaries.

5. **Experience vs. Salary Relationship:** Using a scatter plot to examine the relationship between years of experience and salary, categorized by department and gender.

6. **Top 10 Earners:** Identifying the ten employees with the highest salaries using `nlargest()`.

7. **Departmental Maximum Salaries:** Finding the maximum salary within each department using `groupby()` and `max()`.

8. **Above-Average Earners:** Filtering employees whose salaries are greater than the overall average salary of the organization.

9. **Average Experience per Department:** Calculating the average years of experience for employees in each department.

10. **Age Distribution:** Creating a histogram with KDE to understand the age distribution of employees.

## Observations

| Analysis Task | Key Observation Parameter | Visualization/Method |
| :--- | :--- | :--- |
| **Departmental Salary** | Comparison of average salaries across departments | Horizontal Bar Chart |
| **Employee Distribution** | Number of employees in each department | Count Plot |
| **Gender Demographics** | Proportion of employees by gender | Pie Chart |
| **Salary Frequency** | Distribution and common salary ranges | Histogram with KDE |
| **Experience & Pay** | Relationship between experience and salary | Scatter Plot |
| **Top Earners** | Identification of the 10 highest-paid employees | DataFrame Extraction (`nlargest`) |
| **Maximum Salaries** | Highest salary in each department | Groupby Aggregation (`max`) |
| **Above-Average Earners** | Employees earning more than the organizational average | Boolean Filtering |
| **Experience Trends** | Average experience across departments | Groupby Aggregation (`mean`) |
| **Age Spread** | Distribution of employee ages | Histogram with KDE |

## Result Interpretation & Learnings

- **Understanding the Dataset:** The analysis provides an overall understanding of the employee dataset and its important characteristics.
- **Data Visualization:** Different visualizations help identify salary variations, employee distribution, gender composition, and age patterns.
- **Salary & Experience Relationship:** The scatter plot helps analyze the relationship between employee experience and salary.
- **Data Aggregation:** The experiment provides practical experience with Pandas functions such as `groupby()`, `mean()`, `value_counts()`, `max()`, and `nlargest()`.
- **Data Filtering:** Boolean filtering is used to identify employees whose salaries are above the organizational average.
- **Visual Data Interpretation:** Matplotlib and Seaborn are used to convert numerical and categorical data into meaningful visual representations.
- **Overall Learning:** The experiment demonstrates how Python can be used to perform exploratory data analysis and extract useful insights from structured employee data.
