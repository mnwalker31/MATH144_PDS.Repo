# MATH144.PDS.Repo

##Introduction
This personal data set compiles data about lead service lines (lsls) in two zipcodes covering both the town and city of Poughkeepsie. Although it has been determined that Poughkeepsie does indeed still have lead pipes, I was curious whether or not they are disproportionately distributed throughout the region. The data has been scraped from New York State Department of Health's 2025 Lead Service Line Inventory. I did my best to pull as much data as possible, but the filters prevented me from isolating rows by geographic location, meaning I had to compile the data based on various conditions. I also pulled data from interactive maps, including the University of Richmond's Mapping Inequality redlining map, their social vulnerability map, and zipcode information from unitedstateszipcodes.org. The compiled datasets and my process are included below. 

##Visualization
Included below is a pair of side-by-side bar charts comparing the counts of lead and non-lead service lines in two Poughkeepsie zip codes. The pink columns correlate to lsls. The blue column correlates to all other types of service lines (including unknown but potentially lead lines). 

![Bar Charts of lead service lines compared to non-lead lines separated by zipcode](https://github.com/mnwalker31/MATH144_PDS.Repo/blob/24105441e8052afe04d72ea2142045c87c144c68/lead%20visual.png)

##Analysis
While the total count of lsls across both zipcodes is relatively equal, there are far more non-lsls in the 12601 zipcode. I created a table with these counts and calculated the equivalent proportions: 


| Line Material | Zipcode | Counts |
| ------------- | ------- | ------ |
| Lead         | 12601  | 144  |
| Other        | 12601  | 1277 |
| Lead         | 12603  | 142  |
| Other        | 12603  | 4028 |

The resulting proportions indicate that while 3.5% of service lines in the 12603 zipcodes are confirmed to contain lead, 11.3% of the service lines in 12601 contain lead. These percentages indicate that a disproportionate amount of service lines within this zipcode contain lead, despite the fact that the actual amounts are relatively equal. 

<table><tr><td><img width="348" height="386.5" alt="Screenshot 2025-12-01 150801" src="https://github.com/user-attachments/assets/adb4818a-c04c-4e3d-a4aa-3e313a1e8bf9" /></td><td><img width="349" height="467" alt="Screenshot 2025-12-01 150730" src="https://github.com/user-attachments/assets/1a165fc5-e8e4-4329-8c30-e56ed867bc77" /></td></tr></table>

The image on the left represents the historical redlining, while the image on the right represents the current zipcode boundaries. 12601 encapsulates most of the red and yellow zones, while 12603 contains large of C7, B1, B2, B3, and A1 (the "higher quality" districts. Analyzing both the redlining map and the current zipcode map, it is clear that the 12601 zipcode services a much smaller area than the 12603 neighborhoods. The 12601 zipcode lines also relatively closely follow the boundaries of the most severely redlined districts, where property values were lowered by poor infrastructure and higher levels of racial diversity. While this relationship is likely correlated to many other factors and other data points, the data appears to corroborate the suggestion that within Poughkeepsie, aging infrastructure remains most prevalent in areas inhabited by diverse and lower-income groups. 
