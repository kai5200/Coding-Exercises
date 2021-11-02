```python
"""
Yang Hui’s Triangl

At the top of the triangle is a 1, which makes up the 0th row.  
The 1st row (1,1) contains two 1s each formed by adding the two numbers above them, 
one to the left and one to the right, in this case 0 and 1.  
(All numbers outside the triangle are 0s.)  
Do the same to create the 2nd row; 0+1=1,  1+1=2,  1+0=1 and all subsequent rows.


"""
```


```python
triangle = []
n=9

for i in range(n):
    row = [1]
    for k in range(i):
        row.append(1) if k == i-1 else row.append(0)
    triangle.append(row)
    if i == 0:
        continue
    for j in range(1,i//2 + 1):
        val = triangle[i-1][j-1] + triangle[i-1][j]
        row[j] = val
        if j != i-j:
            row[-j-1]=val
print(*triangle,sep="\n")
```

    [1]
    [1, 1]
    [1, 2, 1]
    [1, 3, 3, 1]
    [1, 4, 6, 4, 1]
    [1, 5, 10, 10, 5, 1]
    [1, 6, 15, 20, 15, 6, 1]
    [1, 7, 21, 35, 35, 21, 7, 1]
    [1, 8, 28, 56, 70, 56, 28, 8, 1]



```python

```


```python
l
```
