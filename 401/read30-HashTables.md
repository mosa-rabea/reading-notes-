# Hash tables :
A Hashtable is an array of a list. Each list is known as a bucket,
The position of the bucket is identified by calling the hashcode() method,
A Hashtable contains values based on the key. Java Hashtable class contains unique elements.

## Terminology

+ Hash: its the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose.

+ Buckets: its what contained in each index of the array of the hashtable.

+ Collisions: what happens when more than one key gets hashed to the same location of the hashtable.


### reasone why we use hash tables

1. Hold unique values
2. Dictionary
3. Library

## Structure

+ when it comes to hashing, a hash code turns a key into an integer.
+  hash codes are deterministic: their output is determined only by their input.
+   Hash codes should never have randomness to them. 
+   The same key should always produce the same hash code.

+ Each index of the array can hold many types of values.

+ Each Index of the array contain “buckets”. Each of these “buckets” holds one key/value pair combination.

### how hash table store a value:

1. accept a key
2. calculate the hash of the key
3. use modulus to convert the hash into an array index
4. store the key with the value by appending both to the end of a linked list

### how hash table read a value:

1. accept a key
2. calculate the hash of the key
3. use modulus to convert the hash into an array index
4. use the array index to access the short LinkedList representing a bucket
5. search through the bucket looking for a node with a key/value pair that matches the key you were given

### Internal Methods

1. Add(): When adding a new key/value pair to a hashtable.

2. Find(): The Find takes in a key, gets the Hash, and goes to the index location specified.

3. Contains(): accept a key, and return a bool on if that key exists inside the hashtable.

4. GetHash(): accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

