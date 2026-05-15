# HealthPulse-Data-Analysis

---

## 📌 Project Overview

This project analyzes a dataset of 50,000 medical appointments to identify patterns behind patient "no-shows." The goal is to provide data-driven recommendations to optimize clinic scheduling and increase patient attendance.



## 📊 Business Problem

The clinic faces a 15% no-show rate, leading to lost revenue and inefficient use of medical staff. We need to identify:

1. Which days and locations are most affected?

2. Which resources (doctors) have the highest patient turnover?

3. How can we optimize the schedule to reduce these gaps?



## 🛠️ Tools Used

- **Excel:** Initial data cleaning and exploratory analysis (Pivot Tables).

- **Power BI:** Data modeling, DAX measures, and interactive dashboarding.




## 🧹 Data Cleaning & Methodology

To ensure accuracy, I performed the following steps:

- **Data Encoding:** Created an `Is_NoShow` flag (1 for No-Show, 0 for Attended) to calculate rates.

- **Time Extraction:** Extracted `Hour` and `Weekday` from raw timestamps to identify peak times.

- **Data Modeling:** Built a relationship between the appointment data and a central Calendar Table for better time-based filtering.


## Opertional Dashboard
<img width="1462" height="820" alt="HealthPulse Patient Appointment   No-Show Analysis" src="https://github.com/user-attachments/assets/3e9f3fdb-e3bf-490d-9097-fbdaa3fc4b20" />
*Figure 1: Healthpulse Patient Appointment Operational dashboard.*



## 💡 Key Insights

- **Temporal:** Saturdays have the highest no-show volume (over 1,100 missed visits).

- **Resource-Specific:** *Doctor D102* has a consistently high no-show rate across all clinics, suggesting a scheduling conflict rather than a location issue.

- **Geographic:** The Downtown Clinic leads in missed appointments, potentially due to local transit or parking barriers.



## 🚀 Recommendations

- **Double Confirmation:** Implement a Thursday call + Friday text for Saturday appointments.

- **Schedule Audit:** Review D102’s appointment intervals to reduce wait-time friction.

- **Capacity Planning:** Adjust staffing during peak hours (8 AM and 4 PM) identified in the trend analysis.
