
# Production Line Downtime Reduction & OEE Analysis

**Data Source:** UCI Machine Learning Repository — AI4I 2020 Predictive Maintenance Dataset  
**Tools Used:** Microsoft Excel | Pareto Analysis | 5 Whys | TPM Framework

---

## 1. Problem Statement
A production line ran **10,000 cycles** with **339 machine failures** (3.39% failure rate). These failures cause unplanned downtime and lower plant output. 
- **Baseline Availability:** 96.61%
- **Baseline OEE:** 78.83%

## 2. Failure Analysis (Pareto)
| Failure Mode | Count | % of Failures |
|---|---:|---:|
| HDF — Heat Dissipation | 115 | 33.9% |
| OSF — Overstrain | 98 | 28.9% |
| PWF — Power Failure | 95 | 28.0% |
| TWF — Tool Wear | 46 | 13.6% |
| RNF — Random | 19 | 5.6% |

**Key Insight:** The top 3 failure modes (HDF, OSF, PWF) account for over 90% of all machine failures. 

*(Screenshot of Pareto chart: `Chart.png`)*

## 3. Root Cause Analysis (5 Whys)
**Top Failure: HDF (Heat Dissipation)**
1. Why HDF? → Temp differential exceeded 8.6K threshold.
2. Why? → Cooling system not maintained.
3. Why? → No preventive maintenance schedule.
4. Why? → No TPM framework in place.
5. Why? → Reactive maintenance culture.

## 4. Proposed Countermeasures (TPM)
- Daily temperature differential checks (HDF)
- Tool wear tracking + scheduled replacement (OSF, TWF)
- Power quality monitoring (PWF)
- Standard work for operator daily checks
- Link failure trends to VPO daily review

## 5. Results & Projected Impact
| KPI | Baseline | After TPM | Improvement |
|---|---:|---:|---:|
| Failures | 339 | 203 | −40% |
| Availability | 96.61% | 97.97% | +1.36 pts |
| OEE | 78.83% | 83.63% | +4.80 pts |

**Annualized Impact:** Recovers approx. **81,600 production cycles/year**.

## 6. Files Included
- `OEE_Project.xlsx` — Working Excel file (Formulas + Pareto Chart)
- `Chart.png` — Visual proof of failure analysis
- `OEE_Calc.png` — Screenshot of OEE calculation
- `Raw_Data.png` — Screenshot of raw data
