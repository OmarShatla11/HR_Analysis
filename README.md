# 📊 HR Analytics & Employee Retention Dashboard - Power BI

## 📌 Executive Overview
This interactive 2-page Power BI dashboard offers an end-to-end HR Analytics solution designed to evaluate employee attrition drivers, job satisfaction levels, and work environment impact. By analyzing key metrics across departments, age demographics, tenure, and overtime habits, this dashboard equips HR leadership with actionable insights to mitigate employee turnover.

---

## 🎯 Key Dashboard Features
* **Executive Summary Page (`Executive & Attrition Overview`):** Highlights core KPIs (Total Headcount, Attrition Count, Attrition Rate, Avg Monthly Income) and key attrition demographics across departments, age groups, and years at the company[cite: 7].
* **Deep-Dive Page (`Satisfaction & Overtime`):** Focuses on employee well-being, work-life balance, environment satisfaction, and job roles analysis via an interactive Matrix visual[cite: 8].
* **Interactive Controls:** Includes global slicers for Gender, Department, and Job Level, alongside custom **Page Navigators** and a **"Clear All Filters"** button for seamless user experience[cite: 7, 8].

---

## 💡 Key Business Insights & Recommendations

### 1. 🚨 High-Risk Departments & Job Roles
* **Insight:** The **Research & Development (R&D)** department accounts for the vast majority of resignations[cite: 7]. At the role level, **Laboratory Technicians** (23.94%) and **Human Resources** staff (23.08%) experience the highest attrition rates[cite: 8].
* **Actionable Recommendation:** Conduct targeted stay-interviews for R&D and Laboratory staff. Re-evaluate compensation structures and workload distribution in these technical positions[cite: 7, 8].

### 2. ⏰ Overtime & Work-Life Balance Correlation
* **Insight:** Overtime is a significant catalyst for turnover[cite: 8]. Employees working **Overtime (`Yes`)** demonstrate a significantly higher rate of departure compared to non-overtime staff[cite: 8].
* **Actionable Recommendation:** Implement strict overtime caps and balance workloads by hiring part-time support or re-allocating tasks, which could reduce voluntary resignations in high-stress departments by up to 50%[cite: 7, 8].

### 3. 👥 Age Demographics & Tenure Trends
* **Insight:** Employees aged **26–35** constitute the largest group leaving the company[cite: 7]. Attrition peaks within the first **1 to 3 years** of tenure before stabilizing[cite: 7].
* **Actionable Recommendation:** Enhance the onboarding experience and establish clear 3-year career development pathways and mentorship programs to retain young professionals during their critical early years[cite: 7].

### 4. 🏢 Work Environment & Satisfaction
* **Insight:** Management positions display the lowest turnover rate (4.90%)[cite: 8]. Low environment satisfaction ratings closely align with higher attrition, especially in entry and mid-level roles[cite: 8].
* **Actionable Recommendation:** Improve workplace culture and environmental conditions for non-management roles to mirror the stability seen in executive/management levels[cite: 8].

---

## 🛠️ Tech Stack & DAX Measures Used
* **Tool:** Power BI Desktop
* **Key DAX Measures Created:**
  * `Attrition Count` = `CALCULATE(COUNT('HR_Analytics'[EmpID]), 'HR_Analytics'[Attrition] = "Yes")`
  * `Attrition Rate %` = `DIVIDE([Attrition Count], [Total Employees], 0)`
  * `Avg Job Satisfaction` = `AVERAGE('HR_Analytics'[JobSatisfaction])`
  * `Avg WorkLifeBalance` = `AVERAGE('HR_Analytics'[WorkLifeBalance])`

---

## 📸 Dashboard Screenshots

| Executive Overview | Satisfaction & Overtime |
| :---: | :---: |
| ![Executive Overview](./Executive%20%26%20Attrition%20Overview.png) | ![Satisfaction & Overtime](./Satisfaction%20%26%20Overtime.png) |
---
