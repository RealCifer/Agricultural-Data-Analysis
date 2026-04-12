# Agricultural Data Analysis  
## Impact of Water and Fertilizer Overuse on Crop Productivity & Sustainability

---

## Project Objective

This project analyzes the relationship between agricultural productivity and resource usage, focusing on fertilizer consumption, groundwater depletion, and climate variability.

The goal is to understand how increasing agricultural inputs impact yield while evaluating long-term sustainability.

---

## Key Features

- Multi-factor agricultural analysis (Yield, Fertilizer, Water, Groundwater)
- Satellite-based groundwater monitoring (GRACE data)
- Climate data integration (Rainfall trends)
- Time-series analysis (2000–2025)
- Predictive modeling using Linear Regression
- Sustainability recommendation system

---

## Project Structure

```
Agricultural_Data_Analysis/
│
├── data/
│   ├── archive/
│   ├── NDTV/
│   │   ├── climate_data/
│   │   └── groundwater_data/
│   ├── tamilnadu_rice_2000_2017.csv
│   └── karnataka_rice_2000_2017.cs
    └── extended_crop_dataset.csv
│
├── notebook/
│   ├── 01_data_loading.ipynb
│   ├── 02_yield_trend_analysis.ipynb
│   ├── 03_water_analysis.ipynb
│   ├── 04_fertilizer_analysis.ipynb
│   ├── 05_groundwater_analysis.ipynb
│   ├── 06_extended_data_analysis.ipynb
│   └── 07_sustainability_recommendations.ipynb    
    └── 08_Collective_analysis.ipynb
│
├── report/
└── README.md
```

---

## Datasets Used

### 1. Crop & Fertilizer Dataset
- Rice production data (Tamil Nadu & Karnataka)
- Years: 2000–2017
- Features:
  - Yield (kg/ha)
  - Fertilizer usage (N, P, K)
  - Rainfall
  - Temperature
  - Humidity

---

### 2. Groundwater Dataset (GRACE Satellite)

- Measures groundwater storage anomalies
- Unit: **cm (water equivalent)**
- Years: 2003–2017

---

### 3. Climate Dataset (CHIRPS)

- Daily rainfall data
- Unit: **mm/day**
- Aggregated to yearly averages

---

## Analysis Performed

---

### 1. Yield Trend Analysis

- Rice yield shows a consistent increasing trend.
- Indicates improved agricultural productivity.

---

### 2. Fertilizer Analysis

- Strong correlation between Nitrogen and Yield (~0.88)
- Evidence of over-fertilization in certain years
- Efficiency fluctuates over time

---

### 3. Groundwater Analysis

- Annual depletion rate: **-0.47 cm/year**
- Total decline: **-10.4 cm**

Interpretation:
- Continuous groundwater extraction
- Unsustainable irrigation practices

---

### 4. Rainfall Analysis

- Rainfall variability observed across years
- Impacts irrigation demand
- Influences groundwater usage

---

## Data Extension (2018–2025)

### Problem
Real datasets were limited to 2017.

### Solution
We extended the dataset using **Linear Regression**

### Method:
- Independent variable: Year
- Dependent variables:
  - Yield
  - Fertilizer
  - Groundwater
  - Rainfall

### Output:
- Predicted values for **2018–2025**
- Ensures continuity in time-series analysis

---

## Key Insight

- Yield increases with fertilizer usage  
- Groundwater consistently declines  
- Indicates a **productivity vs sustainability trade-off**

---

## Sustainability Recommendation System

We built a rule-based system using thresholds:

### Fertilizer Range
- Based on quartile analysis

### Groundwater Limits
- Safe level vs critical depletion

### Rainfall Range
- Optimal crop growth conditions

### Output:
- Suggests:
  - Reduce fertilizer
  - Increase irrigation
  - Avoid groundwater overuse
  - Optimal harvesting conditions

---

## Comparative Analysis

- Tamil Nadu → More stable yield  
- Karnataka → Higher variability  

Conclusion:
- Tamil Nadu shows more consistent agricultural performance

---

## Environmental Impact

- Soil degradation due to over-fertilization
- Groundwater depletion
- Increased production cost
- Long-term sustainability risk

---

## Recommendations

1. Precision fertilizer usage  
2. Controlled irrigation  
3. Groundwater monitoring  
4. Climate-aware farming  
5. Sustainable agricultural policies  

---

## Technical Skills Demonstrated

- Data Cleaning & Preprocessing  
- Time-Series Analysis  
- Correlation Analysis  
- Linear Regression  
- Data Visualization  
- Satellite Data Analysis  
- Sustainability Modeling  

---

## Final Conclusion

This project demonstrates that while fertilizer usage improves agricultural productivity, it comes at the cost of environmental sustainability.

Groundwater depletion and inefficient resource usage highlight the need for sustainable farming practices.

---

## Important Note

- Data from 2000–2017 is **real**
- Data from 2018–2025 is **predicted using Linear Regression**
- Predictions are clearly separated from actual data

---