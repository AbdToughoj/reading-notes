## Hash Tables:

### What is a Hashtable?

A hash table, also known as a hash map, is a data structure that stores key-value pairs. It uses a hashing function to convert a given key into an index where the corresponding value is stored in an array. The primary advantage of hash tables is their ability to perform efficient lookups, insertions, and deletions in constant time on average (O(1)).

### Terminology:

- Hash: A hash is the result of applying a hashing algorithm to a key, converting it into an integer that represents the index in the array where the value will be stored.

- Buckets: Buckets are the storage locations in the array, and each bucket can hold one or more key-value pairs.

- Collisions: Collisions occur when two or more keys produce the same hash value, resulting in the need to store multiple key-value pairs in the same bucket.

### Why do we use Hash Tables?

Hash tables are used to efficiently store and retrieve data, especially in scenarios where fast data access is crucial. They are particularly useful for tasks like searching, caching, and data indexing. Some common use cases for hash tables include:

- Dictionary-like data structures: Hash tables are used to implement dictionaries or associative arrays, where each key corresponds to a specific value.

- Caching: Hash tables can be used for caching frequently accessed data to improve the performance of applications.

- Data indexing: Hash tables help optimize database query times by indexing data based on key values.

Frequency analysis: In various algorithms and data analysis tasks, hash tables are employed to count the frequency of elements.

### Structure of Hash Tables:

- Hashing Process: To create a hash table, the keys are first passed through a hashing function, which generates a hash code. The hash code is then converted into an array index using a modulus operation, ensuring that it falls within the range of the array.

- Collision Handling: Collisions can occur when multiple keys produce the same hash code, leading to the same array index. Hash tables use various collision resolution techniques to handle this situation. Common approaches include using linked lists or open addressing (probing) to store multiple key-value pairs in the same bucket.

### Methods of Hash Tables:

- set(): Adds a new key-value pair to the hash table. It calculates the hash code of the key and stores the pair in the appropriate bucket.

- get(): Retrieves the value associated with a given key from the hash table. It calculates the hash code, finds the appropriate bucket, and searches for the key within the bucket.

- has(): Checks if a specific key exists in the hash table. It calculates the hash code and looks for the key within the corresponding bucket.

- keys(): Returns an array of all unique keys present in the hash table.

### Hashing Algorithm:

A good hashing algorithm is essential to minimize collisions and improve the performance of hash tables. It should be deterministic, meaning that the same key should always produce the same hash code. Common techniques for creating hash codes include summing ASCII values, bitwise operations, and using prime numbers.
