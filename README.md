# Partitioning-and-Sorting-Arrays-with-Many-Repeated-Entries

Question>>

Consider a big array where elements are from a small set and in any range, i.e. there are many repetitions. How to efficiently sort the array?

Examples>>

Example: 
Input:  arr[] = {100, 12, 100, 1, 1, 12, 100, 1, 12, 100, 1, 1}
Output: arr[] = {1, 1, 1, 1, 1, 12, 12, 12, 100, 100, 100, 100}

APPROACH>>

A Basic Sorting algorithm like MergeSort, HeapSort would take O(nLogn) time where n is number of elements
TC = O(nlogn)

A Better Solution is to use Self-Balancing Binary Search Tree like AVL or Red-Black to sort in O(n Log m) time where m is number of distinct elements. The idea is to extend tree node to have count of keys also. ((LATER))
TC = O(logn)
