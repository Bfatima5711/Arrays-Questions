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


//Easy level : question 4

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



//Easy level : question 5

Problem Statement: Check if Array Is Sorted and Rotated

Given: 
Given an array nums, return true if the array was originally sorted in non-decreasing order, then rotated some number of positions 
(including zero). Otherwise, return false.

There may be duplicates in the original array.

Note: An array A rotated by x positions results in an array B of the same length such that A[i] == B[(i+x) % A.length], where % 
is the modulo operation.

Example 1:
Input: nums = [3,4,5,1,2]
Output: true
Explanation: [1,2,3,4,5] is the original sorted array.
You can rotate the array by x = 3 positions to begin on the the element of value 3: [3,4,5,1,2].

Example 2:
Input: nums = [2,1,3,4]
Output: false
Explanation: There is no sorted array once rotated that can make nums.

Constraints:

1 <= nums.length <= 100
1 <= nums[i] <= 100

Problem Link: https://leetcode.com/problems/check-if-array-is-sorted-and-rotated/description/

Note: for code check attached file with name Check if Array Is Sorted and Rotated


//Easy level : question 6

Problem Statement: Pick from both sides!

Given: 
Given an integer array A of size N.
You have to pick exactly B elements from either left or right end of the array A to get the maximum sum.
Find and return this maximum possible sum.
NOTE: Suppose B = 4 and array A contains 10 elements then
You can pick the first four elements or can pick the last four elements or can pick 1 from the front and 
3 from the back etc. you need to return the maximum possible sum of elements you can pick.

Problem Constraints
1 <= N <= 105
1 <= B <= N
-103 <= A[i] <= 103

Input Format
First argument is an integer array A.
Second argument is an integer B.

Output Format
Return an integer denoting the maximum possible sum of elements you picked.

Example Input
Input 1:
 A = [5, -2, 3 , 1, 2]
 B = 3

Input 2:
 A = [1, 2]
 B = 1

Example Output
Output 1:
 8
Output 2:
 2

Example Explanation
Explanation 1:Pick element 5 from front and element (1, 2) from back so we get 5 + 1 + 2 = 8
Explanation 2:Pick element 2 from end as this is the maximum we can get

Problem Link: https://www.interviewbit.com/problems/pick-from-both-sides/

Note: for code check attached file with name Pick from both sides!

//Easy level : question 7

Problem Statement: Best Time to Buy and Sell Stock

Given:
You are given an array prices where prices[i] is the price of a given stock on the ith day.

You want to maximize your profit by choosing a single day to buy one stock and choosing a different
day in the future to sell that stock.

Return the maximum profit you can achieve from this transaction. If you cannot achieve any profit, 
return 0.

Example 1:
Input: prices = [7,1,5,3,6,4]
Output: 5
Explanation: Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = 6-1 = 5.
Note that buying on day 2 and selling on day 1 is not allowed because you must buy before you sell.

Example 2:
Input: prices = [7,6,4,3,1]
Output: 0
Explanation: In this case, no transactions are done and the max profit = 0.
 

Constraints:
1 <= prices.length <= 105
0 <= prices[i] <= 104 

Problem Link: https://leetcode.com/problems/best-time-to-buy-and-sell-stock/description/

Note: for code check attached file with name Best Time to Buy and Sell Stock


//Easy level : question 8

Problem Statement: Majority Element

Given: 
Given an array nums of size n, return the majority element.

The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority 
element always exists in the array.

Example 1:
Input: nums = [3,2,3]
Output: 3

Example 2:
Input: nums = [2,2,1,1,1,2,2]
Output: 2

Constraints:
n == nums.length
1 <= n <= 5 * 104
-109 <= nums[i] <= 109

Problem Link: https://leetcode.com/problems/majority-element/description/

Note: for code check attached file with name Majority Element

//medium level : question 1

Problem Statement: 3Sum
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

//medium level : question 2

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

//medium level : question 3

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

//medium level : question 4
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

//Medium level : question 4

Problem Statement: Minimum sum

Given:
Given an array Arr of size N such that each element is from the range 0 to 9. Find the minimum possible sum of two numbers formed 
using the elements of the array. All digits in the given array must be used to form the two numbers.

Example 1:
Input:
N = 6
Arr[] = {6, 8, 4, 5, 2, 3}
Output: 604
Explanation: The minimum sum is formed 
by numbers 358 and 246.

Example 2:
Input:
N = 5
Arr[] = {5, 3, 0, 7, 4}
Output: 82
Explanation: The minimum sum is 
formed by numbers 35 and 047.

Your Task:
You don't need to read input or print anything. Your task is to complete the function solve() which takes arr[] and n as input 
parameters and returns the minimum possible sum. As the number can be large, return string presentation of the number without 
leading zeroes.

Expected Time Complexity: O(N*logN)
Expected Auxiliary Space: O(N)

Constraints:
1 ≤ N ≤ 107
0 ≤ Arri ≤ 9

