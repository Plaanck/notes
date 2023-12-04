
# Addition rules

- When adding binary numbers, we will have to carry the 1 when there are two 1s, resulting in a 0, same with adding two 0s. Otherwise, we will result with 1. This behavior is reminiscent of the XOR gate.
- On the other hand the carries act like an AND gate, when there are two ones, the result is a 1, but otherwise it remains 0.

XOR GATE

| A | B | C |
|---|---|-- |
| 0 | 0 | 0 |     
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 | 


AND GATE

| A | B | C |
|---|---|-- |
| 0 | 0 | 0 |     
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 | 

- These two together form a **Half adder**, as this does not handle actually adding the carries over, meaning we need more to fully add two numbers