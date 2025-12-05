# MATH144.PDS.Repo

## Motivating Question

Since coming to Poughkeepsie to attend Vassar, I've heard people discuss whether or not lead is present in the water. In 2024, Governor Kathy Hochul and State Representative Pat Ryan announced a [twelve million dollar](https://www.governor.ny.gov/news/governor-hochul-and-representative-ryan-announce-12-million-state-grant-replace-lead-water) state grant to begin to replace lead water pipes throughout Poughkeepsie. I became curious as to wheter or not these service lines are disproportionately distributed throughout the region. The city of Poughkeepsie has a history of redlining, and old infrastructure like water service lines are rarely replaced. To that extent, I searched for data that might point to a relationship between existing lead infrastructure and historical districting. 

## Data

The data has been compiled together from the New York State Department of Health's [2025 Lead Service Line Inventory](https://health.data.ny.gov/Health/New-York-State-Lead-Service-Line-Inventory/j63k-4n92/about_data). I also pulled data from interactive maps, including the University of Richmond's [Mapping Inequality](https://dsl.richmond.edu/panorama/redlining/) redlining map, their [social vulnerability map](https://dsl.richmond.edu/socialvulnerability/map/#loc=13/41.691/-73.915&city=poughkeepsie-ny), and [zipcode](https://www.unitedstateszipcodes.org/) maps. The compiled datasets and my process are included below. 

## Data Processing

The town and city of Poughkeepsie both have individual lead service line inventories, but they were nearly impossible to accurately convert to usable file types. Instead I did my best to pull from the state database. Given that the database has over 4.5 million entries, the whole thing was too large for me to export into Excel.  While the database lets users narrow down the dataset by the material and verification method of the service lines, there is no option for isolating rows by geographic location. This meant that in compiling a dataset, I was required to pull data from the entire state categorized by these various filters. This proved to be incredibly challenging as the filters were poorly organized and redundant. Ultimately I discovered that they did not call up entirely accurate subsets of data as well.  

I downloaded CSV files separated by material and material verification into excel, filtered out all rows corresponding to Poughkeepsie (and other derivative spellings), and combined them into one singlular database. Once compiled, I did very little secondary processing because the data I needed was relatively clean, and the presence of missing values did not hinder my investigation.

## Visualization

Included below is a pair of side-by-side bar charts comparing the counts of lead and non-lead service lines in two Poughkeepsie zip codes. The pink columns correlate to lsls. The blue column correlates to all other types of service lines (including unknown but potentially lead lines). 

![Bar Charts of lead service lines compared to non-lead lines separated by zipcode](https://github.com/mnwalker31/MATH144_PDS.Repo/blob/24105441e8052afe04d72ea2142045c87c144c68/lead%20visual.png)

## Analysis

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
