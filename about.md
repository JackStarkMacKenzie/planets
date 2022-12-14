# Data Descriptions

A short description of where the external data sources have been sourced from and what the
original and resulting outputs describe.

## The Processed Data

Beneath is a table showing the focus each of our output files we processed
had corrosponded to.

| CoL Focus                      | Data file                          | Raw Data Url                        |            
|--------------------------------|------------------------------------|-------------------------------------|                                                                      
| First Time Mothers             | 1st-time-mothers-prop_dz_data.csv  | [First Time Mothers][1]             |                                                                      
| Poor Household EPC Grades      | epc-prop_dz_data.csv               | [Poor Household EPC Grades][2]      |                                                           
| Total Household Floor Area     | epc-floor-area_dz_data.csv         | [Total Household Floor Area][2]     |                                    
| Large Families                 | 3child-households-prop_dz_data.csv | [Large Families][3]                 |                                                  
| Mean & Total Property Sales    | property-sales_dz_data.csv         | [Mean & Total Property Sales][4]    |
| Mean School Attainment         | school-att_dz_data.csv             | [Mean School Attainment][5]         |
| Proportion of Youth Population | youth-prop_dz_data.csv             | [Proportion of Youth Population][6] |



[1]: https://statistics.gov.scot/resource?uri=http%3A%2F%2Fstatistics.gov.scot%2Fdata%2Fage-at-first-birth
[2]: https://statistics.gov.scot/data/domestic-energy-performance-certificates
[3]: https://www.scotlandscensus.gov.uk/documents/2011-census-table-data-sns-data-zone-2011/
[4]: https://statistics.gov.scot/resource?uri=http%3A%2F%2Fstatistics.gov.scot%2Fdata%2Fresidential-properties-sales-and-price
[5]: https://statistics.gov.scot/resource?uri=http%3A%2F%2Fstatistics.gov.scot%2Fdata%2Feducational-attainment-of-school-leavers
[6]: https://statistics.gov.scot/resource?uri=http%3A%2F%2Fstatistics.gov.scot%2Fdata%2Fpopulation-estimates-young-and-old

# Descriptions

## First Time Mothers

From the raw data we filtered and extracted first time mothers underneath the age of nineteen. Breaking down this dataset
by datazone gives us a look at the proportion of potentially, financially disadvantaged young mothers and how they are                                                                               
distributed throoughout the geographical area.

## Poor Household EPC Grades

For this dataset we extracted each UPRN's EPC rating from the raw data and arranged it to show the proportion
of households that have an EPC rating of less than C for every datazone. The resulting dataset can aid an
understanding of how each datazone is coping under the pressure of energy prices during this Cost of Living Crisis.

## Total Household Floor Area

From the same raw data set we used for Poor Household EPC Grades, we processed it instead to show the mean
total floor area of households within every datazone. Knowing the proportion of households that have poor
EPC gradings, and then to also know how big the properties are in each datazone, furthers an investigation
into which datazones are struggling to pay for energy given poor epc gradings and smaller/more affordable
housing.

## Large Families

The Census provides a dataset on the amount of children in each family, for each datazone. Our resulting dataset                                                                                     
is one that only filters through the families with three or more children and gives the proportion of families that
have this many per datazone. As the cost of living rises providing for large families becomes more difficult and it
wouldn't be unreasonable to suggest a lot of these families would be receiving child benefit.

## Mean & Total Property Sales

The resulting dataframe is an extraction of each datazone's mean and total property sales. The table was then
pivoted so that we can see these figures as a time series between 2004-2021.

## Mean School Attainment

The raw data gives the mean of the highest grade every school leaver achieved before graduating. The mean is based on the highest level
of qualification they achieved at grades C to A in National Qualifications or Skills for Work while at school. i.e. If a student's highest
grade was a C, B or A in a Level 3 course, their highest grade is 3. If a D is achieved at a level 3 this gets rounded down to a level 2
in which case the student's highest grade is scored as 2. Then all the leavers' scores are summed up and divded by the amount of
school leavers in that datazone. The sum of all school leavers is totaled across a three year chunk between 2019-2021.

## Proportion of Youth Population

After filtering only the count of under 16 year olds per datazone, we created a resulting proportion feature of how much of
a datazone's population is under 16.
