Lab: Hashing
Objective
The objective of this lab is to explore the concept of hashing, a fundamental technique used in computer science for efficiently retrieving and storing data. In this lab, you will implement and experiment with different hashing techniques and hash functions, and understand their applications in solving common problems like collision handling and optimizing search performance.

Concepts Covered
1. Hash Functions
A hash function takes an input (or "key") and returns a fixed-size string or number that is typically unique to the input. This value is called the hash code or hash value.

Key Points:
A good hash function distributes keys uniformly across the hash table to minimize collisions.
Hash functions should minimize the chance of different inputs producing the same hash value (a collision).
Examples of common hash functions: MD5, SHA-1, SHA-256, and Division method.
2. Hash Tables
A hash table is a data structure that stores key-value pairs. The keys are hashed using a hash function, and the resulting hash value determines where the corresponding value is stored in the table.

Key Points:
A hash table supports efficient O(1) average-time complexity for search, insert, and delete operations.
Collision handling methods are crucial for ensuring that multiple keys can be stored in the same hash table without losing data integrity.
3. Collision Handling Techniques
Since hash functions can sometimes map different keys to the same hash value, it is important to handle collisions effectively. Common methods include:

a. Chaining:
Each hash table entry points to a linked list of entries that hash to the same index.
This method allows multiple elements to be stored at the same index in the table.
b. Open Addressing:
When a collision occurs, the algorithm searches for another open slot in the table using a probing sequence.
Common probing techniques:
Linear Probing: If a collision occurs, check the next slot (i + 1).
Quadratic Probing: If a collision occurs, check the next slot (i + 1^2, i + 2^2, i + 3^2).
Double Hashing: Use a second hash function to compute the next probe location.
Projects and Exercises
1. Implement a Simple Hash Table
Implement a basic hash table using an array.
Use a hash function to calculate the index of each key and store the key-value pair.
Implement collision handling using chaining or open addressing (linear probing).
Features:
Implement insert, search, and delete operations.
Handle collisions using chaining or linear probing.
2. Hashing with Collisions
Modify the hash table implementation to handle collisions.
Experiment with different collision handling techniques: Chaining vs Open Addressing.
Tasks:
Insert keys and values with the same hash values to test collision handling.
Compare the performance of different collision resolution methods in terms of time complexity and memory usage.
3. Hashing in Practical Applications
Apply hashing to solve problems such as:
Duplicate detection: Use hashing to detect duplicate entries in a dataset.
Anagram detection: Use hashing to efficiently check if two strings are anagrams of each other.
Password hashing: Implement a simple password hashing function and understand the concept of salting to make it secure.
4. Performance Testing
Analyze the performance of different hash functions and collision handling techniques.
Measure the average time complexity for search, insert, and delete operations in your hash table.
Test the hash table with varying load factors (number of elements relative to table size) to understand how performance changes.
Tools and Technologies
Programming Language: Python, C++, Java, or any language of your choice.
Libraries: For Python, you can use hashlib for cryptographic hashing functions (e.g., MD5, SHA).
For collision handling: Implement custom hash tables using arrays or linked lists.
Conclusion
Hashing is a key concept in computer science that is widely used for efficient data storage and retrieval. Through this lab, you will learn the practical applications of hash tables, understand the impact of collisions on performance, and experiment with various techniques for collision resolution.

By the end of this lab, you will have gained experience with:

Implementing custom hash tables and hash functions.
Handling hash collisions efficiently.
Understanding real-world applications of hashing.
