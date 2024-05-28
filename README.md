# Kim-2024-PoultrySalmonellaModels

## Overview
_Salmonella_ prevalence declined in U.S. raw poultry products since adopting prevalence-based _Salmonella_ performance standards, but human illnesses did not reduce proportionally. We used Quantitative Microbial Risk Assessment (QMRA) to evaluate public health risks of raw chicken parts contaminated with different levels of all _Salmonella_ and specific high- and low-virulence serotypes. Lognormal _Salmonella_ level distributions were fitted to 2012 USDA-FSIS Baseline parts survey and 2023 USDA-FSIS HACCP verification sampling data. Three different Dose-Response (DR) approaches included (i) a single DR for all serotypes, (ii) DR that reduces _Salmonella_ Kentucky ST152 virulence, and (iii) multiple serotype-specific DR models. All scenarios found risk concentrated in the few products with high _Salmonella_ levels. Using a single DR model with Baseline data (μ = −3.19, σ = 1.29 Log CFU/g), 68% and 37% of illnesses were attributed to the 0.7% and 0.06% of products with >1 and >10 CFU/g _Salmonella_, respectively. Using distributions from 2023 HACCP data (μ = −5.53, σ = 2.45), 99.8% and 99.0% of illnesses were attributed to the 1.3% and 0.4% of products with >1 and >10 CFU/g _Salmonella_, respectively. Scenarios with serotype-specific DR models showed more concentrated risk at higher levels. Baseline data showed 92% and 67% and HACCP data showed >99.99% and 99.96% of illnesses attributed to products with >1 and >10 CFU/g _Salmonella_, respectively. Regarding serotypes using Baseline or HACCP input data, 0.002% and 0.1% of illnesses were attributed to the 0.2% and 0.4% of products with >1 CFU/g of Kentucky ST152, respectively, while 69% and 83% of illnesses were attributed to the 0.3% and 0.6% of products with >1 CFU/g of Enteritidis, Infantis, or Typhimurium, respectively. Therefore, public health risk in chicken parts is concentrated in finished products with high levels and specifically high levels of high-virulence serotypes. Low-virulence serotypes like Kentucky contribute few human cases.

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
Kim, M., Barnett-Neefs, C., Chavez, R. A., Kealey, E., Wiedmann, M., & Stasiewicz, M. J. 2024. Risk assessment predicts most of the salmonellosis risk in raw chicken parts is concentrated in those few products with high-levels of high-virulence serotypes of _Salmonella_. _Journal of Food Protection_, 100304. https://doi.org/10.1016/j.jfp.2024.100304.

## License
This project's code is licensed under the GNU General Public License v3.0 and dataset is licensed the Creative Commons Attribution Share Alike 4.0 International license. Please see the [LICENSE.code](/LICENSE.code) and [LICENSE.dataset](/LICENSE.dataset) files for details.

## Acknowledgements
Both Stasiewicz and Wiedmann are members of a Coalition for Poultry Safety Reform which includes volunteer members from the poultry industry, consumer groups, and academics.

## Funding
This study was supported by a US Poultry and Egg Association grant to Stasiewicz and Wiedmann, for Project #BRF-015 Risk Assessment Comparing Alternative Approaches to Regulating _Salmonella_ in Poultry by Public Health Impact Factors.
