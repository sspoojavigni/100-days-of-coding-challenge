## Given three integers, print the least of them.

```

Example input
5
3
7

Example output
3

```


a = int(input())
b = int(input())
c = int(input())
# Print a value:
if a > c and b > c:
  print(c)
elif a > b and b < c:
  print(b)
else:
  print(a)
