## N numbers are given in the input. Read them and print their sum.

The first line of input contains the integer N, which is the number of integers to follow. Each of the next N lines contains one integer. Print the sum of these N integers.

```

Example input
10
1
2
1
1
1
1
3
1
1
1

Example output
13

```

a=[]
n = int(input())
sum=0
for i in range(n):
  num=int(input())
  a.append(num)
for i in range(n):
  sum += a[i]
print(sum)
