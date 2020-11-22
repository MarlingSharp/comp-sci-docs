# Data Structures

## Array

A fixed size set of data items, stored contiguously in memory.

Arrays are 'fixed' data structures, once created they do not generally change size.

* Advantage: Random elements can be accessed quickly
* Disadvantage: The list cannot be easily added to beyond the fixed number of items known at its creation.

## Multi-Dimensional Array

Arrays can be nested \(arrays of arrays\) to create multi-dimensional arrays. This can be used to represent 2D or 3D structures. 

Here is a simple program that defines a couple of multi-dimensional arrays, just to show the syntax of declaring them and addressing their data.

{% embed url="https://repl.it/@MarlingSharp/multi-dim-array-ts\#index.ts" %}

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

## Binary Tree

This is a tree structure, but each node can only have 2 children, and the Left and Right children have specific relationships with their parent node. Most often the left branch is 'less than' and the right branch contains nodes that are 'more than'.

When values are added to a binary tree, they are placed by deciding if the new node is 'less than' or 'greater than' each node. Once it reaches a leaf node, it attaches itself at the appropriate point.

Once a binary tree has been built, there are three traversal algorithms that one must be aware of:

* In-Order - Visit the left branch, then the node, then the right branch.
* Pre-Order - Visit the node, then left branch, then right branch
* Post-Order - Visit the left branch, right branch, then the node.

Here is an implementation of the Binary Tree data structure, and those three traversal algorithms

{% embed url="https://repl.it/@MarlingSharp/binary-tree-ts\#index.ts" %}

## Graph

Graph's look a lot like trees, in that nodes are connected by links, but there are a couple of key differences.

* Graphs permit links between any given nodes, so there can be loops and there can be more than 2 links going out from any given node.
* Relationships between nodes can be specialised in the following ways
  * Weighted - Given some numerical value, this could relate to strength of relationship, or the physical distance between two navigation points.
  * Directed - The link only goes in one specific direction, social graphs might show person A following B, but B does not follow A.

Once you have built a graph, there are a couple of traversal algorithms which you can use. Traversal algorithms have the following characteristics:

* They require a start vertex to be nominated when invoked
* They should visit every node that is connected to the start node \(direct or transitively\)

The two algorithms are:

* Depth First Search - Drill down a branch until you hit a leaf node, then double back and find the next path to go down. Repeat until all links have been exhausted. Uses a Stack to implement.
* Breadth First Search - Visit the node, then all its children, then all their children, radiating outwards until all links exhausted. Uses a Queue to implement.

An implementation of Graph and it's two traversal algorithms can be found here

{% embed url="https://repl.it/@MarlingSharp/graph-ts\#index.ts" %}



