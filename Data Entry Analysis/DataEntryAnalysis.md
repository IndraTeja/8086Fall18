# Assignment 1 - Data Entry Analysis 
----

## Part1 - Issues in Data Entry

1. There are few Blanks and Missing data in the sheets. zoop - temp-main.xlsx has missing data for Temp coloumn.
2. pond2010.xlsx has issing data values in Temp, density and  colony diameter.
3. The background description explains about the comparison of data collected during day and night. But, this attribute is missing from the all three sheets. There should have been a coloumn with Time or Day/Night along with date.
4. zoop - temp.xlsx has three coloumns with same depth 0.5 for same date, why do we have such data? This is not collected at same time becuase other values are changing. These values are collected at different times on same date.

| Date     | Depth | Cuni #/L | Cuni ColonySize | Chippo #/L | Chippo ColonySize | Chla | Temp |
|----------|-------|----------|-----------------|------------|-------------------|------|------|
| 6/7/2011 | 0.5   | 87       | 2.4             | 49         | 2.8               | 3.2  | 18.2 |
| 6/7/2011 | 0.5   | 66       | 2.48            | 46         | 2.94              | 3.6  | 18.2 |
| 6/7/2011 | 0.5   | 30       | 2.33            | 35         | 2.9               | 3.2  | 18.2 |

5. There are no units for few fields like z, Temp, density, Colony Diameter, Chippo #/L, etc
6. There is a need for Metadata with proper format for attributes, what does z stand for? What is the meaning of #/L? What is Chla?
7. Couldn't find the relationship between pond2010 and zoop - temp.xlsx attributes.
8. pond2010.xlsx has 2010 data, whereas zoop - temp.xlsx has 2011 data. There is no consistency in way data is collected. We cannot compare unless both the datasets have common timeframe.
9. The sheet 'pond2010.xlsx' has the name pond, so does it mean this data was collected in a pond. What about the other 2 sheets? Were they collected in a pond or somewhere else?

----

## Part2 - Recommendations - New format

Species can be abbrivated, but they must follow proper scientific code or standard.

| Location | Date | Time | Depth(m) | Temp(F/C) | Density(units) | Colony Diameter(units) | Species |
|:--------:|:----:|:----:|:--------:|:---------:|:--------------:|:----------------------:|---------|
|          |      |      |          |           |                |                        |         |


OR


| Date 	| Depth(m) 	| Cuni #/L(units) 	| Cuni ColonySize(units) 	| Chippo #/L(units) 	| Chippo ColonySize(units) 	| Chla(units) 	| Temp 	| Time 	| Location 	|
|:----:	|:--------:	|:---------------:	|:----------------------:	|:-----------------:	|:------------------------:	|:-----------:	|:----:	|------	|----------	|
