# Pathogen_Persistance_AgSoil
This depository contains collected data and statistical analyses associated with the study on the persistence of enteric pathogens in agricultural soil. This work is licensed under the [Creative Commons CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).

### :memo: Manuscript: TBA

### :file_folder: Code and Output

- `Obj2_modeling_NM081725.pdf`: Rendered R scripts and statistical outputs supporting this research.

## 📊 Data Files

- `obj2_dat.RDS`: Microbial data collected from the experiments.
- `FAWN_report_2022_2025 daily.csv`: Average daily weather/soil data.
- `FAWN_report_seven_day_hourly.csv`: Average hourly weather/soil data, 7 days before the sampling date.

All the files are archived on Zenodo: [https://doi.org/10.5281/zenodo.16230597](https://doi.org/10.5281/zenodo.16230597)

### 📊 Data Structure for microbial data

| Column Name        | Type        | Description |
|--------------------|-------------|-------------|
|day|Numerical|Sampling intervals in days
|assay|Categorical|The assays used for the quantification of each microbial target|
|matrix|Categorical|Microbe-suspended matrix to be studied|
|microbe|Categorical|Microbial groups|
|replicate|Numerical|Number of each biological replicate|
|survival|Numerical|Microbial survival
|temp|Categorical|Temperature in which the soil samples were incubated (set to 12ºC)|
|week|Numerical|Sampling intervals in weeks|
|week_fac|Categorical|Sampling intervals in weeks|
|month|Numerical|month|
|year|Numerical|year|
|meanTemp|Numerical|Average daily temperature (ºF)|
|mean_Temp_c|Numerical|Average daily temperature (ºC)|
|sd|Numerical|Standard deviation|

## :file_folder: Categorical variables levels for microbial data
|Category  | Levels        | Description        | Unit|
|----  |-----------|--------------------|-----|
|assay|plate|Total plate count| log<sub>10</sub> Colony-Forming Units (CFU)/g|
||tcid50|50% Tissue Culture Infectious Dose (TCID<sub>50</sub>)| log<sub>10</sub> TCID<sub>50</sub>/g|
||pcr|RNase RT-qPCR| log<sub>10</sub> Genome Copies (GC)/g|
|matrix|p|Soil samples without decaying plant materials, served as control sample|-|
||ps|Soil samples without decaying plant materials|-|
|microbe|ec|Enteric bacteria: _Escherichia coli_ TVS 353|-|
||nv|Enteric virus: Human norovirus GII (HuNoV GII)|-|
||tv|Enteric virus: Tulane virus (a surrogate for human norovirus)|-|
