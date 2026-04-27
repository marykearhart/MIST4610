# Yellow Taxi Profit Analysis
# Team Members
1. Derek Quinlan [@derekq111](https://github.com/derekq111)
2. Regan Taylor [@nrt19057](https://github.com/nrt19057)
3. Sydney James [@srj44873](https://github.com/srj44873)
4. Mary Earhart [@mke48687](https://github.com/marykearhart)
# Data Set: 2023 Yellow Taxi Trips
We chose a comprehensive data set depicting thousands of real taxi rides in New York city. Attributes of the dataset include the trip distance, drop off times, drop off and pick up locations, rate types, payment types, and passenger counts. 
# Team Questions
## Overarching Question
Are there certain scenarios and instances that make taxi's more profitable for the driver? What about scenarios where the customer benefits over other ride systems like uber and lyft?

In a fast moving and technological society, it is very common to see goods and services that were once bustling with popularity get replaced by more efficient, automated tools. With a handful of various ride-share systems competing against eachother, we thought the data in this dataset could be useful to indicate customer behaviors specific to New York City and how the iconic yellow taxi system handles comeptition in the evolving transportation market.

## Supplemental Question 1
How does the cost per mile change given the pick up location and the trip distance? What might this indicate about taxi users?

Looking at the dataset's top 20 popular pickup locations in NYC, we wanted to see how far customers typically drive given the location they are picked up at, as well as the average cost per mile they are paying on those trips. By comparing these two data, we hoped that answering this question could help us find out if there are areas where riders can get a great deal for their trip and take advantage of cheaper fares that otherwise wouldd not ge them as far in an Uber or Lyft.

## Supplemental Question 2
How do taxi prices change between airport rides and city regular rides?

This question helps to understand the profitability of the taxi driver, and whether or not their charge of airport fees upcharges their rides out of the range of the average ride-share system, decreasing their competitive advantage. 

# Applied Manipulations
## Manipulation 1
For the first supplemental question, we had to create a new calculated field titled "Cost per Mile" which we used to find the average amount paid by a customer per mile the taxis driver had to deliver them to their destination.
<img width="483" height="300" alt="Screenshot 2026-04-26 at 11 09 09 PM" src="https://github.com/user-attachments/assets/0609f501-5d49-47a1-a5c4-848d196fdacb" />


## Manipulation 2
Our second calulated field was titled 'Airport Trip' which we used to manipulate the data under 'Airport Fee' to differentiate between rides that did have an airport fee (were rides to the airport) and those that didn't (rides that were not to the airport) for our second supplemental question.
<img width="483" height="300" alt="Screenshot 2026-04-26 at 11 46 55 PM" src="https://github.com/user-attachments/assets/af821cd9-c109-429d-9307-5090161ddab1" />


# Analysis and Results
## Supplemental Question 1
To find the answer to our first supplemental quesiton, we started with a line graph indicating the relationship between the average rid edistance from each pickup location, labeled with the average distance in miles. Underneath this we paired the line graph with a bar graph indicating the relationship between the average cost per mile driven at each pick up location. Immeidately upon pairing these two graphs together, we notice an interesting relationship occuring at locations 132 and 138. There was a spike that indicated further rides took place while the average cost per mile was the lowest at these locations. 
<img width="1102" height="742" alt="Screenshot 2026-04-26 at 11 08 47 PM" src="https://github.com/user-attachments/assets/ab94ac14-a20f-4499-bb90-f2211db6c156" />

Before coming to any conclusions, we made a second graph to better visually understand this relationship. This graph shows the area covered for the same relationships with average distance per trip an cost per mile with each pickup location, only this time labeled by the average total cost for a ride by a customer. By bringing the two seperate graphs together, the relationship became more obvious that ucstomers were spending voerall more money at these locations where they were also going farther distances and recieving lower fare costs. This suggests that because fares were so cheap at these locations, customers were more willing to be taken further or closer to their actual destination instead of walking from further away to avoid high fares. While we only looked at the twenty most popular locations for taxi pickups, this ties us back to our overarching question stating that the average taxi customer will change their behavior depending on the deals they can get from the driver.
<img width="1103" height="745" alt="Screenshot 2026-04-27 at 12 07 56 AM" src="https://github.com/user-attachments/assets/49fca624-b6b1-4012-a2ec-dd594eff0690" />

## Supplemental Question 2
While we were given the feees for the rides to the airports, we wantd to find a direct comparison in total costs for rides to the airport versus rides to anywhere else in the city. We also wanted to compare the price breakdown, along with the average trip distance to see what portions of the price change were attributed by the airport fees versus the fact that the riders were being taken farther. We ultimately decided a three way bar chart comparing these features was the best way to differentiate between each attribute for non-airport rides and airport rides. We observed that while the general fares were higher for airport rides, only a very small portion of that was attributed by the airport fee; with this being said, we also observed that the distance travelled for airport rides was signifigcantly more than city rides. We can assume from these observations that while the airport rides are more expensive than regular rides, the are at a competitive price point with Ubers and Lyfts because regardless for the airport fee as the bulk of each ride cost comes from the distance of the ride to the airport. We can therefore further assume that any other bsuiness would also have to upcharge longer drives, meaning that a customer would not be at a real loss choosing a taxi over another ride-share systems when trying to go to the airport.
<img width="1095" height="740" alt="Screenshot 2026-04-26 at 11 55 05 PM" src="https://github.com/user-attachments/assets/51ba0882-6f38-4774-a96e-d87962cda30a" />

## Conclusion
Together, these two experimental data analyses we completed for this project help us see the behavioral descision making of taxi users and taxi drivers in New York when compared against Ubers, Lyfts, and other competitors as we hoped to in our overarching project question. Our first supplemental question helped us to see real proof of areas where riders took advantage of the deals they were getting at certain locations when taking a taxi over another mode of transportation. Additionally, Our second data analysis shows us that when it comes to airport demand, taxis keep a competitive price and do not generally hike up their airport fees as to not deter any customers that will otherwise exchange taxis for Uber or Lyft. For the most part, we can observe from these two examples that customers will find deals where they can within the NYC taxi system, but generally speaking the taxi rivers maintain a comeptitive market price for sustaianble competitive edge.

# Tableau File
https://public.tableau.com/views/MISTPROJECT/Sheet3?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link 
