# 🏥 Healthcare Industry Dashboard — Power BI

An end-to-end, interactive **Healthcare Analytics Dashboard** built in Power BI, designed to transform raw hospital data into actionable insights for hospital management, healthcare stakeholders, and decision-makers.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoft&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

---

## 📌 Overview

This project simulates a real-world **Hospital Management & Healthcare Analytics** use case. It consolidates patient admissions, billing, medical conditions, medications, and insurance data into a single, interactive Power BI dashboard — enabling healthcare administrators to monitor performance, track revenue, and identify operational trends at a glance.

The dashboard is built with a focus on clean UX/UI, meaningful KPIs, and dynamic filtering, making it a strong portfolio piece for **Data Analyst**, **BI Developer**, and **Healthcare Analytics** roles.

---

## 🎯 Key Features

| Category | Details |
|---|---|
| 💰 **Revenue Analysis** | Total revenue tracked across hospitals, doctors, and insurance providers |
| 🏨 **Admissions Overview** | Total patient admissions with year-over-year trend analysis |
| 🏥 **Hospital & Doctor Metrics** | Count of unique hospitals and doctors in the network |
| 🩸 **Blood Type Distribution** | Patient breakdown by blood group |
| 🩺 **Medical Conditions Analysis** | Most common diagnoses across the patient population |
| 🛡️ **Insurance Provider Breakdown** | Revenue and patient volume by insurance provider |
| 💊 **Medication Usage Insights** | Most prescribed medications and usage patterns |
| 📈 **Admission Trends (YoY)** | Seasonal and year-over-year admission patterns |
| 👥 **Gender Distribution** | Patient demographics by gender |
| 🎂 **Age Bucket Analysis** | Patient distribution segmented into age groups |
| 🧪 **Test Results Summary** | Breakdown of normal, abnormal, and inconclusive test outcomes |
| 🎚️ **Dynamic Slicers** | Filter by Doctor, Hospital, Insurance Provider, and Admission Date |

---

## 🖼️ Dashboard Preview

##  OVERVIEW 

<img width="454" height="391" alt="Screenshot 2026-09-02 104617" src="https://github.com/user-attachments/assets/9981a771-4c47-4fab-93ee-34976b6bd884" />

## DASHBOARD 

<img width="453" height="395" alt="Screenshot 2026-09-02 104636" src="https://github.com/user-attachments/assets/5e1a4b29-52e6-4897-aa2f-34b259a9c6d6" />




``` 
--- 






## 🗂️ Dataset

This project uses the **Healthcare Dataset** publicly available on Kaggle.

- **Source:** [Healthcare Dataset — Kaggle](https://www.kaggle.com/datasets/prasad22/healthcare-dataset)
- **Records include:** Patient demographics, admission/discharge dates, hospital & doctor details, medical conditions, medications, insurance providers, billing amounts, and test results.

> ⚠️ Note: This is a synthetic dataset intended for educational and portfolio purposes. It does not represent real patient data (HIPAA-compliant / de-identified for practice use).

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** — Data modeling, visualization & report design
- **Power Query (M Language)** — Data cleaning and transformation
- **DAX (Data Analysis Expressions)** — Calculated columns, measures, and KPIs
- **Star Schema Data Modeling** — Fact and dimension table design for optimized performance

---

## 🔧 Project Workflow

1. **Data Extraction** — Sourced raw healthcare data (CSV) from Kaggle
2. **Data Cleaning & Transformation** — Used Power Query to handle nulls, standardize formats, and create derived columns (e.g., Age Buckets)
3. **Data Modeling** — Structured tables into a star schema for efficient relationships between patients, admissions, hospitals, and insurance
4. **DAX Measures** — Built custom measures for revenue, admissions, averages, and YoY growth calculations
5. **Dashboard Design** — Designed a clean, single-page interactive report with KPI cards, charts, and slicers
6. **Testing & Validation** — Verified visuals against source data for accuracy

---

## 📊 Key DAX Measures (Examples)

```dax
Total Revenue = SUM(Healthcare[Billing Amount])

Total Admissions = COUNTROWS(Healthcare)

Total Hospitals = DISTINCTCOUNT(Healthcare[Hospital])

Total Doctors = DISTINCTCOUNT(Healthcare[Doctor])

YoY Admissions Growth % = 
DIVIDE(
    [Total Admissions] - [Total Admissions PY],
    [Total Admissions PY]
)
```

---

## 📁 Repository Structure

```
Healthcare-Dashboard-PowerBI/
│
├── Healthcare_Dashboard.pbix     # Power BI dashboard file
├── dataset/                      # Raw/processed dataset (or link if too large)
├── assets/                       # Screenshots, GIFs, images
└── README.md                     # Project documentation
```

---

## 🚀 How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/Healthcare-Dashboard-PowerBI.git
   ```
2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/prasad22/healthcare-dataset) if not included due to file size limits.
3. Open `Healthcare_Dashboard.pbix` in **Power BI Desktop**.
4. Refresh the data source to point to your local dataset copy.
5. Explore the dashboard using the interactive slicers and visuals.

---

## 💡 Business Insights Delivered

- Identified top-performing hospitals and doctors by revenue and patient volume
- Highlighted the most common medical conditions and prescribed medications
- Surfaced seasonal/YoY admission trends to support capacity planning
- Enabled insurance-provider-level revenue comparisons
- Provided demographic breakdowns (age, gender, blood type) to support targeted healthcare programs

---

## 👤 About This Project

This dashboard was built as a portfolio project to demonstrate practical Power BI and data analytics skills applied to the healthcare domain — covering data cleaning, modeling, DAX, and dashboard design end-to-end.

If you're preparing for **Data Analyst** or **BI Developer** roles, feel free to fork this repo, explore the `.pbix` file, and adapt it for your own portfolio.

---

## 🤝 Connect With Me

- **LinkedIn:** www.linkedin.com/in/adityaakalyan
- **Portfolio:** https://www.datascienceportfol.io/adityakalyanbscc
- **Email:** adityakalyanbscc@gmail.com
- **Topmate:** https://topmate.io/aditya_kalyan
---

## ⭐ Support

If you found this project helpful, consider giving the repository a ⭐ — it helps others discover it too!

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
