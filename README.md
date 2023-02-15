# IBM Data Engineering Capstone Project Overview

This Capstone provides us with the opportunity to demonstrate all of the practical hands-on Data Engineering skills you have while following the program. 

As part of the Capstone project, we will assume the role of an Associate Data Engineer who has recently joined an e-commerce organization. We will be presented with a business challenge that requires building a data platform for retailer data analytics. 

In this Capstone project, we will: 
1. Design a data platform that uses MySQL as an OLTP database and MongoDB as a NoSQL database. 
2. Design and implement a data warehouse and generate reports from the data. 
3. Design a reporting dashboard that reflects the key metrics of the business. 
4. Extract data from OLTP and NoSQL databases, transform it and load it into the data warehouse, and then create an ETL pipeline.
5. And finally, create a Spark connection to the data warehouse, and then deploy a machine learning model.

## Environment
This section introduces us to the data platform architecture of the ecommerce company named SoftCart. Softcart uses a hybrid architecture, with some of its databases on premises and some on cloud.
![data_platform_architecture](https://user-images.githubusercontent.com/79985278/218961251-1d0b0e65-15cb-438e-b226-6d2523ffc071.png)

### Tools and Technologies used:
- OLTP database = MySQL
- NoSQL database = MongoDB
- Production Data warehouse = DB2 on Cloud
- Staging Data warehouse = PostgresSQL
- Big data platform = Hadoop
- Big data analytics platform = Spark
- Business Intelligence Dashboard = IBM Cognos Analytics
- Data Pipelines = Apache Airflow

### Process:

SoftCart's online presence is primarily through its website, which customers access using a variety of devices like laptops, mobiles and tablets.

All the catalog data of the products is stored in the MongoDB NoSQL server.

All the transactional data like inventory and sales are stored in the MySQL database server.

SoftCart's webserver is driven entirely by these two databases.

Data is periodically extracted from these two databases and put into the staging data warehouse running on PostgreSQL.

Production data warehouse is on the cloud instance of IBM DB2 server.

BI teams connect to the IBM DB2 for operational dashboard creation. IBM Cognos Analytics is used to create dashboards.

SoftCart uses Hadoop cluster as it big data platform where all the data collected for analytics purposes.

Spark is used to analyse the data on the Hadoop cluster.

To move data between OLTP, NoSQL and the dataware house ETL pipelines are used and these run on Apache Airflow.
