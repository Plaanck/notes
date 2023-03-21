## What is a stack?

- A stack is a type of **Abstract** Data Structure, which is defined by the rules we gave it
	>See [[0- Data Types - Introduction|Data Types]] For more on what abstract means

- One key feature of a stack is it's Last-In-First-Out (LIFO) structure.
> The opposite of this, First-In-First-Out is seen in [[3- Queues|Queues]]

- This means that you can only take out what is at the top of the stack.
	> This is an important feature in the Depth-First Search of [[5- Binary Trees|Binary Trees]] and [[6- Graphs|Graphs]] 


-----------------------------------------------------


You can write the code for a stack in two main ways, one centered around lists, and one in an object oriented fashion

Code with Lists-

```
stack = [1,2,3]
MaxItems = 5
numItems = 0

def AddItem(item, stack= stack, MaxItems=MaxItems, numItems=numItems):
    numItems += 1
    if numItems > MaxItems:
        return print("Full")
    stack.append(item)
    return stack
    
def PopItem(stack=stack, numItems=numItems):
    stack.pop()
    numItems -= 1
    return stack
  
def Peek(stack=stack):
    print(stack[-1])


Object Oriented Code-

```


```