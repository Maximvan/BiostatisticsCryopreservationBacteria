# BiostatisticsCryopreservationBacteria
Investigating the impact of cryopreservation on the survival of bacteria as part of the Biostatistics course at Ghent University

## Introduction
Ghent University's Laboratory of Microbiology is conducting the Mibirem project, an experimental study, aiming to optimize the preservation of microbial consortia. The preservation methods under evaluation involve lyophilization at room temperature using two distinct techniques (LYO1 and LYO2) and storage at ultra-low temperatures, either -80 °C (CRYO1) or -196 °C (CRYO2). Simultaneously, seven different preservation media labeled as A, B, C (cryopreservationD), and D, E, F, G (lyophilization) are being tested. Fourteen scenarios, combining different preservation methods (lyophilization and cryopreservation) and media types, are being tested.

To assess the survival rates of microbial consortia under these varied conditions, the researchers collect samples at different time points: 0, 3, 6, 12, 18, 24, and 30 months after initiating storage, with time point 0 representing the moment before storage. The primary focus is on the initial measurement and the 3-month time point, and for each scenario, five tubes containing the microbial consortium are stored for subsequent flow cytometry analysis.

Flow cytometry, a rapid, reproducible, and cost-effective technique, is employed to quantify total bacterial numbers and assess the live/dead ratio of bacterial cells. The researchers have compiled four distinct datasets, capturing the percentage of live, injured, and dead bacteria in each sample, along with the total number of bacterial cells. Each sample undergoes three measurements for each parameter.

In this project, the central research question is: Does the CRYO2 preservation method have an effect over time on stored samples, and does this effect vary across different preservation media?

## Conclusion
The gaussian generalized linear model revealed that there is an extremely significant (p < 0.001) difference of the survival of the bacteria between timepoint zero months and after timepoint 3 months using any of the preservation media.

The percentage of bacteria after three months of storage using the CRYO2 method in any of the preservation media decreases on average for 9.860% (95% CI [14.52444, 5.195565], p = 0.000611 < 0.001). On average, the predicted percentage of living bacteria before storage is 74.479% (95% CI [70.43981, 78.518853], p = 2e-16 < 0.001) and after 3 months of storage 64.619% of living bacteria are expected.

Furthermore, three other gaussian generalized linear model revealed that there is also an extremely significant (p < 0.001) difference on the survival of the bacteria between timepoint zero months and timepoint 3 months when stored in medium A and B. While there is only a significant (p < 0.05) difference when stored in medium C.

When the bacteria are stored for three months using the CRYO2 method in preservation medium A, B and C, there is on average a decrease of 8.743% (95% CI [11.09933, 6.387341], p = 8.61e-05 < 0.001), 9.250% (95% CI [12.29811, 6.20189], p = 0.000343 < 0.001) and 11.587% (95% CI [18.99344, 4.179891], p = 0.0154 < 0.05) of living bacteria respectively. For all the preservation media, the predicted percentage of living bacteria before storage is on average 74.479% (A: 95% CI [72.81340, 76.145273], p = 3.21e-13 < 0.001; B: 95% CI [72.32399, 76.63467], p = 2.51e-12 < 0.001; C: 95% CI [69.24195, 79.716714], 2.96e-09 < 0.001). For preservation medium A, B and C, on average, the expected percentage of living bacteria after three months of storage is 65.736%, 65.229% and 62.892%.

The results derived from the Gaussian Generalized Linear Models suggest that, on average, preservation medium A performs better than medium B and C, as it exhibits a higher percentage of bacterial survival. However, to make this statement, additional information from the later time points is essential.

![Conclusion Figure](https://i.ibb.co/fFbZKb7/finalplot.png)

The plot above visually emphasizes the observed differences in bacterial survival percentages before and after three months of storage using the CRYO2 method in various preservation media.

The larger p value and wider confidence interval for medium C are consistent with the observed data, where points are dispersed from 50% to 75% live bacteria. This dispersion highlights a higher variance in medium C, suggesting potential instability in bacterial survival percentages. Higher variance may imply less consistent outcomes, raising considerations about the reliability of the preservation method in medium C.

Secondly, for medium A, the narrower confidence interval and smaller variance, as evident in the ridgeline plot's narrower peak, suggest a more stable pattern of bacterial survival. The decreased average of 8.743% in medium A, as indicated by the Gaussian Generalized Linear Model, is the lowest among the mediums, further emphasizing its stability in preserving bacteria over three months with the CRYO2 method.

However, when considering medium B, despite a peak that appears higher than medium A in the raw data, the Gaussian Generalized Linear Model's average decrease doesn't fully reflect this. This difference can be attributed to the elevated variance in medium B, manifesting as a secondary peak around 60%, influencing the calculated average decrease and confidence interval from the model. 
