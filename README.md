# MIST4610
# Team Name:
21479 Group 5
# Team Members:
1. Derek Quinlan [@derekq111](https://github.com/derekq111)
2. Regan Taylor [@nrt19057](https://github.com/nrt19057)
3. Sydney James [@srj44873](https://github.com/srj44873)
4. Mary Earhart [@mke48687](https://github.com/marykearhart)
# Problem Description:
  Our group handled the task of creating a data model for our franchise "Loaded Tea" company. Our business is operated in various locations around the US, each with their own employees lead by department chairs in specialized Human Resources. Additionally, our model accounts for the information stored on the customers at each location, their eligibility for military and student discounts, and the supplier-to-business coordination of supply orders aside from those purchases made by the customers either online or in person. Our overarching goals of this project were to accurately display each relationship between entities, create sample data tables for each entity and its attributes, and test out various queries relevant to the business operations of our organization.
# Data Model:
  We started off our data model by creating a customer entity, indicating all of the relevant data stored on our customers ranging from atibutes of name, address, and contact information. For each customer, there are many sales, which we indicated through a one to many relationship with our sales entity. 
  
  The Sales entity displays data on the date, price and the payment method chosen by the customer for each sale. Additionally, the Sales entity contains two foreign keys- CustomerID and ProgramID- to represent the customers making each sale and whether they qualified for any discount programs (Military or Student). This then brings is to the Discount Programs table, which contains the program name and the percentage discount for each program offered for each. In this scenario, our company only offers Military and Student discounts, with military granting a 30% decrease in prices and Student granting a 20% decrease. For the sake of the complexity of our data model, we assume that all customers' sales will apply for one of these discounts. This Discount Program table also connects to the customers table as each customer can qualify for many discount programs in a one-to-many relationship.
  
  Similar to the relationship between sales and customers, Customer Orders and Customers also experience a one-to-many relationship as each customer can have many orders, but each order can only belong to one customer. This entity is differentiated from the sales table as those purchases were made online rather than at a specific franchise location. As an individual entity, Customer Orders stores the monetary amount of each order and the date the order was placed. 

  Considering that many orders can contain many products, we developed the associative identity labeled Customer Order Details to indicate this relationship between Customer Orders and Products. In this entity, we have the product ID and order ID for each, as well as the shipping date, status of the order, price, and quantity of items in the order. For the sake of this data model, we assume that the customer orders all have a scheduled date of which they will be shipped out, even if they are still being processed and have not yet shipped. We also assume that orders which are cancelled will not appear in the table any longer, and that customers are limited to the purchase of 20 items when choosing to by online instead of in person.
  
  Next is our product entity which keeps track of the different flavors and types of drinks offered by our company, specifically either Loaded Teas or Beauty Shakes in various fruity flavors. This table indicates a many-to-many relationship with the sales table as many sales can contain many different products, and vice versa. This relationship is held together by an associative identity labeled product line. This entity is non-identifiable and serves as a holding place for each identifiable entity's foreign keys.

  Many products in the product entity can also go to many store locations, hence the many-to-many connection between Store Location and Products. Since our Loaded Tea company functions as a franchise with many different locations across the United States, the Store Locations entity is comprised of attributes including each store's area code, city, and state to differentiate between each shop. This entity is also connected with the Employees table signifying that many employees can work at one store location, while each employee can only work at one location. 
  
  Together these two tables form the associative identity labeled "Supplier Orders", which contains the foreign keys of each individual entity with no other salient attributes. For completeness, we specify Supplier Orders as to differentiate from orders placed by the customers that come directly from the stock at the store locations versus the franchises purchasing more inventory to sell to customers. But the supplies in these orders must come from a home base, which brings us to our Supplier entity containing individual supplier IDs for each company, as well as their company name.

  Last, the Employees entity is the most complex of our entities, containing information on each employee's name, email, department name, and foreign keys identifying their respective store location and department chair. The department chair identifier is represented by a one-to-many recursive relationship, as one department chair can observe many employees. We will assume in this case that each employee contains a departmentChair ID which refers to the department chair which oversees their work at their respective location.

<img width="952" height="441" alt="Screenshot 2026-03-30 at 11 27 29 AM" src="https://github.com/user-attachments/assets/678fd0a4-afc8-430f-9e32-6d5b40012a24" />

# Data Dictionary:
<img width="678" height="544" alt="Screenshot 2026-03-31 at 9 08 44 AM" src="https://github.com/user-attachments/assets/a8425806-a034-4aa1-8ad3-257b5f5462de" />
<img width="678" height="365" alt="Screenshot 2026-03-31 at 9 08 25 AM" src="https://github.com/user-attachments/assets/a4c8f68e-2ece-4d34-9a91-0166b8b8179f" />
<img width="678" height="555" alt="Screenshot 2026-03-31 at 9 08 11 AM" src="https://github.com/user-attachments/assets/a596cb06-17f9-49c8-9a2f-bea490a0978f" />
<img width="678" height="333" alt="Screenshot 2026-03-31 at 9 07 29 AM" src="https://github.com/user-attachments/assets/eafa2cd9-8853-4eb1-9c4f-3e5a7f77a925" />
<img width="678" height="666" alt="Screenshot 2026-03-31 at 9 07 15 AM" src="https://github.com/user-attachments/assets/29617523-5886-47b1-b2b3-14d5ae272635" />
<img width="678" height="482" alt="Screenshot 2026-03-31 at 9 06 49 AM" src="https://github.com/user-attachments/assets/0d76f6ed-87f1-4649-ac77-e1cb5808cdb2" />
<img width="678" height="482" alt="Screenshot 2026-03-31 at 9 06 35 AM" src="https://github.com/user-attachments/assets/93348015-3678-4a90-aa2f-da06419918e6" />
<img width="678" height="705" alt="Screenshot 2026-03-31 at 9 06 23 AM" src="https://github.com/user-attachments/assets/c55af9d7-5ee5-44cf-a5a6-833b3cfa9dea" />
<img width="678" height="468" alt="Screenshot 2026-03-31 at 9 06 06 AM" src="https://github.com/user-attachments/assets/de254c04-6aa5-45ae-87a9-092af40ad012" />

# Queries:

# Database Information:
Database Name: Group_21479_G5
