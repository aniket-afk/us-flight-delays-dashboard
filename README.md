# U.S. Flight Delays & Cancellations Dashboard  

An interactive **Tableau dashboard** analyzing U.S. domestic flight delays and cancellations using data from the U.S. Department of Transportation (DOT). This project demonstrates end-to-end **data engineering and analytics skills** — from building ETL pipelines to publishing a user-friendly dashboard with actionable insights.  

---

## 📊 Dashboard  
👉 [View on Tableau Public](https://public.tableau.com/)  

---

## 📂 Project Overview  
- **Goal:** Provide insights into U.S. flight performance by analyzing delay causes, cancellation patterns, and trends over time.  
- **Data Source:** [Bureau of Transportation Statistics (BTS) – On-Time Performance](https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp)  
- **Data Size:** ~1M flight records (1–2 years).  
- **Stack:** Python (Pandas), SQL, Tableau Public.  

---

## ⚙️ ETL Pipeline  
1. **Data Collection:** Downloaded CSV files from BTS / Kaggle.  
2. **Data Cleaning (Python + Pandas):**  
   - Fixed date formats, handled missing values, standardized airline/airport codes.  
   - Removed outliers (e.g., negative or unrealistic delay times).  
3. **Transformation:**  
   - Aggregated delays by **airline, airport, month, and cause**.  
   - Created new features: `% delayed flights`, `% cancellations`, `average delay minutes`.  
4. **Export:** Saved cleaned dataset as CSV for Tableau.  

---

## 📈 Dashboard Features  
- **KPI Summary:** On-time %, delayed %, canceled %.  
- **Delays by Cause:** Stacked bar chart showing breakdown (Weather, Carrier, NAS, Late Aircraft, Security).  
- **Airport Performance:** Interactive U.S. map with average delay/cancellation rates.  
- **Airline Comparison:** Delay and cancellation rates across carriers.  
- **Trends Over Time:** Monthly delay and cancellation trends with filters.  

---

## 🔑 Key Insights (Sample)  
- Weather delays spike in **winter months (Jan–Feb)**, contributing ~40% of delays.  
- **Atlanta (ATL)** has the highest flight volume but maintains strong on-time performance.  
- **Southwest Airlines** showed higher cancellation percentages during operational disruptions in 2022.  
- Weekends generally had fewer flights but higher average delays compared to weekdays.  

---

## 📁 Repository Structure  
us-flight-delays-dashboard/
│── data/ # Raw & cleaned datasets (CSV)
│── notebooks/ # Python ETL scripts (Jupyter/Pandas)
│── tableau/ # Tableau workbook (.twbx)
│── README.md # Project documentation


---

## 🛠 Tech Stack

Programming: Python (Pandas, NumPy, Matplotlib), SQL

Visualization: Tableau Public

Data Sources: U.S. DOT BTS, Kaggle (backup datasets)

---
## 👤 Author

Aniket Patole
