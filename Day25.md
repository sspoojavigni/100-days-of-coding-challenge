## In mathematics, the factorial of an integer n, denoted by n! is the following product:

n! = 1 × 2 × … × n

For the given integer n calculate the value 

1! + 2! + 3! + ... + n!

```

Example input
4

Example output
33

```

num = int(input())

def factorial(num):
  fact = 1
  res = 0
  for i in range(1,num+1):
    fact = fact * i
    res = res + fact
  print(res)
    
if(num == 1):
  print(1)
else:
  factorial(num)
