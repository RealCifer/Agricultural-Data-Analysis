# Agricultural Data Analysis  
## Impact of Water and Fertilizer Overuse on Crop Productivity & Sustainability

---

## Project Objective

Overuse of water and fertilizers increases agricultural production cost and leads to environmental damage such as groundwater depletion, soil degradation, and reduced long-term sustainability.

This project performs a comprehensive data-driven analysis of agricultural production, fertilizer usage, climate trends, and groundwater depletion using statistical methods and satellite data.

The study focuses primarily on:

- Rice production in **Tamil Nadu**
- Agricultural trends in **Karnataka**
- Fertilizer efficiency analysis
- Groundwater depletion using GRACE satellite data
- Climate data integration

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
│   └── karnataka_rice_2000_2017.csv
│
├── notebook/
│   ├── 01_data_loading.ipynb
│   ├── 02_yield_trend_analysis.ipynb
│   ├── 03_water_analysis.ipynb
│   ├── 04_fertilizer_analysis.ipynb
│   ├── 05_groundwater_analysis.ipynb
│   └── 06_conclusion_and_recommendations.ipynb
│
├── results/
├── report/
└── README.md
```



---

# DATASETS USED

## Crop Production & Fertilizer Dataset

Source: Historical agricultural dataset  
File: `Custom_Crops_yield_Historical_Dataset.csv`

Filtered:
- State: Tamil Nadu & Karnataka
- Crop: Rice
- Years: 2000–2017

Key Variables:
- Yield_kg_per_ha
- N_req_kg_per_ha
- P_req_kg_per_ha
- K_req_kg_per_ha
- Total_N_kg
- Rainfall_mm
- Temperature_C
- Humidity_%

---

## Groundwater Dataset (GRACE Satellite)

Files:
- grace_2003_2008.csv
- grace_2009_2017.csv

Key Variables:
- date
- ADM2_NAME (district)
- mean (groundwater storage anomaly)

Tamil Nadu districts analyzed:
- Pudukkottai
- Ramanathapuram
- Thanjavur
- Cuddalore
- Nagapattinam

---

## Climate Dataset

Files from:
- chirps_rainfall_timeseries.xlsx
- soil moisture datasets
- SPEI drought index datasets

Used for:
- Rainfall trend analysis
- Climate variability interpretation

---

# ANALYSIS PERFORMED

---

# Yield Trend Analysis (Tamil Nadu & Karnataka)

Filtered rice production data from 2000–2017.

Key Observation:
- Rice yield shows an overall increasing trend.
- Productivity improved over the study period.

Implication:
- Technological or fertilizer inputs may be contributing to yield gains.

---

# Fertilizer Usage Analysis

### Nitrogen vs Yield Correlation

Computed yearly averages and totals.

Correlation Result:
- Total Nitrogen vs Yield ≈ **0.886**

Interpretation:
- Strong positive relationship between nitrogen use and yield.
- Nitrogen significantly influences rice productivity.

---

# Fertilizer Overuse Detection

Identified years where:
- Nitrogen usage > average
- Yield < average

Detected inefficient years:
- 2001
- 2006

Interpretation:
- Evidence of diminishing returns.
- Possible over-fertilization.

---

# Nitrogen Use Efficiency Index

Formula:

Nitrogen Efficiency = Yield / Total Nitrogen Applied

Findings:
- Efficiency fluctuates over years.
- Some periods show declining efficiency.
- Indicates diminishing marginal productivity of fertilizer.

Implication:
- Increasing fertilizer does not always proportionally increase yield.
- Risk of economic inefficiency.

---

# Groundwater Depletion Analysis (GRACE Satellite)

Converted daily data to yearly averages.

Applied Linear Regression to detect trend.

Results:

- Annual groundwater change rate: **-0.47 units per year**
- Total decline (2003–2017): **-10.4 units**

Interpretation:
- Significant groundwater depletion.
- Indicates sustained extraction over time.
- Environmental sustainability concern.

---

# Climate & Rainfall Observations

- Rainfall variability analyzed using climate datasets.
- Some datasets showed non-overlapping years.
- Climate fluctuations may influence irrigation demand.
- Groundwater depletion likely linked to irrigation intensity.

---

# Integrated Interpretation

| Component | Result |
|------------|--------|
| Yield Trend | Increasing |
| Nitrogen Correlation | Strong Positive (0.886) |
| Efficiency | Fluctuating |
| Over-Fertilization | Identified Years |
| Groundwater Trend | Declining |
| Annual Depletion | -0.47 units/year |

Conclusion:

While fertilizer usage contributes to yield growth, groundwater levels show consistent decline, suggesting increased irrigation demand and potential environmental stress.

This indicates a productivity–sustainability trade-off.

---

# Environmental Implications

- Over-fertilization may cause soil nutrient imbalance.
- Excess nitrogen can lead to water contamination.
- Groundwater depletion threatens long-term agriculture.
- Increased input use increases farmer production cost.
- Sustainability must be prioritized.

---

# Recommendations

1. Adopt precision fertilizer application.
2. Promote drip and micro-irrigation systems.
3. Implement soil health monitoring programs.
4. Encourage sustainable water policies.
5. Use satellite monitoring for real-time tracking.

---

# Future Work

- Integrate Sentinel-2 NDVI vegetation analysis.
- Apply machine learning models for yield prediction.
- Expand study to multi-state comparative analysis.
- Include irrigation intensity datasets.
- Perform district-level modeling.

---

# Technical Skills Demonstrated

- Data Cleaning & Filtering
- Time-Series Analysis
- Correlation Analysis
- Linear Regression Modeling
- Efficiency Metric Construction
- Satellite Data Processing
- Multi-dataset Integration
- Environmental Interpretation

---

# Final Conclusion

This project demonstrates that while fertilizer application significantly increases rice yield, groundwater resources are consistently declining.

Sustainable agricultural practices must balance productivity with environmental conservation to ensure long-term food security.

---

