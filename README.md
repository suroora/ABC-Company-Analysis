# ABC Company Employee Analysis (458 x 9)

This repository contains a complete, well-documented workflow to preprocess, analyze, and visualize the ABC company's employee dataset (458 rows, 9 columns).

## Files
- `ABC_Employee_Analysis.ipynb` — Main Jupyter Notebook with all analysis and plots.
- `ABC_Company_cleaned` — Used this Dataset for analysis

## Assumed Columns
The notebook expects these columns (case-insensitive):
- `team`
- `position`
- `age`
- `salary`
- `height`
  
## What the Notebook Does
### Preprocessing (1 mark)
- Validates schema and data types.
- Replaces the `height` column with random integers between 150 and 180 (inclusive), using a fixed random seed for reproducibility.
- Writes out a cleaned copy: `abc_employees_clean.csv`.

### Analysis Tasks
1. **Team distribution + percentage split** (2 marks)  
   - Count of employees by team and share of total.
   - Bar chart with counts and percentage annotations.

2. **Segregate employees by position** (2 marks)  
   - Distribution of employees across positions.
   - Bar chart and Pie Chart

3. **Predominant age group** (2 marks)  
   - Age binned into groups: `[10, 20, 30, 40,50]`.
   - Bar chart highlighting the largest group.

4. **Highest salary expenditure (team & position)** (2 marks)  
   - Total salary by team; total salary by position.
   - Two bar charts.

5. **Correlation between age and salary** (2 marks)  
   - Pearson correlation coefficient.
   - use heat map more finding Correlation 
   - Scatter plot with a simple best-fit line.

### Graphical Representation (10 marks)
Each analysis item above includes a clear plot created with Matplotlib (no seaborn).

### Data Story (3 marks)
A concise narrative at the end of the notebook summarizes key trends, patterns, and correlations observed in your data.

### Timely Submission (1 mark)
Notebook is structured for easy execution and export. Commit the notebook, dataset, and README to your GitHub repo, then submit the repo link.

## Suggested Repo Structure
```
abc-employee-analysis/
├─ ABC_Employee_Analysis.ipynb
├─ README.md
├─ ABC_Company_cleaned
├─ Team_distribution
├─ ABC_Company
```