Problem Link: https://www.geeksforgeeks.org/problems/minimum-sum4058/1

Note: for code check attached file with name Minimum sum


//Medium level : question 5

Problem Statement: Sort Colors

Given:
Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, 
with the colors in the order red, white, and blue.
We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively.
You must solve this problem without using the library's sort function.

Example 1:
Input: nums = [2,0,2,1,1,0]
Output: [0,0,1,1,2,2]

Example 2:
Input: nums = [2,0,1]
Output: [0,1,2]
 
Constraints:
n == nums.length
1 <= n <= 300
nums[i] is either 0, 1, or 2.

Problem Link: https://leetcode.com/problems/sort-colors/description/

Note: for code check attached file with name Sort Colors 


//Medium level : question 6

Problem Statement: Maximum Subarray

Given:
Given an integer array nums, find the subarray with the largest sum, and return its sum.

Example 1:
Input: nums = [-2,1,-3,4,-1,2,1,-5,4]
Output: 6
Explanation: The subarray [4,-1,2,1] has the largest sum 6.

Example 2:
Input: nums = [1]
Output: 1
Explanation: The subarray [1] has the largest sum 1.

Constraints:
1 <= nums.length <= 105
-104 <= nums[i] <= 104

Problem Link: https://leetcode.com/problems/maximum-subarray/description/

Note: for code check attached file with name Maximum Subarray

//Medium level : question 7

Problem Statement: Next Permutation

Given:
A permutation of an array of integers is an arrangement of its members into a sequence or linear order.
For example, for arr = [1,2,3], the following are all the permutations of arr: [1,2,3], [1,3,2], [2, 1, 3], 
[2, 3, 1], [3,1,2], [3,2,1].

The next permutation of an array of integers is the next lexicographically greater permutation of its integer. 
More formally, if all the permutations of the array are sorted in one container according to their lexicographical 
order, then the next permutation of that array is the permutation that follows it in the sorted container. 
If such arrangement is not possible, the array must be rearranged as the lowest possible order 
(i.e., sorted in ascending order).

For example, the next permutation of arr = [1,2,3] is [1,3,2].
Similarly, the next permutation of arr = [2,3,1] is [3,1,2].
While the next permutation of arr = [3,2,1] is [1,2,3] because [3,2,1] does not have a lexicographical larger 
rearrangement.

Given an array of integers nums, find the next permutation of nums.

The replacement must be in place and use only constant extra memory. 

Example 1:
Input: nums = [1,2,3]
Output: [1,3,2]

Example 2:
Input: nums = [3,2,1]
Output: [1,2,3]

Example 3:
Input: nums = [1,1,5]
Output: [1,5,1]
 
Constraints:
1 <= nums.length <= 100
0 <= nums[i] <= 100

Problem Link: https://leetcode.com/problems/next-permutation/description/

Note: for code check attached file with name Next Permutation

//Medium level : question 8

Problem Statement: Rearrange Array Elements by Sign

Given:
1. You are given a 0-indexed integer array nums of even length consisting of an equal number of positive and negative integers.

2. You should return the array of nums such that the the array follows the given conditions:
	1.Every consecutive pair of integers have opposite signs.
	2.For all integers with the same sign, the order in which they were present in nums is preserved.
	3.The rearranged array begins with a positive integer.
3. Return the modified array after rearranging the elements to satisfy the aforementioned conditions.

Example 1:
Input: nums = [3,1,-2,-5,2,-4]
Output: [3,-2,1,-5,2,-4]
Explanation:
The positive integers in nums are [3,1,2]. The negative integers are [-2,-5,-4].
The only possible way to rearrange them such that they satisfy all conditions is [3,-2,1,-5,2,-4].
Other ways such as [1,-2,2,-5,3,-4], [3,1,2,-2,-5,-4], [-2,3,-5,1,-4,2] are incorrect because they do not satisfy one or more conditions.  

Constraints:
1. 2 <= nums.length <= 2 * 105
2. nums.length is even
3. 1 <= |nums[i]| <= 105
4. nums consists of equal number of positive and negative integers. 

It is not required to do the modifications in-place.

Problem Link: https://leetcode.com/problems/rearrange-array-elements-by-sign/description/

Note: for code check attached file with name Rearrange Array Elements by Sign

//Medium level : question 9

Problem Statement: Merge Intervals

Given:
Given an array of intervals where intervals[i] = [starti, endi], merge all overlapping intervals, and return an array of the non-overlapping intervals that cover all the intervals in the input.

Example 1:
Input: intervals = [[1,3],[2,6],[8,10],[15,18]]
Output: [[1,6],[8,10],[15,18]]
Explanation: Since intervals [1,3] and [2,6] overlap, merge them into [1,6].

Example 2:
Input: intervals = [[1,4],[4,5]]
Output: [[1,5]]
Explanation: Intervals [1,4] and [4,5] are considered overlapping.

Constraints:
1 <= intervals.length <= 104
intervals[i].length == 2
0 <= starti <= endi <= 104

