# Modeling-Data-Warehouse-with-Data-Vault

Full course available at: https://www.udemy.com/course/modeling-data-warehouse-with-data-vault-for-beginners/

I am familar with relational database and as a part of my continual learning journey, I am educating myself about data warehouse. I used [diagrams.net](https://www.diagrams.net/) to draw the ER diagrams.

Simple ER diagram for a store use case, converting Relational Database to Dimensional Modeling. 

![Store Diagram](https://user-images.githubusercontent.com/55467236/228358998-1ddd7046-c17f-4c11-8975-651ab159100b.jpg)


Convert Relational Database to Data Vault. 

See databricks definition on Data Vault:

In general, a Data Vault model has three types of entities:

**Hubs** — A Hub represents a core business entity, like customers, products, orders, etc. Analysts will use the natural/business keys to get information about a Hub. The primary key of Hub tables is usually derived by a combination of business concept ID, load date, and other metadata information.

**Links** — Links represent the relationship between Hub entities. It has only the join keys. It is like a Factless Fact table in the dimensional model. No attributes - just join keys.

**Satellites** — Satellite tables have the attributes of the entities in the Hub or Links. They have descriptive information on core business entities. They are similar to a normalized version of a Dimension table. For example, a customer hub can have many satellite tables such as customer geographical attributes, , customer credit score, customer loyalty tiers, etc.

Source: Prescriptive Guidance for Implementing a Data Vault Model on the Databricks Lakehouse Platform (https://www.databricks.com/blog/2022/06/24/prescriptive-guidance-for-implementing-a-data-vault-model-on-the-databricks-lakehouse-platform.html)

![3NF to DV](https://user-images.githubusercontent.com/55467236/228949059-6d9ebe2a-3318-4d7c-aa42-6354fb09f26d.jpg)



Another example, converting Dimentional Modeling to Data Vault:


![DIM to DV](https://user-images.githubusercontent.com/55467236/228949131-37e1cd65-db67-475d-8d5b-f94b8ba327e6.jpg)
