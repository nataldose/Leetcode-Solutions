# 1. Two Sum

## Approach 1: Brute Force
The first thing we can come up with is to check every possiblity of a two number pairing from the given array. One thing we look out for is not to add a number with it self. By these we don't mean not to add two equal numbers. But on the contrary, we can do that provided that they are on different indices or positions in the array.

### Algorithm
1. Initialize two pointers or references to the begining of the array.
2. Fix One of the pointers at the start and move the other one to the end of the array by incrementing one.
3. As You go towards the end of the array check if the two pointers are not pointing to the same position and the values at those positions sum up to the target.
4. When you find it create an array holding the current positions of the indices and return it.

### Complexity Analysis

*__Time Complexity:__ O(n\*n)*

*__Space Complexity:__ O(1)*

__Explanation:__ Since we are not creating any extra space and we only need two variables for the pointers the space complexity will be constant. The time complexity will be quadratic because for each element we are checking if it can be paired with another number and sum up to the target.



## Approach 2: Two pass hashtable
