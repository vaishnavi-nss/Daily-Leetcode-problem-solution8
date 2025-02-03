# Daily-Leetcode-problem-solution8
PROBLEM 

You are given an array of integers nums. Return the length of the longest subarray of nums which is either strictly increasing or strictly decreasing.

Intuition

Two Pointers (or Sliding Window-like approach)

Approach

Traverse the array while maintaining two counters:
One for the longest strictly increasing subarray.
Another for the longest strictly decreasing subarray.
If the sequence breaks (i.e., nums[i] is neither increasing nor decreasing), reset the respective counter.
incLength: Tracks the length of the current increasing subarray.
decLength: Tracks the length of the current decreasing subarray.
Whenever an increasing or decreasing sequence is broken, the corresponding counter is reset.
The final result is the maximum of both counters across all elements.

Complexity

Time complexity:
O(n)

Space complexity:
O(1)
