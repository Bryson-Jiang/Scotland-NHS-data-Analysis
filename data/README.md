# data

Place data file(s) in this folder.

Then, include codebooks (variables, and their descriptions) for your data file(s)
using the following format.

## name of data file
https://www.opendata.nhs.scot/dataset/covid-19-vaccination-in-scotland/resource/9b99e278-b8d8-47df-8d7a-a8cf98519ac1

- `Date`: Date on which vaccination occurred.
- `Country`: 9-digit country code for Scotland.
- `Sex`: Sex of individual.
- `SexQF`: Qualifier for Sex. 
- `Agegroup`: Age group of individual. COVID-19 vaccines are not routinely recommended for children and young people under 16 years of age so this age group is not included in the table. 
- `AgeGroupQF`: Qualifier for AgeGroup
- `Population`: Number of individuals in the cohort.
- `PopulationQF`: Qualifier for population.
- `Dose`: A 2-dose schedule is advised for all vaccine types in the current vaccination programme. Total includes both Dose 1 and Dose 2 vaccines administered.
- `DoseQF`: Qualifier for Dose.
- `NumberVaccinated`: Number of individuals who have received the vaccine
- `NumberVaccinatedQF`: Qualifier for NumberVaccinated
- `PercentCoverage`: Percentage of cohort having received vaccination. Percent coverage is calculated using the NRS Scotland 2020 mid-year population estimates by age and sex.
- `PercentCoverageQF`: Qualifier for PercentCoverage
- `CumulativeNumberVaccinated`: Cumulative number of individuals who have received the vaccine.
- `CumulativeNumberVaccinatedQF`: Qualifier for CumulativeNumberVaccinated
- `CumulativePercentCoverage`: Cumulative percentage of cohor having received vaccination. Percent coverage is calculated using the NRS Scotland 2020 mid-year populations by age and sex.
- `CumulativePercentCoverageQF`: Qualifier for CumulativePercentCoverage
