
# The basics

- Firstly, we have to think about whether a problem can be computable, given that there is an appropriate algorithm
	- A problem is considered **Computable** if an algorithm is able to solve it
- Some problems can not be solved by algorithms, 
	- This is mostly due to limitations in hardware such as not enough memory, or not a strong enough processor

- Problems also need to be **Clearly Defined**, meaning you should understand your current position in the problem, the end goal and the potential obstacles



## Problem Recognition

- Problem recognition consists of being able to fully recognize what a problem actually is, such as
	- Being able to define it
	- Being able to find the cause
	- Being able to tell if you can even feasibly solve the problem
	- What is the most efficient way to solve it?


## Decomposition

- Decomposition is the method of breaking a problem down into smaller, much more easier to manage problems.

- Structure diagrams are an approach to decomposition in a hierarchical approach
	- However not all problems are easily broke down this way, such as event-driven programs, normally based around GUI's


## Divide and Conquer

- This is a method where you normally
	1) Take a dataset
	2) Apply some rules
	3) Based on the outcome, discard unmatching data
	4) Repeat until desired result

	This is seen well in the [[2- Binary Search|Binary Search]]

## Abstraction

- Abstraction is the process of separating ideas from reality/hiding necessary details and highlighting the ones that are useful to the user
	- One Classic example of abstraction is maps, as they hide details, e.g. it's a simplified overview of the area, rather than a satellite image, but highlight other things, e.g. icons showing points of interest, because this is useful to the user.


## Backtracking

- This is the process of incrementally building to solving an issue, and giving up on attempts that will not solve the issue, and returning to a state where it worked
	- This is not a suitable approach to all problems, but problems such as pathfinding use backtracking particularly well, especially in depth first searches
		See [[8- Astar Algorithm|A* Algorithm]]: Showing how backtracking can be used, as well as [[5- Binary Trees|Binary Tree]] For depth first search.

## Data Mining

- Data mining is the concept of analyzing large amounts of data from all across the internet to discover trends and more information about the topic
	- This is associated with the concept of Big Data (extremely large datasets)

- Data mining is seen in applications such as:
	- Weather modelling
	- Business and economics
	- Stocks
	- Science and engineering
	- Medical research
	- Law enforcement

## Heuristics

- Heuristics are at it's core just using estimation and experience to get a solution to a problem that is "good enough"
- They are pretty much just educated guesses based on some previous data or some set of rules
	This is seen in the [[8- Astar Algorithm|A* Algorithm]]

## Performance Modelling

- The process of approximating how well models perform using maths.
	- This uses simulation and approximation rather than detailed testing, as that would be very inefficient in terms of time and cost - (See: [[9- Big-O-Notation|Big O Notation]]) 

- You can do exhaustive testing, e.g. to check a cloud server ad full capacity by sending millions of requests. Or you could monitor how it handles smaller user bases, and use modelling to estimate how it would perform under high stress
	- This is often done in game development of multiplayer games during beta testing.
		- They can limit the servers to a smaller user base, and use performance modelling to calculate if the servers will be able to handle the full player base


## Pipelining

- Splitting a large task into manageable chunks and overlapping them to speed up the overall process
	- E.G. In the [[1.2 - Fetch Decode Execute Cycle|Fetch Decode Execute Cycle]], one core could be fetching an instruction while other cores are either decoding or executing
- More specifically, Pipelining is allowing the result of one process to feed into the processing of another process.
	- E.g. The result of a game character touching an enemy leads into the reducing of the character's health.
