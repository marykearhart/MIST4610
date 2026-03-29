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

  Many products in the product entity can also go to many store locations, which is connected with an associative identity titled "Supplier Orders", to differentiate from order placed by the customers that come directly from the stock at the store locations. 

  The Store Locations entity is comprised of attributes including each store's area code, city, and state. This entity is also connected with the Employees table signifying that many employees can work at one store location, while each employee can only work at one location.

  Last, the Employees entity is the most ocmplex of our entities, containing information on each employee's name, email, and the foeign keys identifying their respective store location, department chair, and the preceeding department chair as indicaed through a recursive one-to-one relationship. The department chair identifier stems from our Department entity which indicates the ID for the department which each employee that serves as department chair is a part of, as well as the name of that department (either Human Resources or general Franchise Operations for the national company).
  <img width="897" height="425" alt="Screenshot 2026-03-29 at 7 37 09 PM" src="https://github.com/user-attachments/assets/5782c0e2-81b0-4e1c-98ef-4bb4d502f950" />

# Data Dictionary:
<img width="724" height="258" alt="Screenshot 2026-03-29 at 7 41 28 PM" src="https://github.com/user-attachments/assets/9112ef65-ba06-447e-8e18-0767150addb8" />
<img width="724" height="306" alt="Screenshot 2026-03-29 at 7 41 22 PM" src="https://github.com/user-attachments/assets/f4b8db86-439a-405d-8005-db1787370641" />
<img width="724" height="373" alt="Screenshot 2026-03-29 at 7 41 14 PM" src="https://github.com/user-attachments/assets/adcb92df-a37f-4d9a-8217-28c373b2a808" />
<img width="724" height="445" alt="Screenshot 2026-03-29 at 7 41 05 PM" src="https://github.com/user-attachments/assets/e9c62120-a666-4ae2-94a0-702cbd751e13" />
<img width="724" height="304" alt="Screenshot 2026-03-29 at 7 40 58 PM" src="https://github.com/user-attachments/assets/e6584bb8-b9cd-40fc-8202-b41762d41294" />
<img width="724" height="343" alt="Screenshot 2026-03-29 at 7 40 48 PM" src="https://github.com/user-attachments/assets/97e97951-8a63-4f50-94d2-0202cef9c6b4" />
<img width="724" height="417" alt="Screenshot 2026-03-29 at 7 40 40 PM" src="https://github.com/user-attachments/assets/98d433a6-d00f-4f01-b2ae-896fd919fcd9" />
<img width="724" height="540" alt="Screenshot 2026-03-29 at 7 40 31 PM" src="https://github.com/user-attachments/assets/40315315-7444-426c-a743-cad3b2b55e6f" />
<img width="724" height="580" alt="Screenshot 2026-03-29 at 7 40 16 PM" src="https://github.com/user-attachments/assets/bee40e1d-56a7-48f7-96f4-18bc8047579a" />
<img width="724" height="686" alt="Screenshot 2026-03-29 at 7 40 06 PM" src="https://github.com/user-attachments/assets/9c7b6343-64c9-4a85-99fa-418e1d970e46" />
<img width="724" height="309" alt="Screenshot 2026-03-29 at 7 39 55 PM" src="https://github.com/user-attachments/assets/92a2cef7-f5b2-46be-b613-9dfa55e1049e" />
<img width="726" height="462" alt="Screenshot 2026-03-29 at 7 39 43 PM" src="https://github.com/user-attachments/assets/40ea1cfa-4b54-4305-a749-97470250eb3c" />

# Queries:

# Database Information:
