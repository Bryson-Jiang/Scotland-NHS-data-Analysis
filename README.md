Project title
================
IDS No.1

## Proposal

Introduction: Our general question is to investigate the trend of
vaccination in Scotland over time from multiple groups of people and
perspectives. We will mainly use one data set which is “Daily Trend of
Vaccinations by Age Group and Sex”. The data is from The Scottish Health
and Social Care Open Data Platform which is managed by Public Health
Scotland. There are several variables in this data set, such as Date,
country, sex, Age group, Population, Dose, Number Vaccinated, Percent
Coverage, Cumulative Number Vaccinated, Cumulative percent Coverage. In
short, this data set has 19 columns(variables) and 26628 rows
(observations).

Link:<https://www.opendata.nhs.scot/dataset/covid-19-vaccination-in-scotland/resource/9b99e278-b8d8-47df-8d7a-a8cf98519ac1>

    ## Rows: 4454 Columns: 11

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (4): Country, Product, Dose, AgeBand
    ## dbl (7): _id, Date, Population, NumberVaccinated, PercentCoverage, Cumulativ...

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

    ## Rows: 26628 Columns: 19

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (8): Country, Sex, SexQF, AgeGroup, AgeGroupQF, Dose, PercentCoverageQF,...
    ## dbl (7): _id, Date, Population, NumberVaccinated, PercentCoverage, Cumulativ...
    ## lgl (4): PopulationQF, DoseQF, NumberVaccinatedQF, CumulativeNumberVaccinatedQF

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

    ## # A tibble: 6 × 11
    ##   `_id`     Date Country   Product Population Dose  NumberVaccinated PercentCoverage
    ##   <dbl>    <dbl> <chr>     <chr>        <dbl> <chr>            <dbl>           <dbl>
    ## 1     1 20201208 S92000003 AstraZ…         NA Dose…               12              NA
    ## 2     2 20201208 S92000003 AstraZ…         NA Dose…                0              NA
    ## 3     3 20201208 S92000003 Modern…         NA Dose…                0              NA
    ## 4     4 20201208 S92000003 Modern…         NA Dose…                0              NA
    ## 5     5 20201208 S92000003 Pfizer…         NA Dose…             1922              NA
    ## 6     6 20201208 S92000003 Pfizer…         NA Dose…                0              NA
    ## # … with 3 more variables: CumulativeNumberVaccinated <dbl>,
    ## #   CumulativePercentCoverage <dbl>, AgeBand <chr>

    ## # A tibble: 6 × 19
    ##   `_id`     Date Country   Sex    SexQF AgeGroup AgeGroupQF Population PopulationQF
    ##   <dbl>    <dbl> <chr>     <chr>  <chr> <chr>    <chr>           <dbl> <lgl>       
    ## 1     1 20201208 S92000003 Female <NA>  12 to 15 <NA>           114486 NA          
    ## 2     2 20201208 S92000003 Female <NA>  12 to 15 <NA>           114486 NA          
    ## 3     3 20201208 S92000003 Female <NA>  16 to 17 <NA>            53579 NA          
    ## 4     4 20201208 S92000003 Female <NA>  16 to 17 <NA>            53579 NA          
    ## 5     5 20201208 S92000003 Female <NA>  16 year… d             2354012 NA          
    ## 6     6 20201208 S92000003 Female <NA>  16 year… d             2354012 NA          
    ## # … with 10 more variables: Dose <chr>, DoseQF <lgl>, NumberVaccinated <dbl>,
    ## #   NumberVaccinatedQF <lgl>, PercentCoverage <dbl>, PercentCoverageQF <chr>,
    ## #   CumulativeNumberVaccinated <dbl>, CumulativeNumberVaccinatedQF <lgl>,
    ## #   CumulativePercentCoverage <dbl>, CumulativePercentCoverageQF <chr>

Data Analysis Plan: Data analysis demonstrates the relationship or trend
of data. We will plan to use different visualizations to deal with the
variables we interested. As shown above, we have planed to use tidyverse
and ggplot to draw plots which will improve the visualization of data.
If we will use more tools in the future of analysis, we will add that
tools into our plan.

In order to have a specific data analysis plan, we had defined the
outcome (Trend of total vaccinations) and the predictor (Age group and
sex) for our research questions. We plan to tidying the dataset firstly,
which could provide us a clear view of what data is telling us about.

After that, some plots will be drawn in order to assist our research.
For instance, we will draw a violin plot associate with the different
age group and total vaccinations. And that violin graph will reveals the
distribution of vaccinations among different age groups. For the
variables which have both x and y, we will draw a line plot to
visualized. Because we have different age group, we are going to colored
the different age group with different color. Comparison between color
could provide more information about the data.

Moreover, for the data only valid in plotting scatter points, we plan to
have a linear regression line of our plot which can reveal the
relationship between the points. We will also calculate correlation
coefficient to figure out whether sex is associate with the number of
vaccinations or not.

## Summary

Our general question is to investigate the trend of vaccination in
Scotland over time from multiple age groups of people and perspectives.
Fortunately, the result is supporting our hypothesis which we talked
before we analyze the data. From the graphs we plotted, we conclude that
majority of population take Dose 1 are during January to April i and
take Dose 2 during April to May in 2021. We thought the result is
trustworthy because there must be a period of waiting time between Dose
1 and Dose 2 about the vaccinations in medical considerations. As we
present in our presentation slides, we have divided the population of
Scotland into different age groups: 12 to 15, 16 to 17 and over 16
years. More specifically, the age group of over 16 years old, had also
being divided into 18 to 29, 30 to 39, 40 to 49, 50 to 54, 55 to 59, 60
to 64, 65 to 69, 70 to 74, 75 to 79 and 80 years and elder. The first
slide shows the line plot of female in number of vaccinations over time,
and the second slide is for male. Overall, they both have similar peak
in January and April which shows that male and female in Scotland have
similar trend in vaccinations. The reason why we keep the age group
categories in original dataset is we want to illustrate the relationship
between the number vaccinations and different age group. And the line
plots reveals that there is no effect of the number of vaccinations in
different age groups. In other words, most people in Scotland intend to
take vaccinations rather than refuse to take it in the US. Besides the
number of vaccinations, we still want to figure out the percentage
coverage of vaccinations in Scotland. Therefore, we have plotted two
graphs in following two slides which also divides the populations into
female and male in different age groups. Also, there is no anomalous
trend in any plot which is good to see it. There are two peaks in
January and April exactly. Those two peaks also support the previous
results we mentioned. Scotland have policies in vaccinations in January
for sure, which encourage people to take doses. Finally, we are looking
for the total percentage coverage of vaccinations in Scotland. The last
two slides with line graphs clearly shows that Scotland have 100%
coverage of Dose 1 around February and 100% coverage of Dose 2 around
May.

## Presentation

Our presentation can be found [here](presentation/presentation.html).
Link:
<https://media.ed.ac.uk/media/IDS_NO.1%20%20%20IDS%20final%20project%20presentation/1_qeieyu1r>
## Data

URL:<https://www.opendata.nhs.scot/dataset/covid-19-vaccination-in-scotland/resource/9b99e278-b8d8-47df-8d7a-a8cf98519ac1>

## References

URL:<https://www.opendata.nhs.scot/dataset/covid-19-vaccination-in-scotland/resource/9b99e278-b8d8-47df-8d7a-a8cf98519ac1>
