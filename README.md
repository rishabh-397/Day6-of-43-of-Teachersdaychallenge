# Day6-of-43-of-Teachersdaychallenge
Maximum Subarray
Problem Description: Given an integer array nums, find the subarray with the largest sum, and return its sum. A subarray is a contiguous non-empty sequence of elements within an array.

Approaches Discussed:

Dynamic Programming (Kadane's Algorithm) (O(N) Time Complexity): This is an optimal and highly efficient single-pass solution.

Initialize current_max and global_max (or use a dp array as in the C++ code).

Iterate through the array: For each number, the current_max ending at that position is either the number itself, or the number added to the current_max from the previous position.

Update global_max if current_max exceeds it.

Key Learning Points:

Understanding dynamic programming principles for optimization problems.

Kadane's Algorithm as a classic example of DP for contiguous subarrays.

Solving problems in a single pass (O(N) time complexity).

The idea of building up a solution from smaller subproblems.

Example (from LeetCode):
Input: nums = [-2,1,-3,4,-1,2,1,-5,4]
Output: 6
Explanation: The subarray [4,-1,2,1] has the largest sum 6.



Reverse Linked List
Problem Description: Given the head of a singly linked list, reverse the list, and return the reversed list.

Approaches Discussed:

Iterative Approach (O(N) Time, O(1) Space): This is generally preferred for its constant space complexity. It involves using three pointers: prev, curr, and next_node. curr iterates through the list, prev tracks the reversed portion, and next_node saves the link before curr's next pointer is changed.

Recursive Approach (O(N) Time, O(N) Space due to call stack): A more elegant but potentially less space-efficient solution for very long lists. The base case is an empty list or a single-node list. For other nodes, it recursively reverses the rest of the list and then links the current node to the end of the reversed part.

Key Learning Points:

Fundamental linked list manipulation.

Mastering pointer re-assignments for modifying list structure.

Understanding the trade-offs between iterative and recursive solutions (especially regarding space complexity due to the call stack).

Handling nullptr (or None) checks for robust code.

Example (from LeetCode):
Input: head = [1,2,3,4,5]
Output: [5,4,3,2,1]

