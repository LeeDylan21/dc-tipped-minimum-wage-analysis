# Effects of Tip Credit Elimination on Tipped Worker Earnings and Employment in Washington D.C.

Traditional microeconomic theory poses the tipped labor market as a simple supply and demand problem: any increase in tipped minimum wage results in a decrease in employment. And indeed, much existing published research reinforces this understanding. But in this study, I utilize a two-way fixed effects analysis of the gradual elimination of tip credit on worker earnings and employment in Washington D.C to show that the gradual increase in tipped minimum wage results in positive earnings effects and employment effects. To do this, I employed a border-discontinuity strategy popularized by Arindrajit Dube to better assert the parallel trends assumption between my control regions and the Washington D.C. area.

## Data and Methodology
- **Data Source:** The Bureau of Labor Statistics's (BLS) Quarterly Census of Employment and Wages (QCEW). The QCEW is a near complete census of employment and wage data of establishments that are covered by unemployment insurance.
- **Sample:** Quarterly employment and wage statistics for the full-service restaurant industry in Washington D.C. (treatment) and nine nearby counties (control) from 2017 Q1 to 2025 Q2. Each observation represents the full-service industry in a specific county during a specific quarter.
- **Treatment:** Washington D.C.'s Initiative 82 which utilized a gradual tip credit elimination phase-in. Therefore, the actual tipped minimum wage level is used rather than a simple before/after flag.
- **Model:** Two-way fixed effects (TWFE) controls for time-invariant county differences, like baseline economic characteristics and shocks common to all counties, like COVID-19.

## Findings
This study found that a $1 increase in the tipped minimum wage is associated with:
1. A +0.73% increase in average weekly wages for the full-service industry, statistically significant at the 1% level (p < 0.01).
2. A +2.51% increase in average quarterly employment for the full-service industry, statistically significant at the 1% level (p < 0.01).

### Average Weekly Wage
|   | Main Model | RC1: Binary DiD | RC2: No COVID | RC3: Contiguous Only |
| --- | :---: | :---: | :---: | :---: |
| **Log Weekly Wage** | 0.0073***<br>(0.0019) | 0.0202***<br>(0.0050) | 0.0065***<br>(0.0021) | 0.0082***<br>(0.0017) |
| **Observations** | 340 | 340 | 220 | 204 |
| **Within R^2** | 0.0101 | 0.0096 | 0.0118 | 0.0192 |
| **Entity FE** | Yes | Yes | Yes | Yes |
| **Time FE** | Yes | Yes | Yes | Yes |

### Average Quarterly Employment
|   | Main Model | RC1: Binary DiD | RC2: No COVID | RC3: Contiguous Only |
| --- | :---: | :---: | :---: | :---: |
| **Log Quarterly Employment** | 0.0251***<br>(0.0033) | 0.1024***<br>(0.0117) | 0.0014<br>(0.0052) | 0.0306***<br>(0.0032) |
| **Observations** | 340 | 340 | 220 | 204 |
| **Within R^2** | 0.0129 | 0.0191 | 0.0012 | 0.0211 |
| **Entity FE** | Yes | Yes | Yes | Yes |
| **Time FE** | Yes | Yes | Yes | Yes |

While these three robustness checks largely validate the results, it is important to note the effect that removing the COVID-19 time period has on the employment effect. While this robustness check still finds a positive effect on employment, the result loses significance. This suggests that the positive employment effects could partially also be driven by post-pandemic labor market recovery coinciding with the Initiative 82 phase-in, rather than just the policy alone.

## Acknowledgements
Data for this study was collected from BLS's QCEW.
