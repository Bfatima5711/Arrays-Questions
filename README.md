# Arrays-Questions
Common folder for all array questions starting from basics to advance level questions 

//Easy level : question 1 - Remove Duplicates from Sorted Array

Problem Statement: Remove Duplicates from Sorted Array
Given: 
Given an integer array nums sorted in non-decreasing order, remove the duplicates in-place such that each unique element appears only once. The relative order of the elements should be kept the same. Then return the number of unique elements in nums.

Consider the number of unique elements of nums to be k, to get accepted, you need to do the following things:

Change the array nums such that the first k elements of nums contain the unique elements in the order they were present in nums initially. The remaining elements of nums are not important as well as the size of nums.
Return k.

Eg.
Input: nums = [0,0,1,1,1,2,2,3,3,4]
Output: 5, nums = [0,1,2,3,4,_,_,_,_,_]
Explanation: Your function should return k = 5, with the first five elements of nums being 0, 1, 2, 3, and 4 respectively.
It does not matter what you leave beyond the returned k (hence they are underscores).

Time and Space Complexity of below code:

Time Complexity: O(N)
Space Complexity: O(1)

Problem Link: https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/

Note: for code check attached file with name  Remove Duplicates from Sorted Array

//Easy level : question 2 - Two Sum

Problem Statement: Two Sum
Given: 
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

Example 1:

Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

3-Approaches to solve the given question:

Approach 1 - One brute force : In this approach consider every pair of elements and check if their sum equals the target. This can be done using nested loops, 
where the outer loop iterates from the first element to the second-to-last element, and the inner loop iterates from the next element to the
last element. However, this approach has a time complexity of O(n^2).

Approach 2 - Two Pass - Hash Table: A more efficient approach to use a hash table (unordered_map in C++). We can iterate through the array once, and for each element,
check if the target minus the current element exists in the hash table. If it does, we have found a valid pair of numbers. If not, we add the current element to the 
hash table. However, this approach has a time complexity of O(2n) ~= O(n).

Approach 3 - one Pass - Hash Table: In this approach we Create an empty hash table to store elements and their indices. Iterate through the array from left to right.
For each element nums[i], calculate the complement by subtracting it from the target: complement = target - nums[i].Check if the complement exists in the hash table. 
If it does, we have found a solution. If the complement does not exist in the hash table, add the current element nums[i] to the hash table with its index as the value.
Repeat steps 3-5 until we find a solution or reach the end of the array. If no solution is found, return an empty array or an appropriate indicator. This approach has
a time complexity of O(n) since hash table lookups take constant time on average. It allows us to solve the Two Sum problem efficiently by making just one pass through
the array.

Problem Link: https://leetcode.com/problems/two-sum/description/

Note: for code check attached file with name Two Sum

//Easy level : question 3

Problem Statement: X of a Kind in a Deck of Cards
Given:
You are given an integer array deck where deck[i] represents the number written on the ith card.

Partition the cards into one or more groups such that:

Each group has exactly x cards where x > 1, and
All the cards in one group have the same integer written on them.
Return true if such partition is possible, or false otherwise.

 

Example 1:

Input: deck = [1,2,3,4,4,3,2,1]
Output: true
Explanation: Possible partition [1,1],[2,2],[3,3],[4,4].
Example 2:

Input: deck = [1,1,1,2,2,2,3,3]
Output: false
Explanation: No possible partition.

Problem Link: https://leetcode.com/problems/x-of-a-kind-in-a-deck-of-cards/description/

Note: for code check attached file with name X of a Kind in a Deck of Cards


Problem Statement: 3Sum

//medium level : question 4

Given:
Given an integer array nums, return all the triplets [nums[i], nums[j], nums[k]] such that i != j, i != k, and j != k, and nums[i] + nums[j] + nums[k] == 0.

Notice that the solution set must not contain duplicate triplets.

 

Example 1:

Input: nums = [-1,0,1,2,-1,-4]
Output: [[-1,-1,2],[-1,0,1]]
Explanation: 
nums[0] + nums[1] + nums[2] = (-1) + 0 + 1 = 0.
nums[1] + nums[2] + nums[4] = 0 + 1 + (-1) = 0.
nums[0] + nums[3] + nums[4] = (-1) + 2 + (-1) = 0.
The distinct triplets are [-1,0,1] and [-1,-1,2].
Notice that the order of the output and the order of the triplets does not matter.


Problem Link: https://leetcode.com/problems/3sum/description/

Note: for code check attached file with name 3Sum

//medium level : question 5

Problem Statement: Rotate Array

Given:
Given an integer array nums, rotate the array to the right by k steps, where k is non-negative.

 

Example 1:

Input: nums = [1,2,3,4,5,6,7], k = 3
Output: [5,6,7,1,2,3,4]
Explanation:
rotate 1 steps to the right: [7,1,2,3,4,5,6]
rotate 2 steps to the right: [6,7,1,2,3,4,5]
rotate 3 steps to the right: [5,6,7,1,2,3,4]

Problem Link: https://leetcode.com/problems/rotate-array/description/

Note: for code check attached file with name Rotate Array

//Easy level : question 6

Problem Statement: Maximum Product of Three Numbers

Given: 
Given an integer array nums, find three numbers whose product is maximum and return the maximum product.

Example 1:
Input: nums = [1,2,3]
Output: 6

Example 2:
Input: nums = [1,2,3,4]
Output: 24

Example 3:
Input: nums = [-1,-2,-3]
Output: -6

Problem Link: https://leetcode.com/problems/maximum-product-of-three-numbers/description/

Note: for code check attached file with name Maximum Product of Three Numbers

//medium level : question 6

Problem Statement: Subarray Sum Equals K

Given:
Given an array of integers nums and an integer k, return the total number of subarrays whose sum equals to k.
A subarray is a contiguous non-empty sequence of elements within an array.

Example 1:
Input: nums = [1,1,1], k = 2
Output: 2

Example 2:
Input: nums = [1,2,3], k = 3
Output: 2

Problem Link: https://leetcode.com/problems/subarray-sum-equals-k/
Note: for code check attached file with name Subarray Sum Equals K

//medium level : question 7
Problem Statement: Longest Sub-Array with Sum K

Given:
Given an array containing N integers and an integer K., Your task is to find the length of the longest Sub-Array 
with the sum of the elements equal to the given value K.

Example 1:
Input :
A[] = {10, 5, 2, 7, 1, 9}
K = 15
Output : 4
Explanation:
The sub-array is {5, 2, 7, 1}.

Problem Link: https://www.geeksforgeeks.org/problems/longest-sub-array-with-sum-k0809/1

Note: for code check attached file with name Longest Sub-Array with Sum K
