# Toylica-Company-Case-Study---SQL

# Online retailer business: Toylica case study

- The online retailing business is quite famous currently. Here, you do not need to take orders by going to each customer. In online retailing, a company launches its website to sell the items in wholesale, and buyers can order the products that they require from that website only. In this case study, you are introduced to a company that manufactures toy replicas or models.

- Toylica , a toy replica company, has captured a huge market globally and supplies toy replicas in almost all the countries. Wholesale buyers order products in their required quantity from the website only. As  the company captured a large customer base and enhanced its workforce, it is essential for this company to maintain the database to navigate and store the employee-, customer- and product-related information.

- The brand has a separate department for analysing its sales and building a machine learning model to predict future sales. Each customer’s order is saved into the database using the OLTP process when they place their order. A team of data analysts and machine learning engineers perform OLAP tasks on the historic data for creating marketing strategies to enhance the business.

- Suppose you are a data analyst working at this company. Here, you are only focusing on the SQL queries to get an idea of the company’s sales. Now, let’s understand the process and structure of the database that the company is using. The three sections in the database of the company are as follows:
       ● Employee section
       ● Customer section
       ● Product section

# 1. Employee section: This section is divided into the following tables:
a. employees: This table contains information about a company’s employees. Each entry in this table is identified uniquely by the ‘employeeNumber’, which is the primary key of this table.

b. offices: This contains information about the company’s offices that are located worldwide. Each office is uniquely identified by the ‘officeCode’, which is the primary key of this table. Each employee must have only one office against their ID, in which they have to work.

# 2. Customer section: This section contains the following tables:
a. customers: This table contains information about customers who buy the models from the company in bulk. They are retailers or shopkeepers who own firms or shops; they are not the final consumers. Each customer is uniquely identified by the ‘customerNumber’, which is the primary key of this table. A particular customer is either assigned an employee or not assigned any. The assigned employee is identified by the ‘salesRepEmployeeNumber’ column in this table. Multiple customers can be assigned to an employee.

b. orders: This table contains information about the orders placed by the customers. Each order is uniquely identified by its ‘orderNumber’, which is the primary key of this table. Multiple orders can be placed by a particular customer, but each order should have a unique ‘orderNumber'.

c. orderdetails: This table also contains details about the orders placed by the customers. However, both the 'orderNumber’ and ‘productCode’ are part of the composite primary key here.

d. payments: This table contains information about the payments made by the customers after placing their orders. Here, you will notice a column named ‘checkNumber’, which refers to the unique number of the check through which the customer (‘customerNumber’) has made the payment. Under this table, ‘checkNumber’ is the primary key.

# 3. Product section: This section has the following tables:
a. products: The ‘products’ table contains information about the different products that are sold by the company. Each product is uniquely identified by the 'productCode’, which is the primary key of this table.

b. productlines: This table is a broad categorisation of the type of toy models that are sold by the company, including vintage cars, motorcycles, trains and ships. Each product in the ‘products’ table must have a single product line.

# Finally, you will have the following eight tables:
1. employees
2. offices
3. customers
4. orders
5. orderdetails
6. payments
7. products
8. productlines

   

