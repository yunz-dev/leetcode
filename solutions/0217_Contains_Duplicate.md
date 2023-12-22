# Intuition
<!-- Describe your first thoughts on how to solve this problem. -->
First thought was to make another array but time complexity would be fail.
# Approach
Iterate through array, check if in hashmap. If it is then it there is a duplicate otherwise keep going.

# Complexity
- Time complexity:
O(n)

- Space complexity:
O(n)

# Code
```
class Solution(object):
    def containsDuplicate(self, nums):
        hashset = set()

        for n in nums:
            if n in hashset:
                return True
            else:
                hashset.add(n)
        return False
```
