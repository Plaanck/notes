
## Iterative Code
```
list = [1,2,3,4,5,6,7,8,9]
NumToFind = 4
flag = False
lowerBound = 0
upperBound = len(list) - 1

while lowerBound <= upperBound and flag == False:
	midPoint = list[(upperBound+lowerBound) // 2]
	if numToFind == midPoint:
		flag = True
	if list[midPoint] < NumToFind:
		lowerBound = midpoint + 1
	else:
		upperBound = midpoint - 1

if flag == True:
	print("found")
```


## Recursive Code

```
arr = [1,2,3,4,5,6,7,8,9]

  

def BinarySearch(arr,DesiredNum,upperBound, lowerBound=0):

    if upperBound <= lowerBound:

        return

    midPoint= (lowerBound + upperBound) //2

  

    if arr[midPoint] == DesiredNum:

        return print(DesiredNum)

    elif arr[midPoint] > DesiredNum:

        return BinarySearch(arr, DesiredNum, midPoint-1, lowerBound)

    elif arr[midPoint] < DesiredNum:

        return BinarySearch(arr, DesiredNum, upperBound, midPoint+1)

  

BinarySearch(arr, 3, len(arr)-1)
```














## How It Works

- This algorithm works by eliminating half of the dataset for each check it does
>	This Makes it Very efficient in Large datasets, See [[2- Binary Search#Efficiency]]
- Essentially, what it is doing is:
	1. Find the midpoint of the list, and make the upper bound one less than the length of the list, and the lower bound 0.
	2. Then see if the midpoint is smaller than, less than or equal to the desired number
		1. If it is equal to the desired number, stop the loop
		2. If it is greater than the desired number, make the Upper bound equal to one less than the midpoint (This is because we know the midpoint is not the desired number, so we skip checking it again)
		3. If it is less than the desired number, make the Lower bound equal to one more than the midpoint, for the same reasons as above



## Efficiency

[[9- Big-O-Notation#Logarithmic |Logarithmic Effieciency]]