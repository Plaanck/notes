
## Hashing Function

- The **hashing function** is an algorithm that transforms a string of characters into a key (hash value) that represents the original input
- You cannot undo the hashing function, meaning it is a one way process, which differentiates it from encryption
- The reason we would want this is, for example, a website holding passwords.
	- The website does not want to store all of its users passwords in a database as is, because if a hacker gets into the database, they have access to the passwords.
	- Instead, we want to be able to validate whether an inputted password (when passed through the hashing function) matches the username and encrypted password

## Other Uses of Hashing

- Hashing can also be used for sorting and searching, as we do not need to check every value in the hash table, we can just input what we are looking for, and run it through the hashing function, and compare to the hash values, and immediately find the item we want.
- On average, a hash search has O(1) [[9- Big-O-Notation||Complexity]]
























This is related to Hash Tables, see below.
[[7- Hash Tables (Theory)]]
[[(Extra) Hash Table (Coding)]]