## Given a three-digit number. Find the sum of its digits.

```

Example input
123

Example output
6

```

num = int(input())
sum = 0
while num > 0:
    d = num%10
    num = num//10
    sum += d
print(sum)
