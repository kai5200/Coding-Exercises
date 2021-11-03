```python
#inout number, count the number and how many time in the numbers
# exaple , inout, 3344, output, 3 count 2, 4 count 2 

```


```python
num = input(">>>")
counter = [0]*10
for x in num: #unique(n) *n
    i = int(x)
    if counter[i] == 0:
        counter[i] = num.count(x)
        print("The count of {} is {}".format(x,counter[i]))
```

    >>>3344
    The count of 3 is 2
    The count of 4 is 2



```python
num = input(">>>")
counter = [0] *10

for i in range(10): #10*n
    counter[i] = num.count(str(i))
    if counter[i]:
        print("The count of {} is {}".format(i,counter[i]))
        
print('~'*20)
```

    >>>4039920889
    The count of 0 is 2
    The count of 2 is 1
    The count of 3 is 1
    The count of 4 is 1
    The count of 8 is 2
    The count of 9 is 3
    ~~~~~~~~~~~~~~~~~~~~



```python

```
