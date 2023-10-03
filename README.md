# VIBRANT

© 2023 The Trustees of Columbia University in the City of New York.  The codes and data in this work may be reproduced, distributed, and otherwise exploited for academic non-commercial purposes only.  To obtain a license to the codes and data in this work for commercial purposes, please contact Columbia Technology Ventures at techventures@columbia.edu.

This is the github repository for the paper VIBRANT: biochemical profiling for single-cell drug responses. 

## Abstract
The measurement of single-cell drug responses is important to drug discovery, as it facilitates understanding drug mechanism of action (MoA), evaluating drug efficacy, overcoming drug resistance and optimizing drug therapy. Despite its importance, a suitable method satisfying the requirements of high throughput, high content and low instrument cost is still lacking. Here, we present a new high-content biochemical profiling method named Vibrational Painting (VIBRANT), which integrates vibrational imaging, multiplexed vibrational probes and optimized data analysis pipeline for measuring single-cell drug responses. Three infrared-active vibrational probes were designed to measure general but distinct metabolic activities in human cancer cells. More than 20,000 single-cell drug response data were collected, corresponding to 23 different drug treatments. The resulting biochemical profile is highly sensitive to drug-perturbed cell phenotypes. Utilizing this property, we built a machine learning classifier to predict drug MoAs at single-cell level with high accuracy and minimal batch effects, which is difficult for other methods. We further designed a novelty detection algorithm to discover drug candidates with novel MoAs and evaluate drug combinations. Overall, VIBRANT has demonstrated great potential across multiple key areas of phenotypic screening, establishing it as a promising approach for advancing drug discovery.

## Requirements
The code was implemented in python 3.7.

## Data
Processed single-cell infrared spectrum data of all the drug treatments is avilable in VIBRANT_data, named as "SingleCellSpec_alldrug.mat". For each drug treatment, its corresponding single cell spectrum is named as "CELL_SPEC_ALL_" + "drugname". The wavenumber matrix ("wave_all.mat") is also provided in this data to indicate the wavenumber location of each vibrational peak in the infrared spectrum.

## Codes
The main codes for data preprocessing, predicting drug MoAs using machine learning and identifying test compounds with novel MoAs using novelty detection are included in VIBRANT_MainCodes.ipynb.
