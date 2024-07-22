# UK_real_estate_data_analysis
In this project, we are using 10 GB of data and adaptability in working with property insight, and  comfort with applying statistical techniques to manipulate data.

Data sources
Dataset Link Notes

Land
Registry

https://www.gov.uk/gover

nment/statistical-data-
sets/price-paid-data-
downloads

Use the complete dataset, not the current
month

Postcodes
(NSPL)

https://geoportal.statistics.
gov.uk/datasets/f7464f36
58ba439ba577651b32014
cfe/about

The NSPL contains codes for various
administrative geographies. The corresponding
names can be found under "Names and Codes"
in the web portal

British
National
Grid
shapefiles

https://github.com/charles
roper/OSGB_Grids?
tab=readme-ov-file

Use 10km resolution

London Borough Count of sales in 2023 Average sale price in 2023
Barking and Dagenham ? ?
Barnet ? ?
...
Exercises

Using the sources above:
1. Find two land registry records that are likely to be errors
2. Complete the following table by calculating the number of sales and average sale price for
all London Boroughs in 2023:
In each case, provide a potential explanation

3. Count the number of new build Flats sold in each UK region since the start of 2020
4. Plot the number of sales per week since the start of 2020 as a line chart
5. Plot a histogram of sale prices and discuss which distribution best represents the data
Discuss the chart, and provide potential explanations for any patterns or anomalies
Feel free to transform the data before plotting, but explain your reasoning if you
choose to do so
For the following exercises, use the complete price paid dataset and British National grid tiles at
10km resolution. If you are unfamiliar with geospatial data, try using GeoPandas
6. Using the BNG tiles and an appropriate scale, plot a map showing the number of sales per
10km grid square
7. Plot a map showing the average sale price per 10km grid square
8. Comment on your findings
9. Given everything you have learned from the exercises above, discuss the following model.
In your discussion, provide an approximate R value that you would expect from the
model
How would you improve the model?
What range of R would you be happy with?
2

2
Price ~ β ∗ Y ear + ∑i=1 α +
nα
i ∑i=1 γ +
nγ
i ε

Where:
is the coefficient for the year of sale
and are dummy variables corresponding to postcode area and property type
respectively
β
αi γi

9. Energy Performance Certificates (EPCs) are published for each property transaction
recorded by the Land Registry. The data schema for these is available here

I. Which fields from this dataset would be useful in determining sale price?
II. How would you approach the task of joining the EPC database with the Land Registry?
N.B. We don't expect you to actually join the databases - but please provide as
much detail as possible about how you would approach the task.
