# COVID-19_Role_of_age
Code for: How asymptomatic SARS CoV-2 infection varies by demographics   

## Citation

How asymptomatic SARS CoV-2 infection varies by demographics   

…………

## Abstract

It is clear that asymptomatic individuals carrying SARS CoV-2 can transmit the virus and contribute to outbreaks of COVID-19  , but it is not yet clear how the proportion of asymptomatic infections varies by age and geographic location. Here we use detailed surveillance data gathered during COVID-19 resurgences in six cities of China at the beginning of 2021 to investigate this question. Data were collected in Chinese cities by multiple rounds of city-wide PCR testing with detailed contact tracing, where each patient was monitored for symptoms through the whole course of infection. Based on the data from China,   we find that the proportion of asymptomatic infections declines with age (coefficient =-0.006, P<0.01), falling from 56% in age group 0–9 years to 12% in age group >60 years. Using an age-stratified compartment model,     we show that an age-dependent asymptomatic pattern and age distribution of cases explain most  of the differences between locations in reported asymptomatic proportions. Combined with demographics and contact matrices from other cities worldwide  ,   we estimate that a maximum of 22%–55%     of COVID-19 cases would be generated by infections from asymptomatic cases in an uncontrolled epidemic. Our analysis suggests that risk of COVID-19 flare-ups are likely if only adults are vaccinated and that some age-balanced vaccination will be needed in the future.

## Notes on the code

To run, you need a Matlab toolbox called "DRAM": DRAM is a combination of two ideas for improving the efficiency of Metropolis-Hastings type Markov chain Monte Carlo (MCMC) algorithms, Delayed Rejection and Adaptive Metropolis. This page explains the basic ideas behind DRAM and provides examples and Matlab code for the computations.(see http://helios.fmi.fi/~lainema/dram/)

About code folder:

About code folder: We used three code folders to estimate the parameters for Tonghua, Changchun and Xingtai, respectively. For each folder: main file 1 (fitting the model): f1.m; function dependencies:f2.m,f3.m,f4.m; The setting of the fixed parameters for each city can be found in the main text and supplemented material.

The code to simulate the scenarios can be found in the Tonghua folder: main file 2: f_simu2.m; function dependencies:fsimu_deterministic.m,fsimu_P_deterministic.m,fsimu_MiddleSize_deterministic.m,fsimu_runFromMiddle_deterministic.m,fsimu_Vaccine_deterministic.m,fsimu_Vaccine_deterministic_asym.m; Note that do not run this file directly since running time is quite long.




## Data

### Epidemiological data

We collected the daily official case reports from the health commission of 2 provincial-level administrative units and 3 city-level units, the website’s links are provided. The information was collected by Bingying Li.

### Population-level testing strategy

We prepared the population-testing strategy files (for example: population_testing_strategy_break0.xlsx. "break0" represents the break interval is 0 day.). Each column represents one popualtion-level testing strategy.
