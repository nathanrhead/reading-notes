# Code 401 | Hash Tables

## Class 30 Reading Notes

I. Reading List and Notes

1. [Introduction to Hash Tables, by Paul Programming (YouTube video)]("https://www.youtube.com/watch?v=MfhjkfocRR0")

- Definition: a data structure used to implement an associative array.

- It's smallest unit is made up of two elements: a key and a value or record, e.g., key: name and value: phone number, or, rather, name:phone number.

- Make an associative array by mapping the key to the value and inserting it into one position in an array.

- With a hash function, evaluate the key and return the location where the data we have should be stored in the array, e.g., hash(key) -> [index].

- Chaining: when an array already has a key-value pair at [i], and you have a new key-value pair assigned to the same [i]--called a collision--you can link it to the first key-value pair, apparently as many times as necessary, though if you do it right, the linked, or chain, shouldn't be too long.

2. ["Hashtables"]("https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html")

- Defintion of a hash: the result of an algorithm that receives a string and turns it into another value, e.g., encoded for security purposes or, in the case of a hash table, the index in an array where the value lives or will live.

- Definition of bucket: "A bucket is what is contained in each index of the array of the hashtable."

- Definition of collision: "A collision is what happens when more than one key gets hashed to the same location of the hashtable."

- Definition of a hashtable: A data structure that utilizes a key-value pair to store data and holds that pair at a particular index in an array.

- Defintion of a hash: "the ability to turn the key of a key-value pair into an integer, which will serve as the index position of that pair in an associative array, allowing for a search in constant time (O(1) of the value in the array."

- Definition of deterministic: for a hash code to work for a hashtable, it needs to determine the same integer from the same key every time, since that integer is used to position the key-value pair in the array.

- A good solution for determining the indices of your key-value pairs:

  - Add or multiply all the ASCII values of each letter of your key together.
  - Multiply that number by a prime number, e.g., 599.
  - Use modulo to get the remainder of the result when divided by the total size of the array (e.g., 1024).
  - oila!

- An empty hashtable has key-value pairs with values equal to null.



3. ["Basics of Hash Tables"](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

4. ["Hash table"]("https://en.wikipedia.org/wiki/Hash_table")

II. Assignment: teach one principle you've learned from the above: True or False about Hashtables?

1. *T* or F: the time it takes to find a particular value in a hash table is O(1).

2. *T* of F: a hashtable is another type of data structure, like an array or a tree.

3. T of *F*: hashtables are native to JavaScript.

4. *T* of F: hashtables may use both arrays and linked lists in their makeup.

5. T of *F*: a collision, or overlapping of indices, should be avoided with "detour code" in your hash table.

6. *T* or F: assigning mulitple nodes to one index is called "chaining."

7. T or *F*: each index of a hashtable is called a "mug?" (It's actually called a "bucket, because, when set up with a linked list, it can hold multiple key-value pairs.")

8. *T* of F: an empty hashtable has key-value pairs with values equal to null.

9. T or *F*: a perfect hash has multiple collisions.

10. *T* or F: collisions may be resolved by using linked lists.

[<--back](401week6.md)

[<--home-->](../../README.md)
