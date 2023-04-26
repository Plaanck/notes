
## Code

```
arr = [2,4,1,3,9,6,5,8]

while True:
	swapped = False
	for index in range(0, len(arr)-1):
		if arr[index] > arr[index +1]:
			temp = arr[index]
			arr[index] = arr[index +1]
			arr[index+1] = temp
			swapped = True
		if swapped = False:
			break
```





## How It Works

What this algorithm is doing:
1.  The for loop is going over every item in the array
	1. If the item that is currently being checked is greater than the one after it, it is out of place, so ...
	2. Swap the two numbers and continue going through the list
	3. By the end of each pass, at least one number will now be in place, which will be the largest one (provided you are ordering in ascending order)
2. The algorithm does this over and over until it goes through a pass where no swaps are made, this indicates that the entire array is now sorted, therefore the algorithm is over, and the loop is broken.

## Efficiency


See: [[9- Big-O-Notation|Big O Notation]]