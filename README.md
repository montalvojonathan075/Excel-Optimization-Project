# Excel Optimization Project – Sensitivity & QA Pipeline

## Overview
This project demonstrates advanced Excel modeling through a dynamic dashboard that evaluates upgrade efficiency across 76 planets and 304 scenarios. It integrates ROI, breakeven, and hybrid scoring to recommend optimal upgrades while maintaining transparency through structured documentation and validation.

## Story in Brief
The model ranks Mining, Speed, Cargo, and Unlock upgrades using ROI/hr and breakeven metrics. Only candidates with valid numeric results are considered. The dashboard dynamically identifies the best upgrade (#6 Newton – Mining, 100% hybrid score) and visualizes trade‑offs between ROI and payback time. Sensitivity testing applies ±10% changes to ore value, upgrade cost, and travel time to confirm model stability.

---

## Dashboard Highlights
- **Best Upgrade:** Newton – Mining (100% hybrid score)  
- **Valid Candidates:** 8 of 304 records (6 Mining, 1 Speed, 1 Cargo)  
- **Visual Trade‑off:** ROI vs Breakeven scatterplot  
- **Sensitivity Analysis:** ±10% tests confirm ranking stability  
- **Interactive Controls:** ROI/Breakeven weighting, timeframe units, telescope selection  

### Screenshots
![IPM Dashboard Part 1](IPM%20Dashboard%20Part%201.png)  
*Main dashboard showing ROI vs breakeven trade‑offs and top upgrade recommendations.*

![IPM Dashboard Part 2](IPM%20Dashboard%20Part%202.png)  
*Ranked list of upgrade candidates across planets, with ROI per hour, breakeven time, and hybrid score.*

![IPM Dashboard Part 3](IPM%20Dashboard%20Part%203.png)  
*±10% sensitivity analysis panel testing ore value, upgrade cost, and travel time to confirm model robustness.*

---

## Model Guide
The workbook includes a detailed **Model Guide** documenting assumptions, editable controls, and data lineage for transparency and reproducibility.

### Assumptions & Editable Controls
- ROI weight: 50%  
- Breakeven weight: 50%  
- Current telescope: 1  
- ROI display timeframe: Hours  
- Breakeven display timeframe: Seconds  
- Sensitivity range: ±10%  

### Data Dictionary
Defines all key metrics used in the model:
- **ROI/hr:** Incremental value per hour relative to upgrade cost  
- **Breakeven:** Time to recover upgrade cost  
- **Efficiency:** Deposit production relative to constraints  
- **Hybrid Score:** Weighted decision score combining ROI and breakeven  
- **Longevity Score:** Final tie‑breaker based on future efficiency  

### Screenshots
![IPM Guide Part 1](IPM%20Guide%20Part%201.png)  
*Documentation of assumptions and editable controls such as ROI/Breakeven weights, telescope selection, and sensitivity range.*

![IPM Guide Part 2](IPM%20Guide%20Part%202.png)  
*Data dictionary defining ROI/hr, Breakeven, Efficiency, Hybrid Score, and Longevity Score.*

![IPM Guide Part 3](IPM%20Guide%20Part%203.png)  
*Data lineage tracing the calculation chain from inputs to decision output, ensuring transparency and auditability.*

---

## Key Features
- Automated calculations with error handling  
- Scenario testing framework for ±10% sensitivity  
- QA validation layer ensuring consistent inputs  
- Interactive dashboards for real‑time decision support  
- Documentation for reproducibility and transparency  

## How to Use
1. Download the Excel workbook (`Idle Planet Miner.xlsm`).  
2. Enable macros when prompted.  
3. Adjust ROI/Breakeven weights or telescope level on the dashboard.  
4. Review updated recommendations, charts, and sensitivity results.  

---

*This project demonstrates structured analytical modeling, scenario validation, and dashboard design — bridging Excel automation with data‑driven decision workflows.*

