# Yellow Taxi Profit Analysis
# Team Members
1. Derek Quinlan [@derekq111](https://github.com/derekq111)
2. Regan Taylor [@nrt19057](https://github.com/nrt19057)
3. Sydney James [@srj44873](https://github.com/srj44873)
4. Mary Earhart [@mke48687](https://github.com/marykearhart)
# Data Set: 2023 Yellow Taxi Trips
We chose a comprehensive data set depicting thoursands of real taxi rides in New York city. Attributes of the dataset include the trip distance, drop off times, drop off and pick up locations, rate types, payment types, and passenger counts. 
# Team Questions
1. How does the number of passengers impact the fare per passenger?

This question inidcates if taxi drivers change their rates to accomodate for the influx of passengers riding in their taxi at a time. Especially if the different passengers are going to different locations, it may take longer for the taxi driver to get to one place after the other and therefore lead to them charging more per customer.

2. How does tip amount differ by average trip distance?

We wanted to analyze whether passengers are more likely to tip more the farther the distance the taxi driver has to take them. This measure is a strong behvaioral indicator of how the average passenger views tips and whether they are a key part of the taxi driver's pay per trip.
# Applied Manipulations
In order to answer the first question, we had to create a new measure labelled "farePerPassenger" which is indicated by the equation in the screenshot below:
<img width="1042" height="614" alt="Screenshot 2026-04-16 at 9 21 17 AM" src="https://github.com/user-attachments/assets/cc3dc8cc-a282-43cf-9054-c2c20db2975f" />

# Analysis and Results
1. To answer our first question, we created a bar graph attached below that depicts the relationship between the average fare per passenger and the number of riders in the taxi. Initially, we assumed that the fares would be generally higher as it may be mroe incovnienient for the taxi driver to have so many people to drive at once. Upon observation of our barchart, we realized that the opposite was true. Since there are more passengers, fare is divided amongst more people and therefore leads to lower prices per individual.

<img width="687" height="887" alt="Screenshot 2026-04-16 at 11 26 56 AM" src="https://github.com/user-attachments/assets/d73a907c-be24-4734-a974-194cd6e05dd4" />

2. To answer our second question, we decided to create a scatter plot of the tip granted per ride given the average distance of each ride. We went into this test assuming that the longer the ride, the more likely the passenger would tip a higher amount out of courtesy. What we ended up discovering was that the tips generally range in a very cocnentrated bubble, with some outliers of passengers tipping more or less for unrelated circumstances we do not have the power to identify. We also discovered a strange occurance of some passengers tipping excessively for the short distance they drove, which we attributed to the type of passenger. For example, a regular taxi passenger commuting to work may be likely to tip less as a regular rider, whereas a tourist may tip more for the service since they are only visiting. In all, we concluded that from a behavioral standpoint, there must be a subcultural standard for tip amounts that locals find reasonable on a regular basis and which seperates them from visiters who are unaware of this unspoken rule.

<img width="688" height="622" alt="Screenshot 2026-04-16 at 11 27 12 AM" src="https://github.com/user-attachments/assets/34d23f5c-7fac-4207-be17-ee5dedda5727" />

# Tableau File
