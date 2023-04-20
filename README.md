## What do we intend to show:
National Park Visitation and Amenities data – We have found data about national park amenities and visitation numbers for the previous year. We would like to see if there is a correlation between any of the park amenities and the number of visitors annually. Criteria for amenities: state, latitude/longitude, total sites, tent only, bumber of electrical hook ups, showers, dump station present, host, potable water, firewood for sale. This data was gathered from the National Park Service and a Kagel user.

We hypothesized that greater amenities would result in greater visitorship due to ease of access and convenience. A potential visitor would be less likely to camp at a location if they had to bring their own water, had to bathe in a muddy river, had to chop down their own wood, and not be able to charge any electric appliances.

### Data Exploration:
The data was gathered from the National Park Service and a user on Kagel.

### Analysis Phase:


## Technology Used:
- Data Prep – Jupyter Notebook/Python, combine and store the excel worksheets we have exported from Kaggle and the National Parks Service website. 
- Data Storage – PostgreSQL
- Statistics/Analysis - Machine Learning/Neural Networks
- Presentation – Tableau Story

### Results:
Shower Y regression shows that the number of campsites in a state that includes showers explains approximately 24% of the variation in annual visitation, however the number of campsites without showers explains approximately 33% of the variation in visitation. These inherently contradictory findings is indicative of the limitations of the data, namely that each park/site could not be assigned its respective visitation figures, meaning we had to assign it only by state. There also did not appear to be any strong correlation between all-inclusive amenities and visitation, indicating that visitors do not particularly care about what is available; they are there for the park itself, and everything else is secondary.

The total number of tent-only campsites explains approximately 58% of the variation in visitation, and sites that have the most electrical hookups and regular access to dump stations correlate with higher visitation, most likely due to RVs being better accomodated. However, the data from which this was pulled no longer exists, so it cannot be confirmed.

The number of total campsites in each states explains approximately 17% of the variation in visitation, meaning that quantity of parks does not strongly explain quantity of visitors; quality matters more.

### Future Analysis Recommendations:
Ensure that the data source includes data for all fifty states instead of approximately half.
The data we had was limited in that we were unable to assign visitation by campsite specifically, so we had to assign it to each state.
Ensure that the data source does not get deleted in the duration of the analysis.

## Group Roles: 
- Noor – Machine Learning/Neural Networks
- Dave - PostgreSQL
- Robert - Tableau 
- Chris – Data Prep/Jupyter Notebook/Python
- Zachary - Written Report
