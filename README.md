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
  Our data model focuses on a Loaded Tea comapany that functions as a franchise with many different locations across the United States. We started with our customer entity, indicating all of the relevant data stored on our customers ranging from atibutes of name, address, and contact information. For each customer, there are many sales, which we indicated through a one to many relationship with our sales entity. 
  
  The Sales entity displays data on the date, price and the payment method chosen by the customer for each sale. Additionally, the Sales entity contains two foreign keys- CustomerID and ProgramID- to represent the customers making each sale and whether they qualified for any discount programs (Military or Student). This then brings is to the Discount Programs table, which contains the program name and the percentage discount for each program offered for each. In this scenario, our comapny only offers Military and Student discounts, with military granting a 30% decrease in prices and Student granting a 20% decrease. This table additionally connects to the customers table as each customer can qualify for many discount programs in a one-to-many relationship.
  
  Similar to the relationship between sales and customers, Customer Orders and Customers also experience a one-to-many relationship as each customer can have many orders, but each order can only belong to one customer. This entity is differentiated from the sales table as those purchases were made online rather than at a specific franchise location. As an individual entity, Customer Orders stores the monetary amount of each order and the date the order was placed. 

  Considering that many orders can contain many products, we developed the associative identity labeled Customer Order Details to indicate this relationship between Customer Orders and Products. In this entity, we have the product ID and order ID for each, as well as the shipping date, status of the order, price, and quantity of items in the order. For the sake of this data model, we assume that the customer orders all have a scheduled date of which they will be shipped out, even if they are still being processed and have not yet shipped. We also assume that orders which are cancelled will not appear in the table any longer, and that customers are limited to the purchase of 20 items when choosing to by online instead of in person.
  
  Next is our product entity which keeps track of the different flavors and types of drinks offered by our company, specifically either Loaded Teas or Beauty Shakes in various fruity flavors. This table indicates a many-to-many relationship with the sales table as many sales can contain many different products, and vice versa. This relationship is held together by an associative identity labeled product line. This entity is non-identifiable and serves as a holding place for each identifiable entity's foreign keys.

  Many products in the product entity can also go to many store locations, hence the many-to-many connection between Store Location and Products.  The Store Locations entity is comprised of attributes including each store's area code, city, and state. This entity is also connected with the Employees table signifying that many employees can work at one store location, while each employee can only work at one location. 
  
  Together these two tables form the associative identity labeled "Supplier Orders", which contains the foreign keys of each individual entity with no other salient attributes. For completeness, we specify Supplier Orders as to differentiate from orders placed by the customers that come directly from the stock at the store locations versus the franchises purchasing more inventory to sell to customers. But the supplies in these orders must come from a home base, which brings us to our Supplier entity containing individual supplier IDs for each company, as well as their company name.

  Last, the Employees entity is the most complex of our entities, containing information on each employee's name, email, department name, and foreign keys identifying their respective store location and department chair. The department chair identifier is represented by a one-to-many recursive relationship, as one department chair can observe many employees.

<img width="952" height="441" alt="Screenshot 2026-03-30 at 11 27 29 AM" src="https://github.com/user-attachments/assets/678fd0a4-afc8-430f-9e32-6d5b40012a24" />

# Data Dictionary:
ADD DICTIONARY

# Queries:

# Database Information:
Database Name: Group_21479_G5
