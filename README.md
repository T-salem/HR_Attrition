# HR Analytics: Employee Attrition Analysis

## Project Overview

This project explores employee attrition to help HR and business stakeholders understand how often employees leave and which workforce characteristics are associated with higher attrition. The analysis uses an HR employee dataset and applies data cleaning, descriptive statistics, pivot-table analysis, and dashboard-style reporting to turn workforce data into actionable questions for retention planning.

The goal is not simply to count employees who left, but to identify patterns that HR teams can investigate further.

## Business Questions

- What proportion of employees in the dataset left the organisation?
- How does attrition vary across departments?
- Is attrition different for employees who work overtime?
- How are job satisfaction and work-life balance associated with attrition?
- Which workforce patterns may warrant further investigation by HR?

## Dataset

- **Records:** 1,470 employees
- **Outcome of interest:** `Attrition` (`Yes` or `No`)
- **Attrition cases:** 237
- **Employees who did not leave:** 1,233

The workbook includes employee demographics, department and job information, compensation, tenure, satisfaction ratings, overtime, and derived category fields. The cleaned-data worksheet also contains some fully blank columns and additional derived fields, so the workbook should be reviewed before being reused for further analysis.

> **Privacy note:** Do not publish employee-level data if it contains confidential or identifying information. If the dataset is shared publicly, confirm that its licence and source terms permit redistribution.

## Tools and Techniques

- **Microsoft Excel**
- Data cleaning and data-quality checks
- Descriptive statistics
- Pivot tables and grouped comparisons
- Dashboard-style visual reporting
- Business interpretation and recommendations

Only list additional tools (such as SQL, Python, Tableau, or Power BI) if they were actually used in this project.

## Analytical Approach

1. **Understand the data** — review the fields, row count, data types, and the meaning of the attrition outcome.
2. **Prepare the dataset** — check missing values, blank columns, duplicate records, and consistency of category labels.
3. **Create useful measures** — count employees and attrition cases, then calculate the attrition rate.
4. **Explore workforce patterns** — compare attrition across department, overtime, satisfaction, work-life balance, and other relevant employee attributes.
5. **Visualise the results** — use pivot tables and dashboard views to make comparisons easier to interpret.
6. **Translate findings into actions** — identify areas HR could investigate, while distinguishing association from causation.

## Key Findings

The following figures are calculated from the 1,470 employee records in the workbook's **Cleaned HR dataset** worksheet.

| Measure | Result |
|---|---:|
| Total employees | 1,470 |
| Employees who left | 237 |
| Employees who stayed | 1,233 |
| Overall attrition rate | 16.12% |

### Attrition by department

| Department | Employees | Attrition cases | Attrition rate |
|---|---:|---:|---:|
| Sales | 446 | 92 | 20.63% |
| Human Resources | 63 | 12 | 19.05% |
| Research & Development | 961 | 133 | 13.84% |

Sales has the highest attrition rate among the three departments in this dataset. Human Resources also has a higher rate than Research & Development, but its employee count is much smaller, so the percentage should be interpreted with that context.

### Attrition and overtime

| Overtime | Employees | Attrition cases | Attrition rate |
|---|---:|---:|---:|
| Yes | 416 | 127 | 30.53% |
| No | 1,054 | 110 | 10.44% |

Employees recorded as working overtime have a higher observed attrition rate than employees not recorded as working overtime. This is an association in the dataset, not proof that overtime alone causes employees to leave.

## Business Recommendations

Based on the patterns above, HR could:

1. **Investigate attrition in Sales** by reviewing role expectations, workload, management support, compensation, and career progression.
2. **Review overtime practices** to understand whether sustained workload, scheduling, or work-life balance may be contributing to employees' decisions to leave.
3. **Use employee feedback alongside the data** before implementing retention interventions.
4. **Monitor attrition over time** and compare rates across teams and employee groups, rather than relying only on organisation-wide totals.
5. **Evaluate interventions** by tracking whether attrition rates change after a policy or programme is introduced.

These are investigation priorities, not causal conclusions. The analysis is observational and does not establish why any individual employee left.

## Data Quality and Limitations

- The workbook contains 1,470 employee records, with 237 attrition cases.
- The cleaned-data worksheet has additional derived fields and fully blank columns; verify which fields are needed before using the data in another tool.
- Some fields are categorical ratings represented by numbers. Their meaning should be confirmed before treating them as continuous numerical measurements.
- Group sizes differ considerably, so rates should be read alongside employee counts.
- The analysis describes patterns in this dataset and should not be generalised automatically to every organisation.
- This is a descriptive analytics project; it does not claim to predict future attrition unless a separate predictive model is built and evaluated.

## Repository Structure

A simple GitHub repository structure could be:

```text
hr-analytics-employee-attrition/
├── README.md
├── data/
│   └── [add the dataset only if sharing is permitted]
├── reports/
│   └── [add exported dashboard images or report]
└── screenshots/
    └── [add dashboard screenshots]
```

Keep only folders and files that you actually add to the repository. If the workbook is not permitted for public redistribution, do not upload it; provide screenshots or a description of the dataset instead.

## How to Use This Project

1. Open the Excel workbook.
2. Review the **Cleaned HR dataset**, **Descriptive Statistics**, and **Pivot Analysis** worksheets.
3. Explore the dashboard worksheets to see how the measures are presented.
4. Recalculate the key metrics if the dataset changes.
5. Use the business questions and recommendations as a starting point for deeper analysis.

## Conclusion

This project demonstrates how employee data can be organised and explored to surface potential workforce-retention concerns. The analysis identifies an overall attrition rate of **16.12%**, a higher observed attrition rate in **Sales**, and a substantially higher rate among employees recorded as working **overtime**. These patterns provide a practical starting point for HR to investigate retention risks and make evidence-informed decisions.

---

**Author:** Paul Tolulope Oyewole-Salem  
**Project:** HR Analytics — Employee Attrition Analysis
