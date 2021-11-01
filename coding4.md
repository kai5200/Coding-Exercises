```python
def find_odd(a):
    odds = []
    for i in a:
        if i % 2 == 1:
            odds.append(i)
    return odds
```


```python
find_odd([10,9,8,7,6,5,4,3,2])
```




    [9, 7, 5, 3]




```python
def find_odd1(a):
    return[i for i in a if i % 2 ==1]
```


```python
find_odd1([10,9,8,7,6,5,4,3,2])
```




    [9, 7, 5, 3]




```python

```
