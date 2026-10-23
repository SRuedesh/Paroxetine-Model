### Absorption

The model includes intravenous infusion, immediate-release oral solution, oral tablet, and controlled-release oral applications. Intravenous simulations do not require an absorption process. Oral-solution and tablet simulations are represented with dissolved formulation input, while controlled-release simulations use a Weibull tablet formulation.

The value for `Specific intestinal permeability` and the solubility at pH 4.5 are summarized in Section 2.2.1. The controlled-release formulation is described by the `CR Weibull shape` and `CR Weibull time` parameters.

### Distribution

Paroxetine is highly bound to plasma proteins. The literature starting value for `Fraction unbound (plasma, reference value)` was 5.00% ([Kaye 1989](#5)). The value was optimized to 4.873% in the PBPK model.

An important parameter influencing the resulting volume of distribution is lipophilicity. A `Lipophilicity` value of 3.95 was used in the model as summarized in Section 2.2.1.

Partition coefficients were calculated with the Rodgers and Rowland method. Cellular permeabilities were calculated with the PK-Sim Standard method.

### Metabolism and elimination

Two metabolic pathways and one residual hepatic clearance process were implemented into the model.

* CYP2D6

CYP2D6 metabolism is represented by Michaelis-Menten kinetics. Two CYP2D6 parameter sets are used. Study arms with an EM phenotype, reported or model default, use the EM k<sub>cat</sub> ([Table 1](#table-1)). Study arms with a reported activity score use separate activity-score CYP2D6 processes ([Table 1a](#table-1a)). The EM k<sub>cat</sub> and the AS = 2 k<sub>cat</sub> were optimized, the AS = 0 value was set to zero, and the other activity-score values were calculated from the regression described by [Rüdesheim 2022](#5). The EM k<sub>cat</sub> is 35% lower than the AS = 1.25 k<sub>cat</sub>. [Rüdesheim 2022](#5) attributes this difference to the often arbitrary definition of the EM phenotype. Exceptions: the [Yasui-Furukori 2007](#5) arm has no reported CYP2D6 data and uses the AS = 1.25 k<sub>cat</sub>. The phenotyped EM arm of [Sindrup 1992](#5) uses the AS = 2 k<sub>cat</sub>.

* CYP3A4

CYP3A4 metabolism is represented by Michaelis-Menten kinetics using the K<sub>m</sub> and k<sub>cat</sub> values summarized in Section 2.2.1.

* Unspecific hepatic clearance

The model contains optimized unspecific hepatic clearance as summarized in Section 2.2.1.

Additionally, renal filtration is represented with a `GFR fraction` of 1. Mechanism-based inhibition processes for CYP2D6 and CYP3A4 are included using the K<sub>i</sub> and k<sub>inact</sub> values summarized in Section 2.2.1.
