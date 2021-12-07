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

![[Pasted image 20211207191218.png]]
**Result : F B A **

![[Pasted image 20211207191255.png]]
.**Result : F B A **

B has adjacent undiscovered node.

![[Pasted image 20211207191403.png]]
**Result : F B A D **

D has two adjacent modes, C and E , and C is less than so discovered first.

![[Pasted image 20211207191549.png]]
**Result : F B A D C**

C is completely explored so is popped off and D is revisited.

![[Pasted image 20211207191830.png]]
**Result : F B A D C**

D is adjacent to E

![[Pasted image 20211207191919.png]]
**Result : F B A D C E**

E is now completely explored, so next item on stack is visited.

![[Pasted image 20211207192052.png]]
**Result : F B A D C E **

D is completely explored, so its popped off and B is revisited

![[Pasted image 20211207192252.png]]
**Result : F B A D C E **

B is completely explored. B is popped off and F is revisited.

![[Pasted image 20211207192423.png]]
**Result : F B A D C E **

F has an adjacent undiscovered node. G is discovered and added to stack.

![[Pasted image 20211207192542.png]]
**Result  : F B A D C E G **

H is only undiscovered node adjacent to G 

![[Pasted image 20211207192653.png]]
**Result : F B A D C E G H**
