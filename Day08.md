## Write a program to calculate the distance between two points.

```
INPUT 
4
0
0
0

OUTPUT
4


INPUT 
0
0
4
3

OUTPUT
5

```


import math
x1 = int(input())  
y1 = int(input())
x2 = int(input())  
y2 = int(input())
distance = math.sqrt((x2 - x1)**2 + (y2 - y1)**2)
print (distance)
