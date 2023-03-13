**In order to see how to program a Hash Table, See:**  [[(Extra) Hash Table (Coding)|Hash Table Code]]


- Hash Tables are a type of data structure that uses keys and hashes to assign values.
	> 	An easy way to think about this is that Python's implementation of a Hash Table is the Dictionary, See [[1- Arrays, Lists, Tuples, Records, Dictionaries#Dictionaries|Dictionaries]]


#### Overview
* In order to find the position of an item in a hash table, we use a **Hashing Function**
	* This is a function that uses all sorts of mathematical functions such as MOD (%), in order to make it hard for anyone to read the actual data, but the hash could be anything
		* E.G. Lets say you put a password, 11 into a Hash Table, and our Hashing Function is:                                		f(x) = x % 3
		* The password will be stored in a hash, which will be 11 % 3, which is = 2
		* This is good, as it is near impossible to tell that your password is 11, as 14%3 is 2, and so on and so forth
		* The drawback to this is how you order this in the Hash Table, if you are ordering it by the hash generated, as said, many passwords could have the same hash, so we need more ways to store them: See [[7- Hash Tables (Theory)#How Do We Order it?|Ordering]]
	
	* There are 3 main properties that a good Hashing Function should have.
		1. **It should be able to be calculated quickly**
		2. **It should result in as little Collisions as possible**
		3. **It should use as little memory as possible**
		> Remember, real life Hash Functions are much more complicated than F(x) = x % 3 So even though there is multiple solutions to what each hash could be, its going to be very hard to have two pieces of data collide due to the complexity of the algorithm



#### How Do We Order it?

* As said previously, we can have situations where there are two pieces of data that is trying to be stored with the same hash, this is known as **Hash Collisions**
	- One solution to this problem is called **Open Adressing**, where if two hashes collide, you just keep checking the next available space and store it there
		> To find the data later, the hashing function tells us where the starting position is, they then use a [[1- Linear Search|Linear Search]] unti it finds the item. This is commonly known as **Linear Probing**

	- A disadvantage with open adressing is that the more misplaced items there are, the more it prevents other items from being stored in their correct places too
		- It also results in **Clustering** where several positions are filled around the common collision values.
	

	- Another Solution to handle collisions is by using a 2D hash table. ^064d5a
		- This then allows two entries to be inputed into the same address while still being separate, this is known as **Chaining**
		> See [[1- Arrays, Lists, Tuples, Records, Dictionaries#2D Lists|2D Lists]] for more information on how they work
	
  
		- Another possibility is to use a second table for collisions, more commonly known as an overflow table, which can also be searched sequentially ^7a09e4
			- You can also use [[4- Linked Lists|Linked Lists]] to maintain the overflow table


- The issue with hashing algorithms is that there is often trade-offs between the efficiency of the algorithm and the size of the hash table
	- The process for finding an alternative position in the table is known as **Rehashing**



## Operations On a Hash Table

- The main three operations you can perform on a hash table is:
	1. Add: adding new items into the hash table
	2. Delete: removing items from the hash table
	3. Retrieve: Finding an item from a hash table using its hash value





