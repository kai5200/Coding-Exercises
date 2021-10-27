```python
#there is a array, full of 0 and 1 
#outpu format[0,0,0,0,1,1,1]
#example [1,0,1,0] >>> [0,0,1,1]

a = [0,0,1,1,0,0,1,1,0,0,0,0]
print(a)
```

    [0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 0, 0]



```python
for i in range(0,len(a)):
    if a[i]==1:
        a.pop(i)
        a.append(1)
print(a)
```

    [0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1]

