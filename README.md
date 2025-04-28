# Niagara Health Patient Flow Analysis (April 2025)

This project analyzes simulated patient flow data for Niagara Health during a HIS (Health Information System) Go Live period.  
The goal was to identify patterns in admissions, discharges, and patient length of stay to recommend operational improvements.

---

## 📊 Project Highlights

- Analyzed patient admissions and discharges over time.
- Calculated average length of stay across different hospital units.
- Identified long-stay outliers (patients >7 days).
- Proposed recommendations for improving patient flow and resource planning.

---

## 📈 Admissions and Discharges Over Time

![Admissions and Discharges Chart](./niagara_health_patient_flow/niagara_health_patient_flow.png)

---

## 📑 Insights Summary

- Average Length of Stay: **5.4 days**
- 31% of patients stayed longer than 7 days.
- **Cardiology** had the longest average stay (~8 days).
- Peak admissions occurred around **April 3, 2025**, with discharges following 5–7 days later.
- Opportunities exist to improve discharge planning for high-load periods.

---

## 📋 Quick Metrics

| Metric | Value |
|:-------|:------|
| Average Length of Stay | 5.4 days |
| % Patients Staying >7 Days | 31% |
| Unit with Longest Stay | Cardiology |
| Peak Admission Date | April 3, 2025 |
| Peak Admission Count | 9 |

---

## 🧠 How Metrics Were Calculated

| Metric | Formula | Explanation |
|:-------|:--------|:------------|
| Average Length of Stay | `=AVERAGE(Length of Stay)` | Average number of days patients stayed. |
| % Patients Staying >7 Days | `=(COUNTIF(Length of Stay, ">7") / COUNTA(Patient ID)) * 100` | Percentage of long-stay patients. |
| Peak Admission Date | `=INDEX(Admission Date, MATCH(MAX(Admissions), Admissions, 0))` | Identified date with highest admissions. |
| Peak Admission Count | `=MAX(Admissions)` | Maximum daily admission count. |

---

## 📢 Recommendations

- **Monitor high average stay units** (Cardiology and Neurology) to optimize discharge planning.
- **Strengthen discharge planning during admission peaks** (early and late April).
- **Set up early alerts for extended-stay patients** (>7 days) for proactive case management.
- **Improve bed turnover processes** to handle high patient loads efficiently.

---

## 📂 Files Included

- `Niagara_Health_Patient_Flow_Analysis.xlsx` — Full Excel analysis workbook.
- `Insights_Summary_Screenshot.png` — Summary of key metrics and findings. (Optional if you add!)

---

## 🔗 Link to Portfolio

[Back to my Portfolio Site](https://seolheekim7.github.io)

---

