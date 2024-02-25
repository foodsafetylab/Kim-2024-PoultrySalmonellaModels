# Kim-2024-PoultrySalmonellaModels

## Overview
_Salmonella_ prevalence has reduced in U.S. raw poultry products since adopting prevalence-based _Salmonella_ performance standards, but human illnesses did not reduce proportionally. To determine better indicators of risk, we used Quantitative Microbial Risk Assessment (QMRA) to evaluate public health risks of raw chicken parts contaminated with different levels of (1) all _Salmonella_ and (2) _Salmonella_ serotypes of interest. Lognormal _Salmonella_ level distributions were fitted using data from 2012 USDA-FSIS Baseline Survey ("Baseline") and 2023 USDA-FSIS routine verification sampling ("HACCP") data. Three different dose-response (DR) models were used to explore the public health risk of _Salmonella_ levels and serotypes: (1) Single DR for all serotypes; (2) Reduced virulence for Kentucky; (3) Multiple serotype-specific DR models. All scenarios indicated concentrated risk in a relatively small proportion of products contaminated with high-levels of _Salmonella_. Our simplest approach using a single DR model with Baseline data (μ=-3.19, σ=1.29) showed that 68% and 37% of illnesses were attributed to the 0.7% and 0.06 % of products above 1 CFU/g and 10 CFU/g _Salmonella_, respectively. More recent HACCP data (μ=-4.85, σ=2.44) showed that 99.9% and 99.6% of illnesses were attributed to the 2.3% and 0.8 % of products above 1 CFU/g and 10 CFU/g _Salmonella_, respectively. The scenarios with serotype-specific DR models showed more concentrated risk at higher levels than the simpler approaches at all levels. Baseline data showed 91.5% and 63.7% and HACCP data showed >99.9% and 99.9% of illnesses were attributed to products above 1 and 10 CFU/g _Salmonella_, respectively. Regarding serotypes, 0.003% and 0.3% of illnesses were attributed to the 0.2% and 0.7% of products with > 1 CFU of Kentucky/g, while 69% and 78.7% of illnesses were attributed to the 0.3% and 1.2% of products above 1 CFU/g containing either Enteritidis, Infantis, or Typhimurium for Baseline and HACCP data, respectively. Our risk assessment suggests public health risk in chicken parts is concentrated in the small proportion of finished products contaminated with high-levels and specifically high-levels of high-risk serotypes. Low-risk serotypes, such as Kentucky, are predicted to contribute to extremely few human cases.

## Usage
### Data Generation
Simulation-produced data can be generated from the models, files used in the associated publication can be [downloaded from Box](https://uofi.box.com/s/r7p3hoty6ymlomipav1xbgzv2p3rf8dy) due to GitHub file size limitations.

### Setup
Data fitting was performed in [R 3.4.2](https://cloud.r-project.org/) and [RStudio Desktop](https://posit.co/download/rstudio-desktop/) with the following packages:
* readxl
* rjags using [JAGS 4.3.1](https://mcmc-jags.sourceforge.io/)
* fitdistrplus
* stringr
* pastecs
* knitr
* MASS

 @Risk models were run using [@Risk 8.1](https://lumivero.com/products/at-risk/), R-based models were run in R 3.4.2 with RStudio Desktop with the following packages:
 * readxl
* parallel
* plyr
* dplyr
* MASS
* BAS
* Rmpfr

### Running
Risk models are located in data and /models/risk models.

@Risk models can be run by launching the respective .xlsx file through Microsoft Office Excel and @Risk.

R models can be run by opening the Risk Model.Rproj file, followed by "Unified Risk Function.Rmd" and running the required code chunks.

## Authors
You can view the list of authors in the [AUTHORS](/AUTHORS) file.

## Contact
Corresponding author: Matthew J. Stasiewicz<br>
103 Agricultural Bioprocess Lab<br>
1302 W. Pennsylvania<br>
Urbana, IL, 1361801<br>
USA<br>
+1-217-265-0963<br>
[mstasie@illinois.edu](mailto:mstasie@illinois.edu)

## Citation
TO DO: Update following publication

## License
This project's code is licensed under the GNU General Public License v3.0 and dataset is licensed the Creative Commons Attribution Share Alike 4.0 International license. Please see the [LICENSE.code](/LICENSE.code) and [LICENSE.dataset](/LICENSE.dataset) files for details.

## Acknowledgements
Both Stasiewicz and Wiedmann are members of a Coalition for Poultry Safety Reform which includes volunteer members from the poultry industry, consumer groups, and academics.

## Funding
This study was supported by a US Poultry and Egg Association grant to Stasiewicz and Wiedmann, for Project #BRF-015 Risk Assessment Comparing Alternative Approaches to Regulating _Salmonella_ in Poultry by Public Health Impact Factors.
