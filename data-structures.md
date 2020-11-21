# Data Structures

## Array

A fixed size set of data items, stored contiguously in memory.

Arrays are 'fixed' data structures, once created they do not generally change size.

* Advantage: Random elements can be accessed quickly
* Disadvantage: The list cannot be easily added to beyond the fixed number of items known at its creation.

## Queue

This is a list of items with a First In First Out logic. There are two key operations

* Enqueue - Place an item on the queue
* Dequeue - Remove an item from the queue, using FIFO

Here is a TypeScript implementation

{% embed url="https://repl.it/@MarlingSharp/queue-ts\#index.ts" %}

## Stack

A stack places items into a dynamic structure with a Last In First Out. There are two key operations:

* Push - Place an item on the stack
* Pop - Remove an item from the stack, using LIFO

Here is an implementation in TypeScript

{% embed url="https://repl.it/@MarlingSharp/stack-ts\#index.ts" %}

## Linked List

Each item contains a pointer to the next item in the list. This allows us to create new items and  simply point to the new locations in memory. 

* Advantage: The list items can be stored anywhere in memory, the structure is highly dynamic.
* Disadvantage: Random access slow, the only way to find items is to a navigate the pointers.

An implementation in TypeScript can be found here, together with a simple program that shows it in operation.

{% embed url="https://repl.it/@MarlingSharp/linked-list-ts\#index.ts" %}

## Hash Table

A hash table attempts to solve both problems, by allocating a fixed array of Linked Lists. When adding items to a hash table, a hash value is calculated for the key of the item, that hash is used to generate an index into the array. The item is then appended to the linked list at that index.

* Advantage - Random access is quicker, the hash effectively narrows down the values to search through to a small proportion of the overall data structure
* Advantage - The structure is dynamic, so items can be easily added and removed
* Disadvantage - A poorly written hash function, or low capacity, can lead to clustering, where lots of items resolve to the same key value and end up with roughly the same problem as a plain linked list.

There is a demonstration of this data structure here:

{% embed url="https://repl.it/@MarlingSharp/hash-table-ts\#index.ts" %}



