# Insurance-Analysis

🧾 Purpose

This dataset contains policyholder demographics, insurance renewal status, health follow-ups, and risk priority segmentation.
It appears designed for insurance retention, claim follow-up analysis, and risk stratification.

🏷️ Key Fields Overview
Column	Meaning
Patient Id	Unique insurance member ID
Patient Name	Full registered name
Gender	Male / Female
Date of Birth	Original DOB format
Updated_DOB	Cleaned YYYY-MM-DD DOB
Year_DOB	Extracted birth year
AGE	Age calculated from DOB
Age Group	Categorized (Adult, Middle-aged, Senior)
Income (LPA)	Annual income bracket
Location (state)	Residential state
Region	Zonal cluster (North, South, East, West)
TRIM_NAME	Cleaned name (spaces corrected)
First_Name	Extracted first name
Name_01 / Name_02	Split name components
Report_Name	Auto PDF name pattern
Priority	Renewal urgency (Regular, High Priority)
Further_Priority	Action type
Further_Priority_IFS	Action using IFS logic
Count	Region-wise total people (reference counts)
🧠 Dataset Highlights

Age segmentation already prepared → Adult, Senior, Middle-aged

Policy urgency labels:

Regular Followup

High Priority

Needs Attention

Ask for Readmission

No Action

Contains Region summary counts integrated inside the sheet

Name cleaning & PDF generation logic included

🧰 Transformations Already Done (from columns observed)

✔ Date formatted to ISO standard
✔ Age calculated
✔ Name split into components
✔ Priority logic assigned
✔ Follow-up logic defined using IFS
✔ Automatic report naming pattern created
✔ Regional grouping w/ total counts

📊 Potential Use Cases
Analysis Goal	Output Expected
Renewal Risk Prediction	Who needs urgent outreach
Income vs Age Claims Pattern	High premium or high risk clusters
Region-wise health utilization	Zonal priority mapping
Senior segment retention	Prioritize 65+
Follow-up Scheduling	Automation through PDF naming
📈 Suggested Dashboards (Power BI / Excel)

Renewal Priority Funnel

High → Regular → No Action

Age Group vs Claim Priority

Identify risk-heavy age groups

Income vs Region Heatmap

Premium capacity & behavior

State-wise Patient Count

Distribution map

🔍 Data Quality Notes

Names are fully cleaned (TRIM done)

DOB cleaned into standard ISO & Age derived correctly

Priority & Re-admission flags are rule-based and consistent

Region summary counts included → verify for duplication before dashboard use

✔ Recommended Next Steps

Create retention model (who is likely to renew)

Link medical history if available to improve segmentation

Visualize High Priority + Senior + Low Income cluster
