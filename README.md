# 🎓 Student Depression Analysis - Tableau Dashboard
 
![Tableau](https://img.shields.io/badge/Tool-Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)
![SQL](https://img.shields.io/badge/Data%20Cleaning-SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Deployment](https://img.shields.io/badge/Deployed%20on-Tableau%20Public%20Cloud-E97627?style=flat-square&logo=tableau&logoColor=white)
![Status](https://img.shields.io/badge/Status-Live%20Project-brightgreen?style=flat-square)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
 
An interactive, **live** Tableau dashboard analyzing patterns of depression indicators among students, exploring how **sleep duration, study hours, academic pressure, financial stress, and study satisfaction** relate to student counts across the dataset. Data was cleaned using **SQL** prior to visualization, and the final dashboard is **deployed on Tableau Public Cloud** for public access.
 
🔗 **[View Live Dashboard on Tableau Public](https://public.tableau.com/app/profile/amit.yadav1803/viz/StudentDepressionAnalysis_17819114122320/StudentCountAnalysis)**
 
---
 
## 📊 Dashboard Preview
 
The dashboard is composed of 6 linked worksheets combined into a single interactive view, allowing exploration of student count distribution across five key wellbeing and lifestyle indicators.
 
| Worksheet | Focus Area |
|---|---|
| `SD & SC` | Sleep Duration vs Student Count |
| `SH & SC` | Study Hours vs Student Count |
| `SS & SC` | Study Satisfaction vs Student Count |
| `AP & SC` | Academic Pressure vs Student Count |
| `FS & SC` | Financial Stress vs Student Count |
| `Student Count Analysis` | Combined summary dashboard |
 
---
 
## 🧠 About the Dataset
 
- **Source:** [Kaggle](https://www.kaggle.com/) - Student Depression Dataset
- **Format:** Microsoft Excel (.xlsx), embedded in the workbook as a Tableau Extract for portability
- **Granularity:** One row per student record
### Key Fields Used
 
| Field | Description |
|---|---|
| Sleep Duration | Categorical buckets - *Less than 5 hours, 5-6 hours, 7-8 hours, More than 8 hours* |
| Study Hours | Numeric - hours spent studying |
| Study Satisfaction | Rated scale (1–5) |
| Academic Pressure | Rated scale (1–5) |
| Financial Stress | Rated scale (1–5) |
 
---
 
## 🧹 Data Cleaning & Preprocessing
 
Raw data was cleaned and preprocessed using **SQL** before being loaded into Tableau - handling tasks such as removing duplicate/null records, standardizing categorical values (e.g. sleep duration buckets), and structuring the dataset for direct use in Tableau worksheets.
 
---
 
## 🧮 Calculated Fields
 
| Field Name | Logic | Purpose |
|---|---|---|
| `Student Count (SC)` | `COUNT([Student ID])` | Aggregates the number of students falling into each category/bucket across all five lifestyle and wellbeing dimensions, used as the consistent measure across every worksheet in the dashboard |
 
---
 
## 🔍 Key Insights
 
- **Sleep Duration** is fairly evenly distributed across all four buckets (~123–128 students each), suggesting no single sleep pattern dominates the sample.
- **Study Satisfaction** peaks at level 4 (116 students), with a relatively balanced spread across the remaining levels.
- **Academic Pressure** is most concentrated at level 3 (125 students), tapering off at the highest pressure level.
- **Financial Stress** shows its highest concentration at level 1 (110 students), gradually declining as stress level increases.
- **Study Hours**, plotted as a trend across student count, shows a fluctuating pattern with a notable peak around the 10-hour mark.
---
 
## 🗂️ Repository Structure
 
```
student-depression-analysis/
│
├── README.md
├── Student Depression Analysis.twbx      # Tableau packaged workbook (extract embedded)
└── Depression Student Dataset.xlsx       # Raw source dataset
```
 
---
 
## 🛠️ Tools Used
 
- **SQL** - data cleaning & preprocessing
- **Tableau Desktop** - dashboard design & calculated fields
- **Tableau Public Cloud** - live deployment & public hosting
- **Microsoft Excel** - source data format
---
 
## 👤 Author
 
**Amit Yadav**
🔗 [LinkedIn](https://www.linkedin.com/) · [GitHub](https://github.com/mr-amit-yadav) · [Tableau Public Profile](https://public.tableau.com/app/profile/amit.yadav1803)
 
