# 📊 IT Job Market Analysis — Data Analyst Jobs

A data cleaning and visualization project analyzing **2,253 Data Analyst job listings** sourced from Kaggle. The project covers salary trends, job distribution by location, and role-level breakdowns across the US IT job market.

---

## 📸 Dashboard Preview

![IT Job Market Analysis Dashboard](/Visuals/dashboard.png)

> Power BI dashboard showing average salaries by job title, geographic distribution of job listings, and key market metrics.

---

## 📁 Project Structure

```
job-market-analysis/
│
├── DataAnalyst.csv          # Raw dataset (sourced from Kaggle)
├── DataAnalyst_cleaned.xlsx # Cleaned dataset after preprocessing in Excel
├── dashboard.pbix           # Power BI dashboard file
└── README.md
```

---

## 📌 Key Insights

- **Total Jobs Analysed:** 2,253
- **Average Salary:** $89.94K
- **Top Paying Role:** AI Insights Data Analyst (~$175K avg)
- **Top Location:** New York, NY (310 listings — 13.76% of all jobs)
- **Most Common Role:** Data Analyst (generic title, highest volume)

---

## 🧹 Data Cleaning Steps

The raw dataset was cleaned manually in **Microsoft Excel** before being loaded into Power BI:

| Issue | Fix Applied |
|---|---|
| Rating embedded in Company Name | Separated rating from company name using text functions |
| Salary stored as a string range | Split into Min Salary and Max Salary numeric columns |
| Inconsistent job title formatting | Standardised casing and removed extra whitespace |
| Duplicate rows | Identified and removed duplicates |
| Irrelevant columns | Removed columns not needed for analysis |

> **Note:** Fields with `-1` placeholder values were retained as-is in this version of the dataset.

---

## 📊 Visualisations

### Average Salary by Job Title
Horizontal bar chart ranking Data Analyst roles from highest to lowest average salary. AI and Senior roles command the highest compensation at ~$150K–$175K.

### Job Distribution by Location (Pie Chart)
Geographic breakdown of all 2,253 listings across US cities. New York leads significantly, followed by Chicago, San Francisco, and Austin.

### KPI Cards
- Total Jobs: **2,253**
- Average Salary: **$89.94K**

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data cleaning & preprocessing |
| Power BI | Dashboard & visualisation |
| Kaggle | Data source |

---

## 📂 Dataset

The dataset was sourced from **Kaggle** and contains Data Analyst job listings with the following fields:

`Job Title` · `Salary Estimate` · `Job Description` · `Rating` · `Company Name` · `Location` · `Headquarters` · `Size` · `Founded` · `Type of Ownership` · `Industry` · `Sector` · `Revenue` · `Competitors` · `Easy Apply`

---

## 🚀 Getting Started

1. Clone the repository
```bash
git clone https://github.com/jazimahmed/job-market-analysis.git
```
2. Open `DataAnalyst_cleaned.xlsx` to explore the cleaned data
3. Open `dashboard.pbix` in **Power BI Desktop** to interact with the dashboard

---

## 👤 Author

**Jazim Ahmed**
[GitHub](https://github.com/jazimahmed)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).