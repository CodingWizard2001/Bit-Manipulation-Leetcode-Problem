# 231. Power of Two

### Description
Given an integer n, return true if it is a power of two. Otherwise, return false.

### Solution

```cpp

bool isPowerOfTwo(int n) {
    if(n <= 0) return false;
    return (n & (n - 1)) == 0;
}

```

### Steps to solution:

- The function first checks if n is less than or equal to 0. If n is less than or equal to 0, it returns false, as negative numbers and zero cannot be powers of two.
- If n is positive, the function uses a bitwise AND operation (&) between n and n - 1. This operation clears the rightmost set bit in n. If the result of this operation is 0, it means that n has only one set bit, indicating that it is a power of two.
- If the result of the bitwise AND operation is 0, the function returns true, indicating that n is a power of two. Otherwise, it returns false.


### Time Complexity:
The time complexity of O(1)

### Space Complexity:
The space complexity is also O(1) 