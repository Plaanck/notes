
#  Database Normalisation 

 - The idea behind normalisation is that it is just another way to organise a database, which can be more efficient, and keep the database easier to maintain.
- There are 3 types of normalisation that we need to know.
	- First order normalisation (1NF)
	- Second order normalisation (2NF)
	- Third order normalisation (3NF)

## First Order Normalisation

- The rules for 1NF are,
	1) All field names must be unique
	2) Values in fields should be from the same domain
	3) Values in fields must be atomic
	4) No 2 records can be identical
	5) Each table needs a primary key

- In the second rule, this means that the information in that field must all be the same type of data, you cannot have someone's name and their age in the same field, they must be separate
- Atomic means that there should only be one value in each entry/cell. 

## Second Order Normalisation

- 2NF has three rules,
	1) The data must be in 1NF
	2) Any Partial Dependencies have been removed
	3) No many-to-many relationships

- A partial Dependency is when a field is not dependent on the primary key.
	- In order to fix this, we would need to split the data into two tables, where now there are no partial dependencies.
	- In doing so, you may make two tables linked in a many-to-many relationship
	- In order to get rid of this, you need to see which fields can be inferred from another field, that isn't the primary key.
		- These fields can be put into a new table, that would be in the middle of the two larger tables.
		- Now, rather than the two tables being connected with Many-to-Many, they are both connected to the middle table in a one-to-many relationship, thus meeting all the requirements for 2NF

