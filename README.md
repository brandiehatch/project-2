# Ames Housing: Project 2
#### Brandie Hatch

## Define the Problem
Interest: increase housing access for Black or African American individuals and families in Ames, Iowa. <br>

Goal: Using the Ames, Iowa Housing Kaggle data set, Census Demographic Data for population density by race and hispanic origin along with the Income by Location Median Household Income map create a model to predict the Sales Price of houses in a certain area of Ames, Iowa. <br>

Problem: As the Black or African American populations rise in a census tract area, how does the sale price of houses in Ames, Iowa change? 

__Null Hypothesis:__  There is a negative association between a high percent of Black population and the sale price (as the Black population rises, sale price goes down).

__Alternative Hypothesis:__ There is not a negative association between high percent of population and the sale price.

## Background

The Ames population was estimated at 58,965 during the 2010 Census. This includes student enrollment at ISU. Iowa State University of Science and Technology (ISU) serves over 36,000 students from all over the world and is located in the heart of Ames, Iowa. 
https://www.cityofames.org/about-ames/interesting-facts-about-ames<br>

Across the United States, Black homeowner rates have only increased 1.2% between 1970 and 2019. Historic real estate practices still plague the market today even though they have been outlawed since the Fair Housing Act of 1968 was passed. The Fair Housing Act prohibits private and public housing discrimination and requires the federal government to administer all federal housing and community development programs to affirm fair housing practices. <br>

Unfortunately, discrimination still occurs. Redlining is the historic act of deeming certain areas as excessively risky for investment. As noted in the NPR article __Black Americans and the Racist Architecture of Homeownership__ [May 8, 2021](https://www.npr.org/sections/codeswitch/2021/05/08/991535564/black-americans-and-the-racist-architecture-of-homeownership), "one way Black people and other minority groups were left out systematically was through a process known as "redlining" which labeled certain areas as "risky" for a home loan. African Americans and immigrants were relegated to areas, marked in red on government-sponsored maps, where poverty was most concentrated and housing was deteriorating." <br>

Today, the term “redlining” is used to describe certain historic race-based segregating tactics in real estate — from estate agents directing Black home buyers and renters to certain neighborhoods and away from others to racial rules in many suburbs and developments. "Houses that are essentially the same with the exception of one being in a majority Black neighborhood and one in a majority white neighborhood have almost a 50 percent difference in value", Twedt-Ball said in the Iowa newspaper [The Gazette](https://www.thegazette.com/education/redlining-continues-to-create-racial-disparity-in-homeownership-in-cedar-rapids-iowa/).<br>

Many of the same neighborhoods that were redlined in the past continue to high poverty rates, lower median household incomes, and higher levels of marginalized populations. "Historically redlined areas have been cumulatively affected by a low prevalence of home ownership, uneven economic development, displacement of residents, and lack of access to education and economic opportunities." From: (https://publichealth.berkeley.edu/news-media/research-highlights/research-more-oil-and-gas-wells-in-redlined-neighborhoods/)

### Datasets:

1. train.csv: Data set contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010.
2. test.csv: Same as train.csv, but without the Sale Price column.

https://www.tablesgenerator.com/markdown_tables# <br>

| **Feature**        | **Type** | **Dataset**  | **Description**                                                                                                                                                                                                              |
|--------------------|----------|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **id**             | _int64_  | train & test | ID number used for Kaggle Submission.                                                                                                                                                                                        |
| **ms_subclass**    | _object_ | train & test | Identifies the type of dwelling involved in the sale.                                                                                                                                                                        |
| **ms_zoning**      | _object_ | train & test | Identifies the general zoning classification of the sale.                                                                                                                                                                    |
| **neighborhood**   | _object_ | train & test | Physical locations within Ames city limits.                                                                                                                                                                                  |
| **n_code**         | _object_ | train & test | Neighborhood locations bundled based roughly on Census Tracts.                                                                                                                                                               |
| **percent_pop**    | _object_ | train & test | Percentage of total Black population that reported their race as Black or African American in the [2020 Census](https://mtgis-portal.geo.census.gov/arcgis/apps/MapSeries/index.html?appid=2566121a73de463995ed2b2fd7ff6eb7) |
| **condition_1**    | _object_ | train & test | Proximity to various conditions.                                                                                                                                                                                             |
| **condition_2**    | _object_ | train & test | Proximity to various conditions (if more than one is present).                                                                                                                                                               |
| **overall_qual**   | _int64_  | train & test | Rates the overall material and finish of the house.                                                                                                                                                                          |
| **overall_cond**   | _int64_  | train & test | Rates the overall condition of the house.                                                                                                                                                                                    |
| **year_built**     | _int64_  | train & test | Original construction date.                                                                                                                                                                                                  |
| **year_remod_add** | _int64_  | train & test | Remodel date (same as construction date if no remodeling or additions).                                                                                                                                                      |
| **sale_type**      | _object_ | train & test | Type of sale.                                                                                                                                                                                                                |
| **saleprice**      | _int64_  | train        | Sale price in US Dollars.                                                                                                                                                                                                    |

## Conclusions and Recommendations


## Sources
- Median Household Income Ames, IA: https://datausa.io/profile/geo/ames-ia#income_geo
- 2020 Census Demographic Data Map Viewer, Population Density, Race Alone or In Combination, Hispanic Origin, and Group Quarters: https://mtgis-portal.geo.census.gov/arcgis/apps/MapSeries/index.html?appid=2566121a73de463995ed2b2fd7ff6eb7 
- Past Housing Policies, Practices Contribute To Iowa's Racial Homeownership, Wealth Gaps | Iowa Public Radio | by Katarina Sostaric | https://www.iowapublicradio.org/racial-justice/2020-12-18/past-housing-policies-practices-contribute-to-iowas-racial-homeownership-wealth-gaps
- Racial Disparities in Home Appreciation | Jul 15, 2019 | Michela Zonta | https://www.americanprogress.org/article/racial-disparities-home-appreciation/
- Why the homeownership gap between White and Black Americans is larger today than it was over 50 years ago | https://www.cnbc.com/2020/08/21/why-the-homeownership-gap-between-white-and-black-americans-is-larger-today-than-it-was-over-50-years-ago.html
- The American Dream While Black: "Locked in a Vicious Cycle" | https://www.nbcnews.com/specials/american-dream-while-black-homeownership/
- Black Americans And The Racist Architecture Of Homeownership | NPR Code Switch | May 8, 2021 11:20 AM ET | By Ailsa Chang, Christopher Intagliata, Jonaki Mehta | https://www.npr.org/sections/codeswitch/2021/05/08/991535564/black-americans-and-the-racist-architecture-of-homeownership
- Research: More oil and gas wells in redlined neighborhoods Historically marginalized communities are exposed to more wells with their accompanying pollution | By Dylan Svoboda | April 13, 2022 | https://publichealth.berkeley.edu/news-media/research-highlights/research-more-oil-and-gas-wells-in-redlined-neighborhoods/
- City of Ames: https://www.cityofames.org/
- Neighborhoods of Ames, IA map from Prediction Model of Ames Real Estate Prices: https://rstudio-pubs-static.s3.amazonaws.com/337439_24918eaefe724411be93e41ede48b256.html



### Instructors, please REMEMBER:

I tried something new and even though I spent many hours working, it did not turn out as well as I had planned. I'm excited to work on this more to get it profile ready.

This is a learning environment and you are encouraged to try new things, even if they don't work out as well as you planned! While this rubric outlines what we look for in a _good_ project, it is up to you to go above and beyond to create a _great_ project. **Learn from your failures and you'll be prepared to succeed in the workforce**.
