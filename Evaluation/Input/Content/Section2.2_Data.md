### 2.2.1 In vitro and physicochemical data

The table below summarizes the drug-dependent inputs documented for the paroxetine model.

The Unspecific CL<sub>hep</sub> value reported by [Rüdesheim 2022](References.md) in the publication and supplement is erroneous. The value implemented in the model is correct.

| Parameter | Unit | Value | Source | Description |
| --- | ---: | ---: | --- | --- |
| MW | g/mol | 329.37 | Literature; [Zhong 2013](References.md) | Compound size used in concentration conversions. |
| pK<sub>a</sub> (base) | - | 9.9 | Literature; [Agrawal 2013](References.md) | Basic ionization constant. |
| Solubility (pH 4.5) | mg/mL | 7.31 | Literature; [Khatavkar 2016](References.md) | Solubility input. |
| logP | - | 3.95 | Literature; [Agrawal 2013](References.md) | Distribution input. |
| f<sub>u</sub> | % | 4.87 | Literature; [Kaye 1989](References.md) | Plasma binding input. |
| CYP3A4 K<sub>m</sub> | µmol/L | 4.7 | Literature; [Jornil 2010](References.md) | CYP3A4 affinity parameter. |
| CYP3A4 k<sub>cat</sub> | 1/min | 1.01 | Optimized; [Jornil 2010](References.md) | CYP3A4 metabolic capacity parameter. |
| CYP2D6 K<sub>m</sub> | µmol/L | 0.028 | Literature; [Jornil 2010](References.md) | CYP2D6 affinity held constant across activity scores. |
| CYP2D6 k<sub>cat</sub> EM | 1/min | 1.3693020782 | Optimized; [Jornil 2010](References.md) | activity-score-dependent CYP2D6 clearance. |
| CYP2D6 k<sub>cat</sub> PM | 1/min | 0 | Assumed; [Jornil 2010](References.md) | CYP2D6 poor-metabolizer activity set to zero. |
| Unspecific CL<sub>hep</sub> | 1/min | 2.2538632474 | Optimized; [Jornil 2010](References.md) | publication and supplement value is erroneous; model value retained |
| CYP2D6 K<sub>i</sub> | µmol/L | 0.16738 | Optimized; [Venkatakrishnan 2005](References.md) | Mechanism-based CYP2D6 inhibition parameter. |
| CYP2D6 k<sub>inact</sub> | 1/min | 0.17 | Literature; [Venkatakrishnan 2005](References.md) | Mechanism-based CYP2D6 inactivation parameter. |
| CYP3A4 K<sub>i</sub> | µmol/L | 4.48 | Literature; [Bertelsen 2003](References.md) | Mechanism-based CYP3A4 inhibition parameter. |
| CYP3A4 k<sub>inact</sub> | 1/min | 0.011 | Literature; [Bertelsen 2003](References.md) | Mechanism-based CYP3A4 inactivation parameter. |
| GFR fraction | - | 1 | Assumed | Passive glomerular filtration fraction. |
| CR Weibull shape | - | 7.17 | Optimized | Controlled-release formulation parameter. |
| CR Weibull time | min | 276.35 | Optimized; [Chen 2015](References.md); [Khatavkar 2013](References.md) | Controlled-release formulation parameter. |
| Partition coefficients | - | Diverse | Calculated; [Rodgers 2007](References.md) | Partition coefficient method. |
| Cellular permeabilities | cm/min | 0.28 | Calculated; [Kawai 1994](References.md) | Cellular permeability method. |
| Specific intestinal perm. | cm/min | 3.93E-05 | Calculated; [Kawai 1994](References.md) | Oral absorption parameter. |

### 2.2.2 Clinical data

The evaluation uses 35 observed-data profiles for paroxetine in peripheral venous blood plasma. The evaluation plan assigns 14 simulations to model building and 19 simulations to model verification.

Model-building clinical data:

| Publication | Arm / Treatment / Information used for model building |
| --- | --- |
| [Lund 1982](References.md) | Plasma PK profiles in adults after intravenous infusion, single dose and oral, single-dose administration of 28 mg, 23 mg, 45 mg doses paroxetine. |
| [Belle 2002](References.md) | Plasma PK profiles in adults after oral tablet, once daily administration of 20 mg paroxetine with CYP2D6 g-EM status. |
| [Massaroti 2005](References.md) | Plasma PK profiles in adults after oral tablet, single-dose administration of 20 mg paroxetine. |
| [Mürdter 2016](References.md) | Plasma PK profiles in adults after oral tablet, single-dose administration of 40 mg paroxetine with CYP2D6 AS = 2 status. |
| [Sindrup 1992](References.md) | Plasma PK profiles in adults after oral tablet, once daily administration of 30 mg paroxetine with CYP2D6 p-PM, p-EM status. |
| [Yoon 2000](References.md) | Plasma PK profiles in adults after oral tablet, single-dose administration of 40 mg paroxetine with CYP2D6 AS = 2 status. |

Model-verification clinical data:

| Publication | Arm / Treatment / Information used for model verification |
| --- | --- |
| [Calvo 2004](References.md) | Plasma PK profiles in adults after oral, once daily administration of 20 mg paroxetine. |
| [McClelland 1984](References.md) | Plasma PK profiles in adults after oral, single-dose administration of 70 mg paroxetine. |
| [Schoedel 2012](References.md) | Plasma PK profiles in adults after oral, once daily administration of 20 mg paroxetine. |
| [Segura 2005](References.md) | Plasma PK profiles in adults after oral tablet, once daily administration of 20 mg paroxetine with CYP2D6 p-EM status. |
| [van der Lee 2007](References.md) | Plasma PK profiles in adults after oral tablet, once daily administration of 20 mg paroxetine with CYP2D6 g-EM status. |
| [Yasui-Furukori 2006](References.md) | Plasma PK profiles in adults after oral, single-dose administration of 20 mg paroxetine with CYP2D6 AS = 1.25 status. |
| [Yasui-Furukori 2007](References.md) | Plasma PK profiles in adults after oral, single-dose administration of 20 mg paroxetine. |
| [Chen 2015](References.md) | Plasma PK profiles in adults after oral controlled release, single-dose administration of 25 mg paroxetine with CYP2D6 AS = 0.5, AS = 1.0, AS = 1.5, AS = 2 status. |
| [Mürdter 2016](References.md) | Plasma PK profiles in adults after oral tablet, single-dose administration of 40 mg paroxetine with CYP2D6 AS = 0, AS = 0.5, AS = 0.75, AS = 1, AS = 3 status. |
| [Yoon 2000](References.md) | Plasma PK profiles in adults after oral tablet, single-dose administration of 40 mg paroxetine with CYP2D6 AS = 0, AS = 0.5, AS = 1.25 status. |