Problem Link: https://leetcode.com/problems/merge-intervals/description/

Note: for code check attached file with name Merge Intervals

//Medium level : question 10

Problem Statement: Find Missing And Repeating

Given:
Given an unsorted array Arr of size N of positive integers. One number 'A' from set {1, 2,....,N} is missing and one number 'B' occurs twice in array. Find these two numbers.

Example 1:
Input:
N = 2
Arr[] = {2, 2}
Output: 2 1
Explanation: Repeating number is 2 and 
smallest positive missing number is 1.

Example 2:
Input:
N = 3
Arr[] = {1, 3, 3}
Output: 3 2
Explanation: Repeating number is 3 and 
smallest positive missing number is 2.

Your Task:
You don't need to read input or print anything. Your task is to complete the function findTwoElement() which takes the array of integers arr and n as parameters and returns an array of integers of size 2 denoting the answer ( The first index contains B and second index contains A.)

Expected Time Complexity: O(N)
Expected Auxiliary Space: O(1)

Constraints:
2 ≤ N ≤ 105
1 ≤ Arr[i] ≤ N

Problem Link: https://www.geeksforgeeks.org/problems/find-missing-and-repeating2512/1

Note: for code check attached file with name Find Missing And Repeating

//Medium level : question 11

Problem Statement: Longest Consecutive Sequence

Given:
Given an unsorted array of integers nums, return the length of the longest consecutive elements sequence.
You must write an algorithm that runs in O(n) time.

Example 1:
Input: nums = [100,4,200,1,3,2]
Output: 4
Explanation: The longest consecutive elements sequence is [1, 2, 3, 4]. Therefore its length is 4.

Example 2:
Input: nums = [0,3,7,2,5,8,4,6,0,1]
Output: 9 

Constraints:
0 <= nums.length <= 105
-109 <= nums[i] <= 109

Problem Link: https://leetcode.com/problems/longest-consecutive-sequence/description/

Note: for code check attached file with name Longest Consecutive Sequence

//Medium level : question 12

Problem Statement: 4Sum

Given:
Given an array nums of n integers, return an array of all the unique quadruplets [nums[a], nums[b], nums[c], nums[d]] such that:
0 <= a, b, c, d < n
a, b, c, and d are distinct.
nums[a] + nums[b] + nums[c] + nums[d] == target
You may return the answer in any order.

Example 1:
Input: nums = [1,0,-1,0,-2,2], target = 0
Output: [[-2,-1,1,2],[-2,0,0,2],[-1,0,0,1]]

Example 2:
Input: nums = [2,2,2,2,2], target = 8
Output: [[2,2,2,2]]

Constraints:
1 <= nums.length <= 200
-109 <= nums[i] <= 109
-109 <= target <= 109

Problem Link: https://leetcode.com/problems/4sum/description/

Note: for code check attached file with name 4Sum

//Medium level : question 13

Problem Statement: Count the subarrays having product less than k

Given:
Given an array of positive numbers, the task is to find the number of possible contiguous subarrays having product less than a given number k.

Example 1:
Input : 
n = 4, k = 10
a[] = {1, 2, 3, 4}
Output : 
7
Explanation:
The contiguous subarrays are {1}, {2}, {3}, {4} 
{1, 2}, {1, 2, 3} and {2, 3}, in all these subarrays
product of elements is less than 10, count of
such subarray is 7.
{2,3,4} will not be a valid subarray, because 
2*3*4=24 which is greater than 10.

Example 2:
Input:
n = 7 , k = 100
a[] = {1, 9, 2, 8, 6, 4, 3}
Output:
16

Your Task:  
You don't need to read input or print anything. Your task is to complete the function countSubArrayProductLessThanK() which takes the array a[], its size n and an integer k as inputs and returns the count of required subarrays.

Expected Time Complexity: O(n)
Expected Auxiliary Space: O(1)

Constraints:
1<=n<=106
1<=k<=1015
1<=a[i]<=105

Problem Link: https://www.geeksforgeeks.org/problems/count-the-subarrays-having-product-less-than-k1708/1

Note: for code check attached file with name Count the subarrays having product less than k

//Medium level : question 14

Problem Statement: Maximum Product Subarray

Given:
Given an integer array nums, find a subarray that has the largest product, and return the product.
The test cases are generated so that the answer will fit in a 32-bit integer.

Example 1:
Input: nums = [2,3,-2,4]
Output: 6
Explanation: [2,3] has the largest product 6.

Example 2:
Input: nums = [-2,0,-1]
Output: 0
Explanation: The result cannot be 2, because [-2,-1] is not a subarray.
 
Constraints:
1 <= nums.length <= 2 * 104
-10 <= nums[i] <= 10
The product of any prefix or suffix of nums is guaranteed to fit in a 32-bit integer.

Problem Link: https://leetcode.com/problems/maximum-product-subarray/description/

Note: for code check attached file with name Maximum Product Subarray
