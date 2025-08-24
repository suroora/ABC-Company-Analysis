# ABC Company Employee Analysis (458 x 9)

This repository contains a complete, well-documented workflow to preprocess, analyze, and visualize the ABC company's employee dataset (458 rows, 9 columns).

## Files
- `ABC_Employee_Analysis.ipynb` — Main Jupyter Notebook with all analysis and plots.
- `data/` — Place your dataset file here (CSV or Excel). Example: `data/abc_employees.csv` or `data/abc_employees.xlsx`.
- `requirements.txt` — Python packages required to run the notebook.

## How to Run
1. Create and activate a virtual environment (optional but recommended).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Put your dataset in the `data/` folder (CSV or Excel). Update the `DATA_FILE` variable in the first cell of the notebook if needed.
4. Open and run `ABC_Employee_Analysis.ipynb` **top to bottom**.

## Assumed Columns
The notebook expects these columns (case-insensitive):
- `team`
- `position`
- `age`
- `salary`
- `height`

If your column names differ slightly (e.g., `Team Name`), the notebook includes a flexible matcher to help map them.

## What the Notebook Does
### Preprocessing (1 mark)
- Validates schema and data types.
- Replaces the `height` column with random integers between 150 and 180 (inclusive), using a fixed random seed for reproducibility.
- Writes out a cleaned copy: `data/abc_employees_clean.csv`.

### Analysis Tasks
1. **Team distribution + percentage split** (2 marks)  
   - Count of employees by team and share of total.
   - Bar chart with counts and percentage annotations.

2. **Segregate employees by position** (2 marks)  
   - Distribution of employees across positions.
   - Bar chart.

3. **Predominant age group** (2 marks)  
   - Age binned into groups: `<25`, `25–34`, `35–44`, `45–54`, `55+`.
   - Bar chart highlighting the largest group.

4. **Highest salary expenditure (team & position)** (2 marks)  
   - Total salary by team; total salary by position.
   - Two bar charts.

5. **Correlation between age and salary** (2 marks)  
   - Pearson correlation coefficient.
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
├─ requirements.txt
└─ data/
   └─ abc_employees.csv  # or .xlsx
```

## Tips
- If your dataset file is Google Sheets, export it as CSV first:
  - **File → Download → Comma Separated Values (.csv)**, then place it in `data/`.
- If you run into missing values or unexpected types, see the "Data Quality Checks" cell in the notebook.

Good luck!
