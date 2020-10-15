# Hash Tables 

 - __Hash__ - The result of some algorithm taking in a string and converting it into a value that will be used to determine the index of an array in a hash table  
 - __Buckets__ - This is what is in each index of the array, containing key value pairs.
 - __Collision__ - This happens when more than one key is hashed to the same location of the hashtable
 - By storing a hashed key, we can quickly retrieve values with O(1) time complexity
 - A hash code turns a key into an integer, and the same key should always produce the same hash code
- To avoid collisions, make each bucket a linked list node, so they will connect if they end up in the same index
- Methods for a hash table include `Add()`, `Find()`, `Contains()`, and `GetHash()`
- One way to make a hash is to add all the ascii values in the key, multiply by a prime number, and then modulo by the length of the array you are using.
