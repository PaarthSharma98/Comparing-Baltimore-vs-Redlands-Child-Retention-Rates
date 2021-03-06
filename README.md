# Business Analytics Project 1

## Background
The aim of this mini project was to compare retention rates for children (how many kids live in the same region as adults) in a small town such as Redlands and a bigger city like Baltimore. Average household income of these kids as adults was also assessed to provide contextual data. In addition to comparing difference between Baltimore and Redlands, intracity analysis was also conducted to see differences in outcomes based on starting parent income of these children. The results are presented below. 

## Results
![alt text](https://github.com/PaarthSharma98/Comparing-Baltimore-vs-Redlands-Child-Retention-Rates/blob/master/Manipulated%20Data%20and%20Figures/Redlands%20Analysis%20Segmented.png)
When looking at retention rate across different parent income levels in Redlands, there was not much difference. However, children with parents in the high income classification were slightly less likely to live in the same region as adults. One interesting trend to note is that household income of children in those regions as adults correlated to some degree with regional retention rate. 

![alt text](https://github.com/PaarthSharma98/Comparing-Baltimore-vs-Redlands-Child-Retention-Rates/blob/master/Manipulated%20Data%20and%20Figures/Baltimore%20Analysis%20Segmented.png)
We see similar trends in retention rate for the Baltimore graph as with Redlands. However, the difference in retention rate for children with middle/low income parents vs high income parents is a bit more pronounced. Another trend to note is that household income (as well as retention rates) varies drastically across the city and thus there are likely a plethora of regional factors which add to the variability. 

![alt text](https://github.com/PaarthSharma98/Comparing-Baltimore-vs-Redlands-Child-Retention-Rates/blob/master/Manipulated%20Data%20and%20Figures/Redlands%20Baltimore%20Comparison.png)
When comparing basic retention rate and household income data for Baltimore and Redlands, two things are clearly visible: the average retention rate for children in Baltimore is about 17% higher than Redlands, but the average household income of those children as adults is about 30% lower. 

## Data Analysis Steps
1. Data was collected from [The Opportunity Atlas](https://www.opportunityatlas.org/) for Baltimore and Redlands. All datasheets had the following column values: [Tract Name Metric]
2. Data was extracted from each excel into a common spreadsheet, separated into different sheets for Baltimore vs Redlands
3. In a new column, I used the IFERROR and INDEX commands to add the tract id of each metric into one column
4. The "Remove Dublicates" excel feature was used to ensure only unique values remained in the column
5. Next, I used VLOOKUP to find and add data pertaining to each tract into a new table. Thus, I had a new table witht he following column values: [Tract Name Metric1 Metric2 Metric3...]
6. I then used the pivot table feature to create a new pivot table to average metric data for each region name
7. A 3 axis plot was then created to showcase regional differences within Baltimore and Redlands
8. A combo bar-line graph was also made using data averaged amongst all region names
