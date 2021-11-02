```python
#Fibonacci Sequence
#0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, ...
```


```python
def fibo(n):
    a,b = 0,1
    i,result = 0,[]
    while i < n:
        result.append(a)
        a,b = b, a+b
        i += 1
    return result
```


```python
fibo(10)
```




    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]




```python
fibo(15)
```




    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377]




```python

```
