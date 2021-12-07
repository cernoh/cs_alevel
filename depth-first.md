# depth-first search

Uses a [[4.2.3.1 Stacks|stack]] . Used for navigating a maze. 

## example use case- tree:
related : [[4.2.5.1 Trees]]

![[Pasted image 20211207184945.png]]

Can start at any node. Starting at F

![[Pasted image 20211207185051.png]]

F is a new node, so is added to the result and to the stack.

![[Pasted image 20211207185442.png]]
**Result: F**

next nodes adjacent to F are observed, B & G . B is higher alphabetically so B is discovered first

![[Pasted image 20211207185700.png]]

**Result: F B**

A is bigger so its selected instead of D

![[Pasted image 20211207190954.png]]

**Result : F B A **

There are no undiscovered nodes adjacent to A.  Therefore A is popped off the stack and labeled completely explored. Next item is looked at- B.