Hash function is a function where you put in a string and get back a number. 

Hash tables maps keys to values. 

1. It needs to be consistent
2. It should map different words to different numbers

Used in caching, DNS resolution tables, good for filtering out duplicates

**Collision** - two keys assign to the same slot in hash table


Hash tables have O(1) for search, insert and delete at AVERAGE case,
but have O(n) for worst case. 

To avoid worst case you need good hash function to avoid collisions


If load factor (taken slots / all slots) is > 1, then something goes bad and you need to resize the hash table (add more slotes) Usually you doulbe the size of hash function 