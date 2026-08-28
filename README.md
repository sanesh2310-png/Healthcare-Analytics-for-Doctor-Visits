# Healthcare-Analytics-for-Doctor-Visits
# Healthcare Analytics for Doctor Visits

A data analysis project exploring doctor visit records to understand patient
flow, wait times, treatment costs, and satisfaction across departments.

## Problem Statement

- Doctor visit records vary widely by department, wait time, diagnosis, and cost.
- It is difficult to identify which factors drive long wait times and patient dissatisfaction.
- Hospitals and clinics need data-driven insights to manage patient load and staffing.
- This project analyzes historical doctor visit data to uncover patterns in patient care.
- The goal is to deliver insights that support better scheduling, staffing, and patient outcomes.

## Objectives

- Analyze patient visit patterns across departments, doctors, and time periods.
- Identify the key drivers of patient wait time and appointment delays.
- Study the relationship between treatment cost, insurance type, and visit type.
- Evaluate patient satisfaction scores against wait time and visit duration.
- Present visual insights that support scheduling and resource-planning decisions.

## Dataset

The dataset contains doctor visit records, including:

| Column | Description |
|---|---|
| `patient_id` | Unique patient identifier |
| `age`, `gender` | Patient demographics |
| `visit_date` | Date of the visit |
| `department` | Hospital department (Cardiology, Pediatrics, etc.) |
| `doctor_id` | Attending doctor identifier |
| `diagnosis` | Recorded diagnosis for the visit |
| `visit_type` | In-Person or Telehealth |
| `wait_time_minutes` | Time spent waiting before being seen |
| `visit_duration_minutes` | Length of the consultation |
| `treatment_cost` | Cost of the visit (USD) |
| `insurance_type` | Private, Government, Self-Pay, Employer-Sponsored |
| `follow_up_required` | Whether a follow-up visit is needed |
| `satisfaction_score` | Patient-reported satisfaction (1-5) |

> Replace `doctor_visits.csv` with your assigned dataset before running the analysis.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Project Structure

```
healthcare-analytics-doctor-visits/
├── healthcare_analysis.py   # Main analysis script
├── doctor_visits.csv        # Dataset (add your assigned dataset here)
├── requirements.txt         # Python dependencies
├── README.md
└── outputs/                 # Generated charts
    ├── age_distribution.png
    ├── visits_by_department.png
    ├── avg_wait_time_by_department.png
    ├── cost_by_insurance_type.png
    ├── waittime_vs_satisfaction.png
    ├── visit_type_distribution.png
    ├── top_diagnoses.png
    └── correlation_heatmap.png
```

## How to Run

```bash
pip install -r requirements.txt
python healthcare_analysis.py
```

## Key Insights

- Wait times differ significantly by department, with higher-acuity departments like Cardiology and Orthopedics running longer than routine ones like Dermatology and Pediatrics.
- Patient satisfaction trends downward as wait time increases, regardless of visit type.
- In-person visits still make up the majority of appointments, though telehealth accounts for a meaningful share.
- Treatment cost is more strongly tied to department and diagnosis than to insurance type alone.


