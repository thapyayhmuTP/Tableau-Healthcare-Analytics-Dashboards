# Tableau-Healthcare-Analytics-Dashboards
Interactive Tableau dashboards analyzing U.S. hospital quality, ownership, and staffing data — from exploratory insights to advanced forecasting and scenario modeling.

This repository presents a series of Tableau dashboards analyzing hospital quality, ownership, and workforce capacity across the United States.  
It demonstrates the progression from **exploratory data visualization** to **interactive dashboards** and **scenario forecasting**, using public healthcare data.

## Project Overview

### Part 1 – Exploratory Analysis of Hospital Quality
**Goal:** Identify patterns in hospital ratings, ownership, and patient experience.  
**Highlights:**
- Top-rated hospitals by state (Top N filter)
- Dual-axis chart comparing Mortality vs. Safety of Care
- Heatmap of Patient Experience (state and region level)
- Tree Map of hospital ownership and type
- Ratings by ownership (bar chart)
- Scatterplot showing Mortality vs. Safety relationship  

**Key Insights:**
- Non-profit hospitals consistently perform best across quality metrics.
- Midwest states show higher patient satisfaction; DC and Virgin Islands have the lowest.
- Ownership and type are key predictors of hospital quality.

---

### Part 2 – Interactive Dashboard for Quality Monitoring
**Goal:** Build an interactive Tableau dashboard for regulators and healthcare administrators to monitor and compare performance across states and counties.  
**Features:**
- **Geographic Map:** color-coded hospital ratings by state
- **Ranked Bar Chart:** overall rating comparison with drill-down
- **Emergency Services vs. Rating:** stacked bar visualization
- **County-Level Table:** ownership, type, and performance metrics (auto-updates via interactivity)
- **Parameter Controls:** toggle between quality indicators (mortality, readmission, timeliness)

**Design Highlights:**
- Tiled 1000×800 layout for consistency  
- Consistent color palette and clear labeling  
- Cross-highlighting between map, bar, and table views  

---

### Part 3 – Advanced Analysis & Scenario Modeling
**Goal:** Integrate multiple datasets and apply advanced Tableau techniques to forecast emergency demand and benchmark performance.  
**Techniques Used:**
- **Data Blending:** merged synthetic staffing dataset with hospital info via Provider ID  
- **LOD Expressions:** created benchmarks at state, ownership, and national levels  
- **Forecasting:** projected emergency department (ED) visit trends  
- **What-if Parameters:** simulated increased ED demand and staffing impact  
- **Navigation Buttons:** interconnected dashboards with persistent filters and parameter controls  

**Key Dashboards:**
- **Comparative View:** ownership vs. staffing ratios and quality outcomes  
- **National Benchmark Dashboard:** KPI panels and forecast visualizations  
- **KPI Map:** % of hospitals above/below national averages  

**Insights:**
- Rising ED demand significantly affects staffing and quality performance.  
- Non-profit hospitals maintain better outcomes across most metrics.  
- Forecasts indicate potential strain on ED resources by 2030, emphasizing proactive planning.

---

## Datasets
[`HospInfo.csv`](data/HospInfo.csv) | Original dataset from [CMS Hospital General Information](https://www.kaggle.com/datasets/cms/hospital-general-information) |
[`Cleaned_HospInfo.xlsx`](data/Cleaned_HospInfo.xlsx) | Standardized dataset used for Tableau dashboards |
[`synthetic_staffing.csv`](data/synthetic_staffing.csv) | Synthetic time-series dataset for staffing and forecasting analysis |
[`Data_Cleaning.tflx`](data/Data_Cleaning.tflx) | Tableau Prep flow used for preprocessing and cleaning |

---


## Skills Demonstrated

- Data Cleaning & Blending  
- Fixed LOD Calculations  
- Parameter & Filter Interactivity  
- Forecasting and Scenario Simulation  
- Dashboard Navigation and Usability Design  
- Healthcare Quality Analytics  

---

**Dataset Source:** [CMS Hospital General Information – Kaggle](https://www.kaggle.com/datasets/cms/hospital-general-information)
