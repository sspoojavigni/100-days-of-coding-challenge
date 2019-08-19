## Given a list of numbers, print all its even elements. Use a for-loop that iterates over the list itself and not over its indices. That is, don't use range()

```

Example input
1 2 2 3 3 3 4

Example output
2 2 4

```

# Read a list of integers:
a = [int(i) for i in input().split()]
for elem in a:
    if elem % 2 == 0:
        print(elem)
