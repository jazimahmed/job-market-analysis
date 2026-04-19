# 📊 IT Job Market Analysis — Data Analyst Jobs

A data cleaning and visualization project analyzing **2,253 Data Analyst job listings** sourced from Glassdoor. The project covers salary trends, job distribution by location, and role-level breakdowns across the US IT job market.

---

## 📸 Dashboard Preview

![IT Job Market Analysis Dashboard](/Visuals/dashboard.png)

> Power BI dashboard showing average salaries by job title, geographic distribution of job listings, and key market metrics.

---

## 📁 Project Structure

```
job-market-analysis/
│
├── DataAnalyst.csv          # Raw dataset (Glassdoor job listings)
├── DataAnalyst_cleaned.csv  # Cleaned dataset after preprocessing
├── analysis.ipynb           # Data cleaning & EDA notebook
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

The raw dataset required significant preprocessing before analysis:

| Issue | Fix Applied |
|---|---|
| Rating embedded in Company Name | Stripped newline + rating from company string |
| Salary as string range | Extracted min/max salary as numeric columns |
| `-1` used as placeholder for missing values | Replaced with `NaN` across all affected columns |
| `Size` had both `"Unknown"` and `"-1"` | Unified to `NaN` |
| `Easy Apply` had `"-1"` instead of `False` | Standardised to boolean |
| `Founded` had `-1` for unknown years | Replaced with `NaN` |
| `Competitors` had `-1` for no entry | Replaced with `NaN` |
| 1 missing `Company Name` | Flagged and handled |

---

## 📊 Visualisations

### Average Salary by Job Title
Horizontal bar chart ranking Data Analyst roles from highest to lowest average salary. AI/Senior roles command the highest compensation at ~$150K–$175K.

### Job Distribution by Location (Pie Chart)
Geographic breakdown of all 2,253 listings across US cities. New York leads significantly, followed by Chicago, San Francisco, and Austin.

### KPI Cards
- Total Jobs: **2,253**
- Average Salary: **$89.94K**

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python (pandas) | Data cleaning & preprocessing |
| Power BI | Dashboard & visualisation |
| Glassdoor Dataset | Source data |

---

## 🚀 Getting Started

### Prerequisites
```
python >= 3.8
pandas
```

### Run the cleaning notebook
```bash
git clone https://github.com/jazimahmed/job-market-analysis.git
cd job-market-analysis
jupyter notebook analysis.ipynb
```

---

## 📂 Dataset

The dataset was sourced from Glassdoor and contains the following fields:

`Job Title` · `Salary Estimate` · `Job Description` · `Rating` · `Company Name` · `Location` · `Headquarters` · `Size` · `Founded` · `Type of Ownership` · `Industry` · `Sector` · `Revenue` · `Competitors` · `Easy Apply`

---

## 👤 Author

**Jazim Ahmed**
[GitHub](https://github.com/jazimahmed) 

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).