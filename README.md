# Police Traffic Stop Data Analysis with Python

**Project from:** *13 Python Data Analytics Real World Hands-on Projects* (Udemy)  
**Dataset:** `Police Data.csv` – Real-world traffic stop records

---

## Project Overview
This project analyzes **police traffic stop data** using **Pandas** to uncover patterns in **driver demographics**, **violations**, **search rates**, and **outcomes**. The dataset includes detailed records of stops, including gender, age, race, violation type, and arrest status.

---

## Dataset Columns
| Column               | Description |
|----------------------|-----------|
| `stop_date`          | Date of the stop |
| `stop_time`          | Time of the stop |
| `driver_gender`      | M/F |
| `driver_age`         | Age of driver |
| `driver_race`        | Race/ethnicity |
| `violation`          | Type of violation (e.g., Speeding, Equipment) |
| `search_conducted`   | True/False |
| `search_type`        | Reason for search (if conducted) |
| `stop_outcome`       | Citation, Warning, Arrest |
| `is_arrested`        | True/False |
| `stop_duration`      | Duration in minutes |

---

## Key Analysis Performed
- Cleaned missing values and standardized data types
- Grouped by **violation type** to analyze:
  - **Average driver age**
  - **Age distribution** (min, max, quartiles)
- Calculated **search and arrest rates**

> **Driver Age by Violation Type:**
> | Violation             | Avg Age | Min | Max |
> |-----------------------|--------|-----|-----|
> | **Speeding**          | 33.3   | 15  | 88  |
> | **Moving violation**  | 36.7   | 15  | 86  |
> | **Equipment**         | 31.7   | 16  | 81  |
> | **Other**             | 40.4   | 16  | 86  |

---

## Tools & Libraries
```python
pandas, numpy

```
### Insights Gained

- **Speeding is the most common violation** (37K+ stops)  
- **Older drivers (40+)** are more likely stopped for **"Other" violations**  
- **Younger drivers (under 30)** dominate **equipment violations**  
- **Searches are rare** but **highly correlated with drug-related stops**  
- **Useful for traffic safety, policy reform, and bias analysis**
