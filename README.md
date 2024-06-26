# README


## **Housing Burden Among Aging Populations**

The overall research question: How are different aging populations
affected by housing costs in Central Pines Regional Council’s seven NC
counties?

The seven counties in North Carolina we will be looking at are:

1\. Chatham

2\. Durham

3\. Orange

4\. Wake

5\. Moore

6\. Lee

7\. Johnston

## **Why is this question important?**

In the United States (U.S.), North Carolina (NC), and all seven CPRC
counties, populations are rapidly aging. For the last 20 years, the
fastest growing age group across all geographic domains in the U.S. is
the adult population 65 years and older (65 plus).

According to the U.S. Census Bureau’s American Community Survey 2020
5-year estimate, 30% of US adults 65 plus are below the 200% federal
poverty threshold. This number is expected to increase from 5.3 million
low-income older adult households in 2018 to 7.9 million households in
2038. Yet only one third of those older low-income adult households that
are eligible for housing assistance based on their income levels
received assistance.

Limited incomes today are met with rising housing costs pushing many
families into a cost-burdened category where they are paying more than
30% of their income on housing.

The purpose of this research is to visualization and better understand
who is burdened by housing costs in CPRC’s counties to better target
future housing policy interventions.

## **Key Definitions**

• **Housing burden**: an individual spending over 30% of their gross
income on rent or housing costs.

• **Rent burden**: an individual spending over 30% of their gross income
on rent.

• **Home owner cost burden**: an individual spending over 30% of their
gross income on financing a home they own (e.g., mortgage expenses).

• **Aging population**: Most demographic data is collected for 65 years
and older populations, but some agencies consider a broader group under
this definition based on funding. The Older American’s Act has
opportunities for those 60 years and older, while county-based senior
centers in North Carolina are moving towards serving populations 55
years and older. For the purposes of this analysis, CPRC’s prefers to
use the broader definition of 55 years and older where they can.

## **Data Source**

Data was pulled from two sources: 1. American Community Survey (ACS)
1-Year 2021 Public Use Microdata Sample (PUMS) from Census.gov:
https://www.census.gov/programs-surveys/acs/microdata/access.2021.html#list-tab-735824205.
Can be found in /data folder on my github /censuselderlyhousing
repository.

2\. Using the R ‘tidycensus’ package, we pulled all relevant shapefiles
for mapping PUMS areas and NC counties.

- \#tigris::pumas(“NC”, cb = TRUE, year = 2020, progress_bar = FALSE)

- \#tigris::counties(“NC”, cb = TRUE, year = 2020, progress_bar = FALSE)

## **Census Data Analysis**

PUMS data is a sample of about 1% of the US population. When we want to
estimate a variable that represents the entire population rather than a
sample, we have to apply a weighting adjustment. The weight variable
tells us the number of people in the population that the observation
represents We used the PUMS person weight for all population estimate
calculations.

## **Chnages Made to Graphs**

Following the presentations we made, we made changes on the population
bar chart and the dot plots on race taking feedback and moving the
legend to the bottom of the charts. We also added in the scale for the
values on the y-axis.

## **Findings**

- Rent cost burden and home ownership burden is worse for Black
  residents of all counties.
- Chatham and Lee counties the percent home owner cost burden is closer
  making it less of a disparity along race.
- Rent burden is consistently under 10% across all counties for white
  residents, potentially because they are more likely to own than rent.
- Wake County as the most populous county has the largest number of
  individuals 55+ with an expected stacking of more younger age groups
  compared to older age groups.
- Rent burden is concentrated around Raleigh in Wake County and Durham
  in Durham County.
- Percent of population burdened by home owner costs are more evenly
  distributed across the counties with some hot spots in Durham, Wake,
  and Johnston Counties
- Most counties follow an expected pattern of aging populations across
  different age groups meaning there are more people in younger
  categories and less people as they age.
