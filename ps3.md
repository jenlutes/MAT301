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
Answer: 

####6. Give an example of a relation.  Determine a natural key for this relation.
Answer: 

  For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).  

####7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)
Answer: 

####8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.
Answer: 

####9. Given two relations S and R below find the Cartsian Product S x R. 
Answer: 

####10. Find the natural join between the Faculty and Department relations below.
Answer: 

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
