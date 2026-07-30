### In vitro and physicochemical data

The table below summarizes the drug-dependent inputs documented for the paroxetine model.

| Parameter | Unit | Value | Source | Description |
| --- | ---: | ---: | --- | --- |
| MW | g/mol | 329.37 | [Zhong 2013](#5) | Molecular weight. |
| pK<sub>a</sub>,base | - | 9.9 | [Agrawal 2013](#5) | pKa of a basic ionization site. |
| Solubility | mg/mL | 7.31 | [Khatavkar 2016](#5) | Aqueous solubility at pH 4.5. |
| logP | - | 3.95 | [Agrawal 2013](#5) | Octanol-water partition coefficient of the neutral species. |
| f<sub>u</sub> | % | 4.873 | Optimized; [Kaye 1989](#5) | Fraction unbound in plasma. |
| K<sub>m,CYP3A4</sub> | µmol/L | 4.7 | [Jornil 2010](#5) | Michaelis constant for CYP3A4-mediated metabolism. |
| k<sub>cat,CYP3A4</sub> | 1/min | 1.01 | Optimized; [Jornil 2010](#5) | Catalytic rate constant for CYP3A4-mediated metabolism. |
| K<sub>m,CYP2D6</sub> | µmol/L | 0.028 | [Jornil 2010](#5) | Activity-score-invariant Michaelis constant for CYP2D6-mediated metabolism. |
| k<sub>cat,CYP2D6</sub>, EM | 1/min | 1.3693020782 | Optimized; [Jornil 2010](#5) | Catalytic rate constant for the extensive-metabolizer pathway. |
| k<sub>cat,CYP2D6</sub>, PM | 1/min | 0 | Assumed; [Jornil 2010](#5) | Catalytic rate constant for the poor-metabolizer pathway. |
| CL<sub>hep</sub> | 1/min | 2.2538632474<sup>c</sup> | Optimized; [Jornil 2010](#5) | CYP2D6-independent hepatic clearance. |
| K<sub>i,CYP2D6</sub> | µmol/L | 0.16738 | Optimized; [Venkatakrishnan 2005](#5) | Inhibition constant for mechanism-based CYP2D6 inhibition. |
| k<sub>inact,CYP2D6</sub> | 1/min | 0.17 | [Venkatakrishnan 2005](#5) | Maximum CYP2D6 inactivation rate constant. |
| K<sub>i,CYP3A4</sub> | µmol/L | 4.48 | [Bertelsen 2003](#5) | Inhibition constant for mechanism-based CYP3A4 inhibition. |
| k<sub>inact,CYP3A4</sub> | 1/min | 0.011 | [Bertelsen 2003](#5) | Maximum CYP3A4 inactivation rate constant. |
| GFR fraction | - | 1 | Assumed | Fraction used to scale passive glomerular filtration. |
| Weibull shape | - | 7.17 | Optimized | Shape parameter for controlled-release dissolution. |
| t<sub>50</sub> | min | 276.35 | Optimized; [Chen 2015](#5); [Khatavkar 2013](#5) | Time to dissolve 50% of the controlled-release dose. |
| Partition coefficients | - | Rodgers and Rowland | Calculated; [Rodgers 2007](#5) | Tissue-to-plasma partition coefficients calculated with the Rodgers and Rowland method. |
| Cellular permeabilities | - | PK-Sim Standard | Calculated | Cellular permeabilities calculated with the PK-Sim Standard method. |
| P<sub>int</sub> | cm/min | 3.93 × 10<sup>−5</sup> | Optimized | Specific transcellular intestinal permeability. |

**Table 1:**<a name="table-1"></a> Drug-dependent physicochemical, distribution, metabolism, elimination, inhibition, and formulation parameters used in the final paroxetine model.

<sup>c</sup> The optimized snapshot value is retained. The supplement to [Rüdesheim 2022](#5) reports 1.37 1/min.

The CYP2D6 activity-score-specific catalytic rate constants implemented in the model are listed below.

| CYP2D6 AS | k<sub>cat</sub> [1/min] | Origin |
| ---: | ---: | --- |
| 0 | 0.00 | Assumed |
| 0.5 | 0.66 | Calculated |
| 0.75 | 1.08 | Calculated |
| 1 | 1.56 | Calculated |
| 1.25 | 2.11 | Calculated |
| 1.5 | 2.71 | Calculated |
| 2 | 4.09 | Optimized |
| 3 | 7.58 | Calculated |

**Table 1a:**<a name="table-1a"></a> CYP2D6 activity-score-specific k<sub>cat</sub> values for paroxetine metabolism from Table 2 of [Rüdesheim 2022](#5). The AS = 2 value was optimized, AS = 0 was assumed to have no CYP2D6 activity, and the other implemented values were calculated from the relative activity scale. AS: activity score.

### Clinical data

The evaluation uses 33 plasma concentration-time profiles from adults ([Table 2](#table-2)). Fourteen profiles were used for model building and 19 profiles were used for model verification. The assignments follow the training and test classifications in the published model supplement. For interaction studies, this report includes only paroxetine-only or control-arm pharmacokinetic data.

| Source | Dose [mg] / schedule\* | Age [years] | Weight [kg] | Sex | N | Form. | CYP2D6 characterization |
| --- | --- | --- | --- | --- | ---: | --- | --- |
| [Belle 2002](#5)<sup>+</sup> | 20 q.d., 12 days | 38 (20–49) | NR | 23% female | 22 | Tablet | EM |
| [Calvo 2004](#5) | 20 q.d., 15 doses | 26 | 64 | 64% female | 25 | NR | EM |
| [Chen 2015](#5) | 25 | 26 (19–45) | 64 | 25% female | 4 | Tablet CR | AS = 0.5 (IM) |
| [Chen 2015](#5) | 25 | 26 (19–45) | 61 | 45% female | 11 | Tablet CR | AS = 1 (IM) |
| [Chen 2015](#5) | 25 | 22 (19–45) | 58 | 60% female | 5 | Tablet CR | AS = 1.5 (NM) |
| [Chen 2015](#5) | 25 | 28 (19–45) | 61 | 25% female | 4 | Tablet CR | AS = 2 (NM) |
| [Lund 1982](#5)<sup>+</sup> | 23, intravenous infusion | 29 | 72 | Male | 1 | Solution | EM |
| [Lund 1982](#5)<sup>+</sup> | 28, intravenous infusion | 28 | 75 | Male | 1 | Solution | EM |
| [Lund 1982](#5)<sup>+</sup> | 28, intravenous infusion | 24 | 66 | Male | 1 | Solution | EM |
| [Lund 1982](#5)<sup>+</sup> | 28, intravenous infusion | 26 | 88 | Male | 1 | Solution | EM |
| [Lund 1982](#5)<sup>+</sup> | 45 | 28 | 75 | Male | 1 | NR | EM |
| [Lund 1982](#5)<sup>+</sup> | 45 | 24 | 66 | Male | 1 | NR | EM |
| [Lund 1982](#5)<sup>+</sup> | 45 | 26 | 88 | Male | 1 | NR | EM |
| [Lund 1982](#5)<sup>+</sup> | 45 | 29 | 72 | Male | 1 | NR | EM |
| [Massaroti 2005](#5)<sup>+</sup> | 20 | 28 (18–42) | 72 (57–87) | Male | 28 | Tablet | EM |
| [McClelland 1984](#5) | 70 | 31 (22–44) | NR | Male | 5 | NR | EM |
| [Mürdter 2016](#5) | 40 q.d., 3 days | 25 (22–26) | 62 (50–70) | Female | 3 | Tablet | AS = 0 (PM) |
| [Mürdter 2016](#5) | 40 q.d., 3 days | 24 (21–29) | 59 (56–64) | Female | 4 | Tablet | AS = 0.5 (IM) |
| [Mürdter 2016](#5) | 40 q.d., 3 days | 25 | 68 | Female | 1 | Tablet | AS = 0.75 (IM) |
| [Mürdter 2016](#5) | 40 q.d., 3 days | 26 (23–28) | 67 (64–74) | Female | 2 | Tablet | AS = 1 (IM) |
| [Mürdter 2016](#5)<sup>+</sup> | 40 q.d., 3 days | 32 (26–43) | 57 (48–64) | Female | 3 | Tablet | AS = 2 (NM) |
| [Mürdter 2016](#5) | 40 q.d., 3 days | 26 (22–28) | 62 (54–73) | Female | 3 | Tablet | AS = 3 (UM) |
| [Schoedel 2012](#5) | 20 q.d., 12 days | 34 (19–55) | 75 | 14% female | 14 | NR | EM |
| [Segura 2005](#5) | 20 q.d., 2 days | 23 | 65 | Male | 7 | Tablet | EM |
| [Sindrup 1992](#5)<sup>+</sup> | 30 q.d., 14 doses | 24 (20–30) | 73 (65–81) | Male | 9 | Tablet | EM |
| [Sindrup 1992](#5)<sup>+</sup> | 30 q.d., 14 doses | 27 (23–39) | 82 (68–95) | Male | 8 | Tablet | PM |
| [van der Lee 2007](#5) | 20 q.d., 10 days | 44 (18–64) | 69 (51–89) | 69% female | 26 | Tablet | EM |
| [Yasui-Furukori 2006](#5) | 20 | 25 (20–35) | 58 (46–75) | 25% female | 12 | NR | AS = 1.25 (NM) |
| [Yasui-Furukori 2007](#5) | 20 | 24 (21–35) | 57 (45–67) | 23% female | 13 | NR | EM |
| [Yoon 2000](#5) | 40 | 21 | 58 | Female | 1 | Tablet | AS = 0 (PM) |
| [Yoon 2000](#5) | 40 | 22 | 68 | Male | 3 | Tablet | AS = 0.5 (IM) |
| [Yoon 2000](#5) | 40 | 22 | 67 | Male | 6 | Tablet | AS = 1.25 (NM) |
| [Yoon 2000](#5)<sup>+</sup> | 40 | 23 | 59 | 17% female | 6 | Tablet | AS = 2 (NM) |

**Table 2:**<a name="table-2"></a> Clinical paroxetine concentration-time profiles used for model building and verification. \*: Single oral dose unless otherwise specified; AS: activity score; CR: controlled release; EM: extensive metabolizer; IM: intermediate metabolizer; NM: normal metabolizer; NR: not reported; PM: poor metabolizer; PT: predicted phenotype; q.d.: once daily; UM: ultrarapid metabolizer; <sup>+</sup>: data used for model building. Parenthetical PTs for AS-coded rows use the current CPIC CYP2D6 activity score-to-phenotype mapping ([Moore 2026](#5)). EM is the model default when study-specific CYP2D6 information is not available.
