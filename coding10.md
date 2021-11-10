```python
#longest increasing subsequence

lst = [2, 1,3,4,5,4,7,8,11,1]

d = [0] *len(lst)
res = 1
for i in range (len(lst)):
    for j in range (i):
        if lst[j] <= lst[i] and d[i] < d[j] +1:
            d[i] = d[j]+1
        if d[j] > res:
            res = d[j]
print(res)
```

    6



```python
#longest common substring

s1 = [1,3,5,7,9,11]
s2 = [3,5,7,9,2,4,6]

d = [ [0]*(len(s2)+1) for i in range (len(s1)+1) ]

for i in range(1, len(s1)+1):
    for j in range(1, len(s2)+1):
        if s1[i-1] == s2[j-1]:
            d[i][j] = d[i-1][j-1] + 1
        else:
            d[i][j] = max(d[i-1][j], d[i][j-1])
            
print("max LCS numer:", d[-1][-1]) 
```

    max LCS numer: 4



```python

```
