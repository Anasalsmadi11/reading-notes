# Hash Tabels

## [Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

### What is a Hashtable?
Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.


### Why do we use them?
Hold unique values
Dictionary
Library

## [basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)


Hashing is a technique used to uniquely identify objects within a group of similar objects. It has practical applications such as assigning unique IDs to students in universities or books in libraries. 

The core steps of hashing involve:

1. Hash Function: A hash function converts a large key into a smaller value, which acts as an index in the hash table.

1. Index Calculation: The hash value is further reduced to an index using the modulo operation (%), making it a number between 0 and the size of the array.

1. Storage: The element associated with the key is stored in the hash table at the calculated index, allowing for quick retrieval.
    
## [hash table wiki](https://en.wikipedia.org/wiki/Hash_table)


A hash table, or hash map, is a data structure that stores key-value pairs using a hash function to map keys to array indexes (buckets). This enables fast data retrieval, insertion, and deletion. Hashing is used in applications like associative arrays, database indexing, caching, sets, and game algorithms.

Hashing can cause collisions (multiple keys mapping to the same index), which are managed using techniques like separate chaining and open addressing. Popular languages provide hash table implementations, such as JavaScript objects, C++ unordered_maps, Python dictionaries, and Java HashMaps. A good hash function is essential for efficient performance. Hash tables are a crucial tool for efficient data storage and retrieval.