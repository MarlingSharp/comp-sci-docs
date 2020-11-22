# Algorithms

Algorithms are defined as a series of instructions, specific enough that a computer can follow them, with some end condition at which point the algorithm is complete.

For A Level and GCSE, students need to be able to articulate how various algorithms operate \(not necessarily be able to code them though\).

The algorithms you need can be divided into the following categories:

* Searching
* Sorting
* Routing
* Traversal

The traversal algorithms for Trees and Graphs are demonstrated on the [Data Structures](data-structures.md#binary-tree) page. This page will restrict itself to the other families of algorithm. I will not describe the full operation of those algorithms \(this can be found elsewhere\) but I will provide code implementations that can be examined.

## Sorting

### Bubble Sort

Good for short lists, performs badly on large lists. Very simple to code.

{% embed url="https://repl.it/@MarlingSharp/bubble-sort-ts\#index.ts" %}

### Insertion Sort

Similar simplicity as the bubble sort.

{% embed url="https://repl.it/@MarlingSharp/insertion-sort-ts\#index.ts" %}

### Merge Sort

One of the many 'divide and conquer' algorithms.

{% embed url="https://repl.it/@MarlingSharp/merge-sort-ts\#index.ts" %}



### Quick Sort

Sorts a list in place by successively partitioning the data around a pivot.

{% embed url="https://repl.it/@MarlingSharp/quick-sort-ts\#index.ts" %}

## Searching

### Linear Search

By far the simplest search algorithm, just look at every single data item in order until you find a match. Works on unsorted lists. Performance is bad for large lists.

{% embed url="https://repl.it/@MarlingSharp/linear-search-ts\#index.ts" %}

### Binary Search

Much quicker than linear search, but requires the data to be sorted first \(which incurs its own performance cost\).

{% embed url="https://repl.it/@MarlingSharp/binary-search-ts\#index.ts" %}

## Routing

There is one algorithm that you must be familiar with here, it is Dijkstra's routing algorithm, there is also an enhancement of this you need to be able to briefly describe called A\*.

{% embed url="https://repl.it/@MarlingSharp/dijkstras-routing-ts\#Graph.ts" %}



