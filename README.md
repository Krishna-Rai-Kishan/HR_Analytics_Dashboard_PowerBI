# HR Analytics Dashboard | Power BI

An interactive **HR Analytics Dashboard** built with Microsoft Power BI to analyze employee attrition, workforce demographics, salary distribution, job roles, and employee tenure. The dashboard helps HR teams explore workforce patterns and identify areas that may require further investigation.

![HR Analytics Dashboard Preview](images/dashboard_screenshot.png)

## Project Overview

Employee attrition can affect workforce stability, recruitment costs, and organizational productivity. This project transforms HR employee data into an interactive dashboard that allows users to explore attrition patterns across departments, job roles, age groups, salary bands, education fields, and years at the company.

The report uses **Power Query for data preparation, DAX for KPI calculations, and interactive Power BI visuals** to present workforce information in an accessible format.

## Key Performance Indicators (KPIs)

The dashboard displays six headline metrics:

| KPI | Dashboard Result |
|---|---:|
| Total Employees | 1,470 |
| Attrition Count | 237 |
| Attrition Rate | 16.1% |
| Average Age | 37 years |
| Average Monthly Income | 6.5K |
| Average Years at Company | 7.0 years |

## Dashboard Features

- **Attrition by Years at Company:** Explore attrition patterns across employee tenure.
- **Attrition by Salary Slab:** Compare attrition across salary categories.
- **Attrition by Age Group:** Examine attrition across different age groups.
- **Attrition by Job Role:** Compare attrition counts across job roles.
- **Attrition by Education Field:** Explore attrition across educational backgrounds.
- **Attrition by Gender:** Examine the distribution of attrition by gender.
- **Job Role and Job Satisfaction:** Compare attrition counts across job roles and satisfaction levels.
- **Department Slicer:** Filter the report by department and interactively explore the corresponding visuals.

## Data Preparation and Transformation

The project uses the IBM HR Analytics Employee Attrition dataset. Data preparation was performed in **Power Query Editor** before developing the dashboard.

The Applied Steps include:

1. **Promoted Headers:** Converted the first row into column headers.
2. **Removed Columns:** Excluded columns that were not required for the analysis.
3. **Removed Duplicates:** Removed duplicate records during data preparation.
4. **Replaced Value:** Replaced specified values to support consistent analysis.
5. **Changed Type:** Assigned appropriate data types to columns.
6. **Added Conditional Column:** Created a derived column based on conditional logic.
7. **Filtered Rows:** Applied row filters to prepare the final dataset.
8. **Changed Type 1:** Applied additional data-type adjustments after transformation.

An `AttritionCount` field was derived from the `Attrition` field, assigning a numeric value to support aggregation in Power BI.

The final report uses **1,470 employee records**, with 237 employees marked as having left the organization.

## Data Source

The dataset is the well-known IBM HR Analytics Employee Attrition dataset (CSV). Columns include demographics (Age, Gender, Marital Status), job details (Department, Job Role, Job Level), compensation (Monthly Income, Salary Slab), satisfaction scores (Job Satisfaction, Environment Satisfaction, Work-Life Balance), and tenure fields (Years at Company, Years in Current Role, Years Since Last Promotion).

An `AttritionCount` column (1/0) is derived in Power Query from the `Attrition` (Yes/No) field to support summable measures.

> **Note:** This is a static snapshot dataset, not a live connection — the data is embedded in the .pbix, so the report opens and displays correctly without needing to refresh.

## Repository Structure

```
HR-Analytics-Dashboard/
├── HR_Analytics_Dashboard.pbix    # Power BI report file
├── data/
│   └── HR_Analytics.csv           # Source dataset
├── images/
│   └── dashboard_screenshot.png   # Preview image for README
└── README.md
```

## How to Use

1. Download `HR_Analytics_Dashboard.pbix`
2. Open it in [Power BI Desktop](https://www.microsoft.com/power-bi/downloads) (free)
3. Use the Department slicer to filter; click any chart to cross-filter the rest of the page

## Business Questions Explored

The dashboard enables users to investigate questions such as:

- What proportion of employees have left the organization?
- How does attrition vary across departments and job roles?
- Which age groups and salary bands have higher attrition counts?
- How does attrition vary with years at the company?
- How is attrition distributed across education fields and gender?
- How do job roles and job satisfaction levels relate to attrition?
- How do these patterns change when a specific department is selected?

These views support exploratory workforce analysis. The observed patterns show associations and should not be interpreted as proof of causation.

## Tools and Technologies

- **Microsoft Power BI Desktop** — dashboard development and interactive reporting
- **Power Query Editor** — data cleaning and transformation
- **DAX** — measures and KPI calculations
- **Microsoft Excel / CSV** — data inspection and source-data handling
- **GitHub** — project versioning and portfolio presentation

## Key Learnings

Through this project, I practised:

- Preparing and transforming structured HR data using Power Query.
- Creating DAX measures for business KPIs.
- Designing a single-page dashboard with multiple visual types.
- Building interactive filters and cross-filtering experiences.
- Presenting workforce metrics in a business-oriented format.

## Future Improvements

- Add month-over-month or year-over-year attrition analysis if historical data becomes available.
- Introduce drill-through pages for detailed department and job-role analysis.
- Add clearer comparisons between attrition rates and employee counts where appropriate.
- Enhance report accessibility, titles, and tooltips for a better user experience.

---

**Project Type:** Business Intelligence / HR Analytics  
**Status:** Completed  
**Primary Skills:** Power BI, Power Query, DAX, Data Cleaning, Data Visualization, KPI Reporting