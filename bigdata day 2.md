ods(operational data store)=> kis bhi data base ke all data ko ek sath leker Jha store krtre use ods(operational data store) kahte hai jo dta hum jaha rkhte use staging area bhi kahte hai,in ods hum data short term tak hi store rhta hai aur isme realtime dta and current data store krte h





**oltp(online transaction processing)**=>  its use genrally database ,for bussines run we use it, its take low time,in this data NOT Historical not long data is store and not duplicate in this store



**olap(online anylitcal processing)**=> its use genrally dwh data warehouse,making a dessions for bussions, its take more time  because its store histrocal data and long data and



**data modeling =>** its creatae vislluasation how to store a data access the data mange the data



1. **er modeling =>** its use databases
2. \*\*dimensional modeling=>\*\*its is data modeling technic to use in our data ware house to -



\*\*dimensional modeling\*\* => 2 type table preseent

**fact table** => its store measure value menas those value whose we calculate ,It usually has foreign keys that link to dimension tables.

 		example=>salary,amount,quantity sold

**dimensional table**=> its provide descriptive value means in refrences of measures

 	example=> location of sale ,department of my salarys, quantity sold for my product



**schema**=> its is database structure where we store database.

In Dimensional Modeling, a Schema is the logical design or structure of how fact tables and dimension tables are organized and connected in a data warehouse.



\*\* **schema type in dwh\*\* =>**

star schema=>The fact table is at the center. and the fact table directly connected wuth

multiple Dimension tables are directly its called starts schema.

 its Looks like a star shape.

Simple and fast for queries.

**Example:**

Fact Table → Sales\_Fact (Sales\_Amount, Quantity)

Dimensions → Product, Customer, Time, Store

**snowflake schema=>**

An extension of Star Schema means

Dimension tables are normalized into multiple related tables.

Looks like a snowflake shape.

Saves storage space, but queries become more complex.





**\*\*\*difference between start schema vs snowflake\*\*\***



| Feature         | Star Schema ⭐                            | Snowflake Schema ❄️                      |

| --------------- | ---------------------------------------- | ---------------------------------------- |

| \*\*Structure\*\*   | Fact + denormalized dimensions           | Fact + normalized dimensions (hierarchy) |

| \*\*Design\*\*      | Simple, star-like                        | Complex, snowflake-like                  |

| \*\*Storage\*\*     | More storage needed (redundant data)     | Less storage  (removes 											redundancy)        |

| \*\*Query Speed\*\* | Faster (fewer joins)                     | Slower (more joins)                      |

| \*\*Maintenance\*\* | Easy to maintain                         | More complex to maintain                 |

| \*\*Use Case\*\*    | Best for small to medium data warehouses | Best for large, complex data 										warehouses  







galaxy schema=>the mutiple fact table are connected and sharing with multiple dimensions 		tables

&nbsp;		galaxy call fact consellation schema

-- its reduce redudence 





