
- In a nutshell, the Big O Notation is a way of describing how much effort it will take for a computer to process an algorithm.
	> This can either be represented in how long it takes (Time), or how much space it takes up in Memory


- There is an order in magnitude as to how much space/time it takes for each type of algorithm to compute
	- The main ones are (ascending order):
		- Constant - O(1)    [[9- Big-O-Notation#Constant - O(1)|Jump To Heading]]
		- Logarithmic - O(log(n)) [[9- Big-O-Notation#Logarithmic|Jump To Heading]]
		- Linear - O(n) [[9- Big-O-Notation#Linear|Jump To Heading]]
		- ~~O(nlog(n))~~
		- Polynomial - O(n$^x$) [[9- Big-O-Notation#Polynomial|Jump To Heading]]
		- Exponential - O(x$^n$)


## Constant - O(1)

- Constant complexity is where an algorithm is ran in purely sequency, so no looping/recursion
	- This is the ideal situation in terms of complexity, as it is the fasted for the computer to run, however most algorithms that have a constant complexity will not be able to do very much...






## Logarithmic

* This is also an ideal complexity, as it is present when an algorithm is looped, but after every pass it halves the dataset / load, which leads to it being very efficient
	>	This is seen in the [[2- Binary Search |Binary Search]] , as for each pass, half of the list is cut off, as we know the desired number is not there.



## Linear

- Linear Complexity is where Loops come into play, if a loop will be repeated n number of times, then we say that the complexity scales with a magnitude of n.
	> This is observed in the  [[1- Linear Search | Linear Search]]



## Polynomial

* Polynomial Complexity is often found in nested for loops, where you have a for loop, which is linear, every n times, so it would be n$^2$ complexity.

* Example of an algorithm witch Polynomial complexity
```
for i in range(n):
	for x in range(t):
		print("Bruh")
```



## Exponential




test test

























