# Pathogen_Persistance_AgSoil
This depository contains data and statistical analyses from a study on the persistence of enteric pathogens in agricultural soil.

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

### :memo: Citation
- If you use this repository, please cite the manuscript (currently under review).

### :file_folder: Code and Output
- `Obj2_modeling_NM081725.pdf`: Rendered R scripts and outputs supporting this research. 

## 📊 Data Files
The following data files are included in this repository and permanently archived on Zenodo [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.16230597.svg)](https://doi.org/10.5281/zenodo.16230597)
- `obj2_dat.RDS`: Triplicate microbial data collected during experiments.  
- `FAWN_report_2022_2025_daily.csv`: Average daily weather and soil data.  
- `FAWN_report_seven_day_hourly.csv`: Average hourly weather and soil data from 7 days before each sampling date.  

### 📊 Data Structure for Microbial Data

| Column Name        | Type        | Description |
|--------------------|-------------|-------------|
|`day`|Numerical|Sampling intervals in days
|`assay`|Categorical|The assays used for the quantification of each microbial target|
|`matrix`|Categorical|Microbe-suspended matrix to be studied|
|`microbe`|Categorical|Microbial groups|
|`replicate`|Numerical|Number of each biological replicate|
|`survival`|Numerical|Microbial survival
|`temp`|Categorical|Temperature in which the soil samples were incubated (set to 12ºC)|
|`week`|Numerical|Sampling intervals in weeks|
|`week_fac`|Categorical|Sampling intervals in weeks|

## :file_folder: Categorical Variables Levels for Microbial Data
|Category  | Levels        | Description        | Unit|
|----  |-----------|--------------------|-----|
|`assay`|`plate`|Total plate count| log<sub>10</sub> Colony-Forming Units (CFU)/g|
||`tcid50`|50% Tissue Culture Infectious Dose (TCID<sub>50</sub>)| log<sub>10</sub> TCID<sub>50</sub>/g|
||`pcr`|RNase RT-qPCR| log<sub>10</sub> Genome Copies (GC)/g|
|`matrix`|`p`|Soil samples without decaying plant materials, served as control sample|-|
||`ps`|Soil samples without decaying plant materials|-|
|`microbe`|`ec`|Enteric bacteria: _Escherichia coli_ TVS 353|-|
||`nv`|Enteric virus: Human norovirus GII (HuNoV GII)|-|
||`tv`|Enteric virus: Tulane virus (a surrogate for human norovirus)|-|

