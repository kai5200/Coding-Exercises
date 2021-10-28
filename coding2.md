```python
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

 

Example 1:

Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Output: Because nums[0] + nums[1] == 9, we return [0, 1].
Example 2:

Input: nums = [3,2,4], target = 6
Output: [1,2]
Example 3:

Input: nums = [3,3], target = 6
Output: [0,1]
```


```python
def two_sum(num, target):
    d = {}
    for index, dig in enumerate(nums):
        item = target - dig
        for key, value in d.items():
            if value == item:
                return (key, index)
        d[index] = dig
```


```python
nums = [4, 11, 4, 15, 4, 10, 80]
target =25
result = two_sum(nums, target)
print(result)
```

    (3, 5)



```python
nums = [7, 21, 44, 6, 90, 100, 88]
target =50
result = two_sum(nums, target)
print(result)
```

    (2, 3)



```python

```
