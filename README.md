# LeetCode-Bit-Manipulation Problem Solutions

Welcome to the **LeetCode Bit Manipulation Problems Solutions Repository!** This repository contains Java solutions for 
**Important Bit Manipulation Problems** on LeetCode. You can find the [Bit Manipulation Problems List here
](https://github.com/SwarajShelavale/LeetCode-Bit-Manipulation/tree/main/Bit%20Manipulation)

Each solution is accompanied by **Detailed Explanations, Intuitive Approaches, and Time Complexity Analyses** to help you master the art of bit manipulation.


## Bit Manipulation Formulas

1. **Create a number with Kth Set bit as digit:** `1 << (k - 1)`
2. **Set Kth bit in the number:** `n | (1 << (k - 1))`
3. **Check if Kth bit is Set or Not:** `n & (1 << (k - 1))`
4. **Unset Kth bit in the number:** `n & ~(1 << (k - 1))`
5. **Toggle the Kth Bit of the Number:** `n ^ (1 << (k - 1))`
6. **Count of Bits:** `(int)(Math.log(n) / Math.log(2) + 1)`
7. **Count of Set Bits:** `Integer.bitCount(n)`
8. **Find LSB (Lowest Set Bit):** `n = n & ~(n - 1)`
9. **Clear all bits from the most significant bit through the Kth bit inclusive:** `n & ((1 << k) - 1)`
10. **Clear all bits from the Kth bit through 0th bit inclusive:** `n & ~((1 << (k + 1)) - 1)`
11. **Check if a number is a power of 2:** `(n & (n - 1)) == 0`
12. **Set all bits from the most significant bit through the Kth bit inclusive:** `n | ((1 << (k + 1)) - 1)`
13. **Clear the rightmost set bit:** `n & (n - 1)`
14. **Get the value of the rightmost set bit:** `n & -n`
15. **Check if the number is even or odd:** `(n & 1) == 0` for even, `(n & 1) == 1` for odd
16. **Swap two numbers using XOR:** 
    ```java
    a = a ^ b;
    b = a ^ b;
    a = a ^ b;
    ```

## List of Important Bit Manipulation Problems

1. [Number of 1 Bits](https://leetcode.com/problems/number-of-1-bits/)
2. [Sum of Two Integers](https://leetcode.com/problems/sum-of-two-integers/)
3. [Single Number](https://leetcode.com/problems/single-number/)
4. [Single Number II](https://leetcode.com/problems/single-number-ii/)
5. [Majority Element](https://leetcode.com/problems/majority-element/)
6. [Reverse Bits](https://leetcode.com/problems/reverse-bits/)
7. [Single Number III](https://leetcode.com/problems/single-number-iii/)
8. [Hamming Distance](https://leetcode.com/problems/hamming-distance/)
9. [Divide Two Integers](https://leetcode.com/problems/divide-two-integers/)
10. [Decode XORed Permutation](https://leetcode.com/problems/decode-xored-permutation/)
11. [Minimum One Bit Operations to Make Integers Zero](https://leetcode.com/problems/minimum-one-bit-operations-to-make-integers-zero/)
12. [XOR Queries of a Subarray](https://leetcode.com/problems/xor-queries-of-a-subarray/)
13. [Minimum Number of Bit Flips to Convert Number](https://leetcode.com/problems/minimum-number-of-flips-to-convert-binary-matrix-to-zero-matrix/)
14. [Subsets](https://leetcode.com/problems/subsets/)
15. [Pow(x, n)](https://leetcode.com/problems/powx-n/)

## Accessing Solutions

To access the solutions for each problem, simply click on the respective problem title. Each problem has its own markdown file which contains the `Problem Link`, `Description`, `Solution Approach`, `Java Code`, `Complexity Analysis`, and `Code Explanation`.

## Contribution

Contributions to this repository are welcome! If you have alternative solutions or improvements to existing solutions, feel free to open a pull request.

For any queries, please feel free to reach out to me at `shelavaleswaraj1610@gmail.com`.
