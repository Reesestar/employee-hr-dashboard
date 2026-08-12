# Employee HR Dashboard — Tableau

An interactive HR analytics dashboard built in Tableau, giving a quick overview of headcount, department distribution, compliance training status, and vacation usage across the company.

🔗 **https://public.tableau.com/views/EmployeeSpreadsheet_17865761667930/EmployeeSpreadsheet?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link(#)** 

![Dashboard screenshot](images/Employee-Spreadsheetpng)


## What's in the dashboard

- **Employee & Department counts** — quick KPI tiles for total headcount and number of departments
- **Employees by state** — a filled map showing employee distribution across department locations
- **Compliance training trend** — how many employees have completed required training over time
- **Employees trained** — list/detail view of employees who have completed compliance training
- **New hires per year** — headcount growth by employee start date
- **Top 10 employees by vacation usage** — highest vacation-day usage, ranked
- **T-shirt size distribution** — company merch sizing, sized and colored by employee count

## Data

The dashboard pulls from a single Excel workbook (`company_spreadsheet.xlsx`) with three related tables:

| Table | Rows | Description |
|---|---|---|
| `Employees` | 100 | id, name, department, start date, t-shirt size, vacation days taken |
| `Departments` | 34 | department name, address, office manager, desk count, state |
| `ComplianceTraining` | 46 | employee id, training completion date |

All data is sample/practice data, not real company records.

## Tools used

- **Tableau Public / Desktop** — dashboard design and data modeling (relationships across three tables)
- **Excel** — source data

## Files in this repo

- `Employee Spreadsheet.twbx` — the packaged Tableau workbook (open in Tableau Public or Desktop to explore/edit)
- `company_spreadsheet.xlsx` — underlying source data
- `images/dashboard-screenshot.png` — static preview of the finished dashboard

## Notes on reproducing this

If you open the `.twbx` file yourself, the data connection may point to a local file path from when it was built. To relink it to your own copy of `company_spreadsheet.xlsx`: right-click the data source in the Data pane → **Edit Connection** → browse to the file on your machine.
