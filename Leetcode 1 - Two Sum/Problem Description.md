# [1. Two Sum](https://leetcode.com/problems/two-sum)
### Easy

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.


__Example 1:__

>__Input:__ nums = [1, 2, 3, 4];  target = 9

>__Output:__ [0, 1]

__Example 2:__

>__Input:__ nums = [3, 2, 4];  target = 6

>__Output:__ [1, 2]

__Example 3:__

>__Input:__ nums = [3,3];  target = 6

>__Output:__ [0, 1]


#### __Constraints:__


- 2 <= nums.length <= 10,000
- -1,000,000,000 <= nums[i] <= 1,000,000,000
- -1,000,000,000 <= target <= 1,000,000,000
- __*Only One valid Answer Exists*__

#### __Follow Up:__ Can You come up with an algorithm that is less than O(n*n) time complexity?



### Topics: Array, Hashtable




__Hint 1:__ A really brute force way would be to search for all possible pairs of numbers but that would be too slow. Again, it's best to try out brute force solutions for just for completeness. It is from these brute force solutions that you can come up with optimizations.

__Hint 2:__ So, if we fix one of the numbers, say x, we have to scan the entire array to find the next number y which is value - x where value is the input parameter. Can we change our array somehow so that this search becomes faster?

__Hint 3:__ The second train of thought is, without changing the array, can we use additional space somehow? Like maybe a hash map to speed up the search?