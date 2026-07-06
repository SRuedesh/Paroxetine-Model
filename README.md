# Paroxetine-Model
Whole-body PBPK model of paroxetine including CYP2D6 drug-gene interactions.

This repository contains the paroxetine model published by Rüdesheim et al. [[1](#references)].

## Original publication
[S Rüdesheim, D Selzer, T Mürdter, S Igel, R Kerb, M Schwab, T Lehr. Physiologically Based Pharmacokinetic Modeling to Describe the CYP2D6 Activity Score-Dependent Metabolism of Paroxetine, Atomoxetine and Risperidone. Pharmaceutics, 2022;14:1734.](https://doi.org/10.3390/pharmaceutics14081734)

This paroxetine model is intended to describe CYP2D6 activity score-dependent paroxetine pharmacokinetics and to support CYP2D6 drug-gene interaction simulations.

The model was developed and evaluated using published clinical plasma pharmacokinetic data after intravenous or oral paroxetine administration by Lund et al. [[2](#references)], Sindrup et al. [[3](#references)], Yoon et al. [[4](#references)], Belle et al. [[5](#references)], Massaroti et al. [[6](#references)], Mürdter et al. [[7](#references)], Calvo et al. [[8](#references)], Chen et al. [[9](#references)], McClelland and Raptopoulos [[10](#references)], Schoedel et al. [[11](#references)], Segura et al. [[12](#references)], van der Lee et al. [[13](#references)] and Yasui-Furukori et al. [[14](#references), [15](#references)].

The presented model includes the following features:

- metabolism by CYP2D6,
- metabolism by CYP3A4,
- unspecific hepatic clearance,
- renal filtration,
- mechanism-based inhibition of CYP2D6 and CYP3A4,
- oral absorption for immediate-release and controlled-release formulations.

## Model note
The unspecific hepatic clearance value reported by Rüdesheim et al. in the publication and supplement [[1]](https://doi.org/10.3390/pharmaceutics14081734) is erroneous. The value implemented in the model is correct.

## Repository files
This repository contains:

- a [PK-Sim snapshot (*.json) file](https://docs.open-systems-pharmacology.org/working-with-pk-sim/pk-sim-documentation/importing-exporting-project-data-models#exporting-project-to-snapshot-loading-project-from-snapshot) of the current PBPK model
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (evaluation_plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

**The latest release of the snapshot of the model, the evaluation plan and the static content can be found in the [latest release in this repository](./releases/latest).**

**The latest release of the PK-Sim project model file and the respective evaluation report can be found in the [latest OSP PBPK Model Library release](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/releases/latest).**

## Code of conduct
Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution
We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License
The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References
[1] [S Rüdesheim, D Selzer, T Mürdter, S Igel, R Kerb, M Schwab, T Lehr. Physiologically Based Pharmacokinetic Modeling to Describe the CYP2D6 Activity Score-Dependent Metabolism of Paroxetine, Atomoxetine and Risperidone. Pharmaceutics, 2022;14:1734.](https://doi.org/10.3390/pharmaceutics14081734)

[2] [J Lund, P Thayssen, H Mengel, O L Pedersen, C B Kristensen, L F Gram. Paroxetine: Pharmacokinetics and Cardiovascular Effects after Oral and Intravenous Single Doses in Man. Acta Pharmacol Toxicol, 1982;51:351-357.](https://pubmed.ncbi.nlm.nih.gov/6217723/)

[3] [S H Sindrup, K Brøsen, L F Gram, J Hallas, E Skjelbo, A Allen, G D Allen, S M Cooper, G Mellows, T C Tasker, et al. The relationship between paroxetine and the sparteine oxidation polymorphism. Clin Pharmacol Ther, 1992;51:278-287.](https://pubmed.ncbi.nlm.nih.gov/1531950/)

[4] [Y R Yoon, I J Cha, J H Shon, K A Kim, Y N Cha, I J Jang, C W Park, S G Shin, D A Flockhart, J G Shin. Relationship of paroxetine disposition to metoprolol metabolic ratio and CYP2D6*10 genotype of Korean subjects. Clin Pharmacol Ther, 2000;67:567-576.](https://pubmed.ncbi.nlm.nih.gov/10824636/)

[5] [D J Belle, C S Ernest, J M Sauer, B P Smith, H R Thomasson, J W Witcher. Effect of potent CYP2D6 inhibition by paroxetine on atomoxetine pharmacokinetics. J Clin Pharmacol, 2002;42:1219-1227.](https://pubmed.ncbi.nlm.nih.gov/12412820/)

[6] [P Massaroti, N M Cassiano, L F Duarte, J Pedrazzoli. Validation of a selective method for determination of paroxetine in human plasma by LC-MS/MS. J Pharm Pharm Sci, 2005;8:340-347.](https://sites.ualberta.ca/~csps/JPPS8%282%29/E.Meurer/paroxetine.htm)

[7] [T Mürdter, et al. Impact of CYP2D6 genotype and co-medication with paroxetine and clarithromycin on clomiphene metabolism in vivo. Naunyn-Schmiedeberg's Arch Pharmacol, 2016;389:8.](https://clinicaltrials.gov/study/NCT01289756)

[8] [G Calvo, et al. Lack of pharmacologic interaction between paroxetine and alprazolam at steady state in healthy volunteers. J Clin Psychopharmacol, 2004;24:268-276.](https://doi.org/10.1097/01.jcp.0000125681.30544.bf)

[9] [R Chen, H Wang, J Shi, K Shen, P Hu. CYP2D6 genotype affects controlled-release paroxetine pharmacokinetics in healthy Chinese subjects. Eur J Clin Pharmacol, 2015;71:835-841.](https://doi.org/10.1007/s00228-015-1863-8)

[10] [G R McClelland, P Raptopoulos. EEG and blood level of paroxetine after a single oral dose to normal volunteers. Psychopharmacology, 1984;83:327-329.](https://doi.org/10.1007/BF00428542)

[11] [K A Schoedel, L E Pope, E M Sellers. Randomized open-label drug-drug interaction trial of dextromethorphan/quinidine and paroxetine in healthy volunteers. Clin Drug Investig, 2012;32:157-169.](https://doi.org/10.2165/11596910-000000000-00000)

[12] [M Segura, et al. Contribution of CYP2D6 to MDMA disposition in humans: use of paroxetine as metabolic inhibitor probe. Clin Pharmacokinet, 2005;44:649-660.](https://doi.org/10.2165/00003088-200544060-00007)

[13] [M J van der Lee, et al. Interaction study of paroxetine and fosamprenavir-ritonavir in healthy subjects. Antimicrob Agents Chemother, 2007;51:4098-4104.](https://doi.org/10.1128/AAC.00421-07)

[14] [N Yasui-Furukori, et al. Terbinafine increases plasma concentration of paroxetine after single oral administration. Eur J Clin Pharmacol, 2006;63:51-56.](https://doi.org/10.1007/s00228-006-0219-7)

[15] [N Yasui-Furukori, et al. Effect of itraconazole on pharmacokinetics of paroxetine. Ther Drug Monit, 2007;29:45-48.](https://doi.org/10.1097/FTD.0b013e3180307e48)
