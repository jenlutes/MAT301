## Problem Set 3 

#### 1. Define the terms: relation, tuple, attribute, record, and field.
Answer: Relation is a set of tables connecting to each other that exist in prexisting categories. Relation=Table. Tuple, or record is one set of data in relation. Tuple=record=row. Attributes, or field are specific database characteristics. Attribute=field=column.  

####2. What are keys in a relation?
Answer: Keys in a relation uniquely identify attributes or fields in a table. Examples of keys are: candidate, primary, foreign, natural, surrogate, and composite. 

####3. What is a surrogate key and how is it used?
Answer: A surrogate key is used to identify an item independent from other attributes. It is used to identify a single attribute, which is the best choice for a primary key. 

####4. In the following equation, Area = Length x Width, identify the determinant(s).
Answer: Determinants are used to identify another attribute in the relation. The determinants are length and width. When they are multiplied together, they determine area. 

####5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?
Answer: Primary keys are unique identifiers. There can be many composite keys to uniquely identify a single occurence. In order to make sure there is only one primary key, search through all the attributes to make sure only unqiue rows are delivered. 

####6. Give an example of a relation.  Determine a natural key for this relation.
Answer: An example of a relation is a clothing store inventory table with many field such as upc, product_id, department_id inventory, ect. Natural keys are universal identifiers that exist across the business world. The natural key in this table would be upc, a standard code for each product. The product_id could be considered a primary key to uniquely identify all products. 

  For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).  

####7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)
Answer: 

1NF:

----
| customer_id | first_name | last_name | zipcode | state | city | street | house_number | phone | email | order_id | items | quantity | price |

2NF: 

--------------
| customer_id |
|-------|
| first_name |
| last_name |
| phone |
| email |

| zipcode |
|-------|
| state |
| city |
| street |
| house_number |

| order_id|
|-------|
| item |
| quantity |
| price |


3NF: 

-----------
| customer_id |
|-------|
| customer_info|
| zipcode |
| order_id |

| customer_info |
|-------|
| first_name |
| last_name |
| phone |
| email |
| zipcode |

| zipcode |
|-------|
| state |
| city |
| street |
| house_number |

| order_id|
|-------|
| item |
| quantity |
| price |


####8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.
Answer: Since emails cannot be the exact same for different individuals, email could uniquely identify customers as a primary key. However, email should not be used as a primary key, rather it should be used as a natural, or reference key. The disadvantages of using email as a primary identifiers are email strings can be very similar and mistyped often, security on email servers are not always secure, and people can use many emails. It would be best to use customer's addresses or phone numbers because there is less room for mistakes. 

####9. Given two relations S and R below find the Cartsian Product S x R. 
Answer: 
RxS
--------------
| A | B| C | D | E |  
|---|---|---|---|---|
| 1 | 2 | 3 | 1 | 1 |
| 1 | 2 | 2 | 2 | 3 |
| 1 | 2 | 2 | 1 | 5 |
| 2 | 3 | 3 | 1 | 1 |
| 2 | 3 | 2 | 2 | 3 |
| 2 | 3 | 2 | 1 | 5 |

---------
####10. Find the natural join between the Faculty and Department relations below.
Answer:  The natural join, or common column between Faculty and Department Tables is Dept attribute. 

S
--------------
| A | B |
|---|---|
| 1 | 2 |
| 2 | 3 |
---------

R
------------
| C | D | E |
|---|---|---|
| 3 | 1 | 1 |
| 2 | 2 | 3 |
| 2 | 1 | 5 |



Faculty
--------------
| Name | ID | Dept |
|-------|----|----------------|
| Joe | 1 | Chemistry |
| Susan | 2 | Math |
| Tom | 3 | Marine Science |
| Mike | 4 | Math |


Department
------------
| Dept | Chair  |
|---|---|
| Chemistry | John |
| Math | Mike |
| Marine Science | Barry |
