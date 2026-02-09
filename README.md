# Automated-Icu-Patient-Risk-Monitoring-Dashboard


## 📌 Project Overview

This project demonstrates an end-to-end **automated healthcare analytics pipeline** that identifies ICU patients at risk of deterioration or sepsis. The solution standardizes multilingual clinical data, applies rule-based risk scoring, and feeds an auto-refreshing Power BI dashboard.

The project is designed to reflect **real-world Data Analyst / Business Analyst / Operations Analyst work**, focusing on automation, data quality, and decision-ready insights.

---

## 🎯 Problem Statement

ICU patient monitoring data is often:

* Manually updated
* Inconsistent across systems
* Difficult to analyze quickly for risk identification

This increases the risk of delayed insights and inefficient reporting.

---

## ✅ Solution

An automated analytics pipeline that:

* Translates Turkish clinical data into a standardized English schema
* Cleans and validates ICU patient data
* Calculates SIRS, qSOFA, and NEWS-based risk scores
* Categorizes patients into High / Medium / Low risk
* Automatically refreshes results in Power BI

---

## 🧠 Key Features

* Full Python automation (no manual data prep)
* Multilingual data standardization (Turkish → English)
* Clinical risk scoring logic
* Power BI–ready output
* Scalable and refresh-safe design

---

## 🛠️ Tools & Technologies

* **Python** (pandas, numpy)
* **Excel** (source dataset)
* **Power BI** (dashboarding & DAX)
* **Windows Task Scheduler / Cron** (automation)

---

## 🔁 Automation Workflow

```
Raw ICU Excel Dataset
        ↓
Python Automation Script
(Data cleaning + translation + scoring)
        ↓
Clean English CSV Output
        ↓
Power BI Scheduled Refresh


## 📊 Risk Scoring Logic

### SIRS Criteria

* Fever > 38°C
* Pulse rate > 90
* Respiratory rate > 20
* WBC < 4 or > 12

### Composite Risk Score

```
Risk Score =
(SIRS × 2) + (qSOFA × 3) + (NEWS × 1.5)
```

### Risk Categories

* **High Risk**: Score ≥ 12
* **Medium Risk**: Score 6–11
* **Low Risk**: Score < 6

---

## 📈 Power BI Dashboard

The dashboard includes:

* Total ICU patients
* High / Medium / Low risk counts
* Risk score trends
* Patient-level risk table
* Interactive slicers

All visuals update automatically when the data refreshes.


## 🚀 How to Run

1. Clone this repository
2. Install dependencies:

```bash
pip install pandas numpy openpyxl
```

3. Run the automation script:

```bash
python icu_full_automation_pipeline.py
```

4. Connect the output CSV to Power BI
5. Enable scheduled refresh

<img width="1536" height="1024" alt="Automated project image" src="https://github.com/user-attachments/assets/35b6bd33-c68e-43d4-b9b2-02b1e0c97294" />

