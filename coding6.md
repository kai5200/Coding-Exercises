```python
#find medians of num21 and nums2

nums1 = [1, 2, 3, 4, 6]
nums2 = [5,7,9,100]

```


```python
def get_medians(nums1, nums2):
    item = nums1 + nums2
    item.sort()
    count = len(item)

    if count % 2 == 1:
        return (item[count // 2])
    else:
        return ((item[count // 2] + item[count // 2 - 1]) / 2)
```


```python
print(get_medians(nums1, nums2))
```

    5



```python

```
