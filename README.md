# Excel Optimization Project – Sensitivity & QA Pipeline

## Overview
This project demonstrates advanced Excel modeling through a dynamic dashboard that evaluates upgrade efficiency across 76 planets and 304 scenarios. It integrates ROI, breakeven, and hybrid scoring to recommend optimal upgrades while maintaining transparency through structured documentation and validation.

## Story in Brief
The model ranks Mining, Speed, Cargo, and Unlock upgrades using ROI/hr and breakeven metrics. Only candidates with valid numeric results are considered. The dashboard dynamically identifies the best upgrade (#6 Newton – Mining, 100% hybrid score) and visualizes trade‑offs between ROI and payback time. Sensitivity testing applies ±10% changes to ore value, upgrade cost, and travel time to confirm model stability.

## Dashboard Highlights
- **Best Upgrade:** Newton – Mining (100% hybrid score)
- **Valid Candidates:** 8 of 304 records (6 Mining, 1 Speed, 1 Cargo)
- **Visual Trade‑off:** ROI vs Breakeven scatterplot
- **Sensitivity Analysis:** ±10% tests confirm ranking stability
- **Interactive Controls:** ROI/Breakeven weighting, timeframe units, telescope selection

![Planet Upgrade Dashboard](dashboard.png)
*Main dashboard showing ROI vs breakeven trade‑offs and top upgrade recommendations.*

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

![Model Guide](model-guide.png)
*Documents assumptions, data dictionary, and lineage for transparency.*

### Data Lineage
1. **Inputs:** Capture levels, telescope, distances, ore values, and costs  
2. **Upgrade Logic:** Calculate next‑state efficiency, ROI, and breakeven  
3. **Standardization:** Convert metrics into comparable rank scores  
4. **Consolidation:** Normalize 304 alternatives and apply weights  
5. **Quality Assurance:** Validate inputs and lookup consistency  
6. **Decision Output:** Present recommendations, charts, and sensitivity  

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
