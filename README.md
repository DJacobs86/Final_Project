# Final Project
https://public.tableau.com/app/profile/dave.jacobs/viz/NationalParksFinal_ProjectNPS_VBSP-CGEdit4-19-23_16820154840060/NationalParks?publish=yes

### What do we intend to show:
National Park Visitation and Amenities data – We have found data about national park amenities and visitation numbers for the previous year. We would like to see if there is a correlation between any of the park amenities and the number of visitors annually. Criteria for amenities: state, lat/long, total Sites, tent only, the number of electrical hook ups, showers, dump station present, host, potable water, firewood for sale.

We hypothesized that greater amenities would result in greater visitorship due to ease of access and convenience. A potential visitor would be less likely to camp at a location if they had to bring their own water, had to bathe in a muddy river, had to chop down their own wood, and not be able to charge any electric appliances.

### Data Exploration:
The park visitation data was collected from the National Park Service, and the amenities data was gathered from Kaggle.com. During the initial data exploration phase, the data sourced from Kaggle had been deleted shortly after acquisition, meaning some of the context for the data had been lost.

<img src="Final_Project/Resources/DBD.png" alt="A list of our variables" title="Our variables" style="display: inline-block; margin: 0 auto; max-width: 300px">

### Analysis Phase:
We have displayed charts, maps, and graphs showing the sum of visitors by state in 2022, percent change in visitors to parks between 2021 and 2022, various displays of the amenities (showers, dump stations, tents, etc.), and visualizations of visitation based on the changes in amenities. To create the correlations between amenities and visitation, we performed logistic regressions.

### Technology Used:
- Data Prep – Jupyter Notebook/Python, combine and store the excel worksheets we have exported from Kaggle and the National Parks Service website. 
- Data Storage – PostgreSQL
- Statistics/Analysis - Machine Learning/Neural Networks
- Presentation – Tableau Story

### Results:
Shower Y regression shows that the number of campsites in a state that includes showers explains approximately 24% of the variation in annual visitation, however the number of campsites without showers explains approximately 33% of the variation in visitation. These inherently contradictory findings is indicative of the limitations of the data, namely that each park/site could not be assigned its respective visitation figures, meaning we had to assign it only by state.

The total number of tent-only campsites explains approximately 58% of the variation in visitation.

The number of total campsites in each states explains approximately 17% of the variation in visitation.

### Future Analysis Recommendations:
Ensure that the data source includes data for all fifty states instead of approximately half.
The data we had was limited in that we were unable to assign visitation by campsite specifically, so we had to assign it to each state.
Ensure that the data source does not get deleted in the duration of the analysis.

### If Time Was Not A Factor
We have strong reason to believe that proximity to a commercial airport is a statistically significant variable that could explain the variation in visitation, for it is much more difficult to access a park if it is incredibly remote and cut off. We would have calculated the distance using the latitude and longitude of each campsite and airport. The stand-in for the significance of the airport would have been based on whether it had "international" in its name.

A limitation of the data was that we were not able to assign visitation to each of the campsites. Had we had more time, we could have simply used all of the national parks and hard-collected the visitation data for each of them. That way, we would not have had to stratify it on state.

### Group Roles: 
- Noor – Machine Learning/Neural Networks
- Dave - PostgreSQL
- Robert - Tableau 
- Chris – Data Prep/Jupyter Notebook/Python
- Zachary - Readme/Written Analysis

### Notes from SQL Server
We ran into an issue in which the data didn't matchup. We went into the CSV file to manually change some cells to match the data types. The merge was successful then.
