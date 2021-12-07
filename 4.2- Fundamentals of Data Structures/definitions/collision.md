# collision
When different inputs produce the same hash. Can lead to data being overwritten

## example:
when The Shard (310m) is added to the hash table, the key is calculated by the hashing algorithm as 1 (310 MOD 3 = 1) however position 1 is already occupied 

![[Pasted image 20211114142831.png]]

In order to get around the collision, a [[rehashing ]] algorithm is carried out. The next position is inspected, but is occupied, so the algorithm moves onto position 3. 

![[Pasted image 20211114142940.png]]

When The Shard is retrieved from the hash table, the hash is calculated as 1, so the value in position 1 is queried. The value in position 1 is not the requested value, and so the next position is queried. this continues until the desired value is found.
