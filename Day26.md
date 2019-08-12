## For the given integer N calculate the following sum:

1³ + 2³ + ... + N³

```
Example input
3

Example output
36
```

num = int(input())
cube =0
for i in range(1,num+1):
  cube += i**3 
print(cube)
