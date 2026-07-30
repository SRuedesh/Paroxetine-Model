The PBPK model for paroxetine was developed and verified with clinical pharmacokinetic data after intravenous and oral administration. The evaluation covers immediate-release and controlled-release applications, single-dose and repeated-dose regimens, and a dose range of 20 to 70 mg. The clinical dataset also includes CYP2D6 poor-metabolizer, extensive-metabolizer, and activity-score stratified groups, which are central to the intended use of the model.

The model was built with data supporting distribution, oral absorption, CYP2D6-dependent clearance, CYP2D6-independent clearance, and controlled-release dissolution. Intravenous data from [Lund 1982](#5) supported systemic disposition independent of oral absorption. Oral data from [Belle 2002](#5), [Massaroti 2005](#5), [Mürdter 2016](#5), [Sindrup 1992](#5), and [Yoon 2000](#5) supported oral absorption, repeated-dose behavior, and CYP2D6 activity-score-dependent clearance. Verification used independent immediate-release and controlled-release oral studies, including [Chen 2015](#5), [McClelland 1984](#5), [Schoedel 2012](#5), [Segura 2005](#5), [van der Lee 2007](#5), and [Yasui-Furukori 2006](#5).

The model quantifies CYP2D6- and CYP3A4-mediated metabolism, unspecific hepatic clearance, and passive renal filtration. The CYP2D6 activity-score implementation is the major driver for differences between poor-, intermediate-, extensive-, and higher-activity groups. CYP3A4 metabolism and unspecific hepatic clearance provide additional clearance capacity.

The next sections show:

1. the final model input parameters for the building blocks: [Section 3.1](#31).
2. the overall goodness of fit: [Section 3.2](#32).
3. simulated vs. observed concentration-time profiles for the clinical studies used for model building and for model verification: [Section 3.3](#33).

The concentration-time profiles should be interpreted by study context. Intravenous profiles mainly test distribution and systemic clearance. Immediate-release oral profiles test the combined absorption and first-pass components. Controlled-release profiles additionally test the Weibull dissolution parameters. CYP2D6 poor-metabolizer and low-activity-score profiles are particularly informative for CYP2D6-independent clearance.
