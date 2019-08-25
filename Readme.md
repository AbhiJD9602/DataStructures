**Binary Search Tree:-**

1) Do In-Order Traversal of the given tree and store the result in a temp array.
2) Check if the temp array is sorted in ascending order, if it is, then the tree is BST.

Time Complexity: O(n)

We can avoid the use of Auxiliary Array. While doing In-Order traversal, we can keep track of previously visited node.
If the value of the currently visited node is less than the previous value, then tree is not BST.
This BST is space optimized.

**Searching Algorithms :--**

Searching Algorithms are designed to check for an element or retrieve an element from any data structure where it is stored.
Based on the type of search operation, these algorithms are generally classified into two categories:


Sequential Search: In this, the list or array is traversed sequentially and every element is checked.For example: Linear Search.
Interval Search: These algorithms are specifically designed for searching in sorted data-structures.
These type of searching algorithms are much more efficient than Linear Search as they repeatedly target the center of the search structure and divide the search space in half. 
For Example: Binary Search.

**Linear Search :--**

The time complexity of above algorithm is O(n).

Linear search is rarely used practically because other search algorithms such as the binary search algorithm and hash tables allow significantly faster searching comparison to Linear search.


**Binary Search :--**

Two implementation  :--
1. Recusrive
2. Iterative

Time Complexity :- O(Log n)

Space Compleixity for binary search

Recursive :- O(Log n)
Iterative :- O(1)

Algorithmic Paradigm: Decrease and Conquer.


**Sorting :-**

**Selection Sort :-**

The selection sort algorithm sorts an array by repeatedly finding the minimum element (considering ascending order) from unsorted part and putting it at the beginning.
The algorithm maintains two subarrays in a given array.

1) The subarray which is already sorted.
2) Remaining subarray which is unsorted.

In every iteration of selection sort, the minimum element (considering ascending order) from the unsorted subarray is picked and moved to the sorted subarray.

Time complexity :- O(n*n) as there are two nested loops.
Space complexity :- O(1)

The good thing about selection sort is it never makes more than O(n) swaps and can be useful when memory write is a costly operation.

**Bubble Sort :-** 

Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in wrong order.

Worst and Average Case Time Complexity: O(n*n). Worst case occurs when array is reverse sorted.

Best Case Time Complexity: O(n). Best case occurs when array is already sorted.

Auxiliary Space: O(1)

Boundary Cases: Bubble sort takes minimum time (Order of n) when elements are already sorted.

Sorting In Place: Yes

Stable: Yes

**Insertion Sort :-** Insertion sort is a simple sorting algorithm that works the way we sort playing cards in our hands.

Time Complexity: O(n*2)

Auxiliary Space: O(1)

Boundary Cases: Insertion sort takes maximum time to sort if elements are sorted in reverse order. And it takes minimum time (Order of n) when elements are already sorted.

Algorithmic Paradigm: Incremental Approach

Sorting In Place: Yes

Stable: Yes

Online: Yes

**Merge Sort :-**  It divides input array in two halves, calls itself for the two halves and then merges the two sorted halves. 

Time complexity of Merge Sort is \Theta(nLogn) in all 3 cases (worst, average and best) as merge sort always divides the array into two halves and take linear time to merge two halves.

Auxiliary Space: O(n)

Algorithmic Paradigm: Divide and Conquer

Sorting In Place: No in a typical implementation

Stable: Yes

**Heap Sort :-**

Heap sort is a comparison based sorting technique based on Binary Heap data structure.
It is similar to selection sort where we first find the maximum element and place the maximum element at the end.
We repeat the same process for remaining element.


Heap sort is an in-place algorithm.
Its typical implementation is not stable, but can be made stable

Time Complexity: Time complexity of heapify is O(Logn).
Time complexity of createAndBuildHeap() is O(n) and overall time complexity of Heap Sort is O(nLogn).

Applications of HeapSort
1. Sort a nearly sorted (or K sorted) array
2. k largest(or smallest) elements in an array