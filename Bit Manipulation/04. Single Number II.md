# LeetCode Problem: [137. Single Number II](https://leetcode.com/problems/single-number-ii/)

## Problem Description

Given an integer array `nums` where every element appears three times except for one, which appears exactly once. Return the single element that appears only once.

You must implement a solution with a linear runtime complexity and use only constant extra space.

## Solution Approach


To find the single number in the given array where every element appears three times except for one, we can use bitwise manipulation. We iterate through the 32 bits of an integer and count the number of set bits for each bit position. If the count of set bits is not a multiple of three, we set that bit in the result.

## Java Solution

```java
class Solution {
    public int singleNumber(int[] nums) {
       int singleNumber = 0;
       for (int i = 0; i < 32; i++) {
           int setBit = 0;
           for (int j = 0; j < nums.length; j++) {
               if ((nums[j] & (1 << i)) != 0)
                   setBit++;
           }
           if (setBit % 3 != 0)
               singleNumber |= (1 << i);
       }
       return singleNumber;
    }
}
```

## Complexity Analysis

- **Time Complexity**: O(n), where n is the number of elements in the array. We iterate through the array once and for each element, we iterate through 32 bits.
- **Space Complexity**: O(1), as we use only a constant amount of extra space for the variables `singleNumber`, `setBit`, `i`, and `j`.

## Code Explanation
- We initialize the `singleNumber` variable to 0.
- We iterate through each bit position from 0 to 31.
- For each bit position, we count the number of set bits in that position among all elements in the array.
- If the count of set bits is not a multiple of three, we set that bit in the `singleNumber` using bitwise OR.
- Finally, we return the value of `singleNumber`.
