Code -
```
def LinearSearch():

    check = False # Flag for whether the item has been found

    index = 0 # an incremental variable for the position in the list

    list = [1,2,3,4,5,6] # dataset containing the numbers we are searching through

    itemtofind = 6#the number that we want to find in the list, it may or may not be in the list

  

    while check == False and index < len(list):#loop with 2 conditions, 1: while the check == false, when it hasnt been found, AND when the item we are checking is a number in the list

        if list[index] == itemtofind:#if statement deciding whether the item we are looking at is the item we want to find

            check = True#if it is the number, we have found the number, so our flag is True

            print(list[index])#prints our found number

        else:#if it has not been found

            index += 1#increment the index to check the next item in the list

    if check == False:#if it was never found

        print("Item not found")#tell the user that the item is not in the list

  

    return list
```

## How It works

- What this algorithm is doing is,
	1. Starting at the 0th index of the list
	2. Checking whether that item is the desired item to find
		1. If not, Check the next index, go back to ^^^
		2. If it is, Stop this loop
	3. Return the desired item to the user




## Efficiency
 **See :** [[9- Big-O-Notation]]



