# Evaluation Analysis of MOVES Data
Repository for analysis and visualization of MOVES emissions data.
# Overview
### Data
This repository uses data collected from U.S. Environmental Protection Agency using Motor Vehicle Emissions Simulation tool (MOVES). There are two datasets named "all_countiesby16.csv" and "cleaned_c02_data_non_va_wv.csv" respectively. The first is raw data collected using the EPA's Motor Vehicle Emissions Simulation Tool alongside estimated inputs. The second is the processed data after removing the extreme data from Virginia and West Virginia and filling in missing data. The "evaluation_analysis.py" file contains functions to generate histograms of emissions in different years as well as plots of aggregate emissions over time under different scenarios.
### Generating Plots
The "evaluation_analysis.ipynb" file is a notebook that contains python code for generating plots based on the cleaned data mentioned above. It generates two types of plots: charts of aggregate emissions over time with different numbers of top carbon emitters making credible commitments as well as histograms of emissions levels during a specific year alongside 2005 and 50% of 2005 aggregate emissions as benchmarks. The current emissions reductions per year is based on the Long Term Strategy of the United States but can easily be edited by the user. In the plots we assume that all counties with non-credible carbon commitments continue to emit as predicted by MOVES. There are two types of these plots --one that assumes that credible climate action begins in 2005 and another that assumes that credible commitments begin in 2025.

The histogram plots the distribution of CO2 emissions levels in the dataset. It also fits a log-normal distribution to the data using the scipy.stats library. 





