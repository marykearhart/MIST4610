# MIST4610
# Team Name:
21479 Group 5
# Team Members:
1. Derek Quinlan [@derekq111](https://github.com/derekq111)
2. Regan Taylor [@nrt19057](https://github.com/nrt19057)
3. Sydney James [@srj44873](https://github.com/srj44873)
4. Mary Earhart [@mke48687](https://github.com/marykearhart)
# Problem Description:
Our group handled the task of creating a data model for our franchise "Loaded Tea" company. Our loaded tea company is operated in variious locations around the US, each with their own employees lead by department chairs in Human Resources and Franchise Coordination. Additionally, our model accounts for the unformation stored on the customers at each location, their eligibility for military and student discounts, and the supplier-to-business coordination of supply orders aside from those purchases made directly from the location by the customer. Our overarching goals of this project were to accurately display each relationship between entities, create sample data tables for each entity and its attributes, and finally test out various queries relevant tov the business operations of our organization.
# Data Model:
  Our data model focuses on the overaching Loaded Tea comapny as a franchise with many different locations. We started with our customer entity, indicating all of the relevant data stored on our customers ranging from atibutes of name, address, and contact information. For each customer, there are many sales, which we indicated through a one to many relationship with our sales entity. 
  
  The sales entity displays data omn the date of each sale, price of each sale, and the payment method chosen by the customer with the addition of the customer ID as a foreign key to connect each purchase to the purchaser. 
  
  Similar to sales, we expressed a one-to-many relationship between Customer orders and Customers, which is differentiated from the sales table as those purchases were made online rather than at a specific franchise location. This table stores the this table store the monetary amount of each order and the date the order was placed. 
  
  The third and final table connected to the Customers entity is the Discount Programs table, also expressed through a one-to-many relationship as each customer can qualify for many discount programs. The programs offered are Miltary and Student discount, each offering a 20% decrease in price for the customer if they apply. This table includes the program name and the percentage discount for each program offered, and additioinally connects to the sales table as each discount code can have many sales. 
  
  Next is our product entity which keeps track of the different flavors and types of drinks offered by our comapny, ranging from different fruity flavors of both our "Beauty Shakes" and "Loaded Teas". This table indicated a many-to-many relationship with the sales table as many sales can contain many different products, and vice versa. This relationship is held together by an associative identity labeled product line. 

  
# Data Dictionary:

# Queries:

# Database Information:
