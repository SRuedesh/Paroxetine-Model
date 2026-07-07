### 2.3.1 Absorption

The model includes intravenous infusion, immediate-release oral solution, oral tablet, and controlled-release oral applications. Intravenous simulations do not require an absorption process. Oral-solution and tablet simulations are represented with dissolved formulation input, while controlled-release simulations use a Weibull tablet formulation.

The value for `Specific intestinal permeability` and the solubility at pH 4.5 are summarized in Section 2.2.1. The controlled-release formulation is described by the `CR Weibull shape` and `CR Weibull time` parameters.

### 2.3.2 Distribution

Paroxetine is highly bound to plasma proteins. A value of 4.87% was used in this PBPK model for `Fraction unbound (plasma, reference value)` as summarized in Section 2.2.1.

An important parameter influencing the resulting volume of distribution is lipophilicity. A `Lipophilicity` value of 3.95 was used in the model as summarized in Section 2.2.1.

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation in PK-Sim.

### 2.3.3 Metabolism and Elimination

Two metabolic pathways and one residual hepatic clearance process were implemented into the model.

* CYP2D6

CYP2D6 metabolism is represented by Michaelis-Menten kinetics. CYP2D6 activity score-dependent k<sub>cat</sub> values are implemented as separate CYP2D6 processes. CYP2D6 k<sub>cat</sub> for AS=2 was optimized, AS=0 was set to zero, and intermediate or higher activity-score k<sub>cat</sub> values were calculated from the activity-score regression described by [Rüdesheim 2022](References.md).

* CYP3A4

CYP3A4 metabolism is represented by Michaelis-Menten kinetics using the K<sub>m</sub> and k<sub>cat</sub> values summarized in Section 2.2.1.

* Unspecific hepatic clearance

The model contains unspecific hepatic clearance. The Unspecific CL<sub>hep</sub> value reported by [Rüdesheim 2022](References.md) in the publication and supplement is erroneous. The value implemented in the model is correct.

Additionally, renal filtration is represented with a `GFR fraction` of 1. Mechanism-based inhibition processes for CYP2D6 and CYP3A4 are included using the K<sub>i</sub> and k<sub>inact</sub> values summarized in Section 2.2.1.

### 2.3.4 Automated Parameter Identification

The following parameters were optimized by fitting the model to the data:

| Model Parameter |
| --- |
| k<sub>cat</sub> (CYP3A4) |
| k<sub>cat</sub> (CYP2D6, AS=2) |
| K<sub>i</sub> (CYP2D6) |
| Unspecific CL<sub>hep</sub> |
| `CR Weibull shape` |
| `CR Weibull time` |
