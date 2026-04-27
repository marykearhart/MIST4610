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
1. For the first supplemental question, we had to create a new calculated field titled "Cost per Mile" which we used to find the average amount paid by a customer per mile the taxis driver had to deliver them to their destination.
<img width="483" height="300" alt="Screenshot 2026-04-26 at 11 09 09 PM" src="https://github.com/user-attachments/assets/0609f501-5d49-47a1-a5c4-848d196fdacb" />


2. Our second calulated field was titled 'Airport Trip' which we used to manipulate the data under 'Airport Fee' to differentiate between rides that did have an airport fee (were rides to the airport) and those that didn't (rides that were not to the airport) for our second supplemental question.
<img width="483" height="300" alt="Screenshot 2026-04-26 at 11 46 55 PM" src="https://github.com/user-attachments/assets/af821cd9-c109-429d-9307-5090161ddab1" />


# Analysis and Results
1. bar chart depicting the cost per mile at each pick up location and line graph depicting the average trip distance based on the pick up location.
comparing the average price with the average distance, a certain spike indicate where there are good deals that would make a customer want to specifically choose a taxi over another ride share service.
also an area chart depicting the average cost per mile at each location and the average distance with a label of the average total cost which altogether indicates that custoemrs take advantage of the lowest fares to travel the furtheest, using certain pick up locations to do so.
<img width="1102" height="742" alt="Screenshot 2026-04-26 at 11 08 47 PM" src="https://github.com/user-attachments/assets/ab94ac14-a20f-4499-bb90-f2211db6c156" />
<img width="1103" height="745" alt="Screenshot 2026-04-27 at 12 07 56 AM" src="https://github.com/user-attachments/assets/49fca624-b6b1-4012-a2ec-dd594eff0690" />


2. three way bar chart comparing average total cost, average airport fee, and average trip distance given whether or not the ride was to the airport or not. shows a payment breakdown of whether the aiport fee is a deal-breaker for customers. data suggests that the pricing is more based on distance travelled rather than the fees to get to the airport, making taxis a comparable competition with other ride share companies.
<img width="1095" height="740" alt="Screenshot 2026-04-26 at 11 55 05 PM" src="https://github.com/user-attachments/assets/51ba0882-6f38-4774-a96e-d87962cda30a" />


# Tableau File
https://public.tableau.com/views/MISTPROJECT/Sheet3?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link 
