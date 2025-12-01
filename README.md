# MATH144.PDS.Repo

##Introduction
This personal data set compiles data about lead service lines (lsls) in two zipcodes covering both the town and city of Poughkeepsie. Although it has been determined that Poughkeepsie does indeed still have lead pipes, I was curious whether or not they are disproportionately distributed throughout the region. The data has been scraped from New York State Department of Health's 2025 Lead Service Line Inventory. I did my best to pull as much data as possible, but the filters prevented me from isolating rows by geographic location, meaning I had to compile the data based on various conditions. I also pulled data from interactive maps, including the University of Richmond's Mapping Inequality redlining map, their social vulnerability map, and zipcode information from unitedstateszipcodes.org. The compiled datasets and my process are included below. 

##Visualization
Included below is a pair of side-by-side bar charts comparing the counts of lead and non-lead service lines in two Poughkeepsie zip codes. The pink columns correlate to lsls. The blue column correlates to all other types of service lines (including unknown but potentially lead lines). 

![Bar Charts of lead service lines compared to non-lead lines separated by zipcode](https://github.com/mnwalker31/MATH144_PDS.Repo/blob/24105441e8052afe04d72ea2142045c87c144c68/lead%20visual.png)

##Analysis
While the total count of lsls across both zipcodes is relatively equal, there are far more non-lsls in the 12601 zipcode. I created a table with these counts and calculated the equivalent proportions: 

   | Line Material | Zipcode | Counts |
    | ----------- | ----- | ---- |
    | Lead         | 12601  | 144  |
    | Other        | 12601  | 1277 |
    | Lead         | 12603  | 142  |
    | Other        | 12603  | 4028 |
