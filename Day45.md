## It is possible to place 8 queens on an 8×8 chessboard so that no two queens threaten each other. Thus, it requires that no two queens share the same row, column, or diagonal.

```
Example input
1 5
2 3
3 1
4 7
5 2
6 8
7 6
8 4
(shown on the picture)

Example output
NO

```

n = 0
coord = {}
myList = []
x_co = []
y_co = []
Rule_vi = None
while n < 16:
    a = input()
    inList = list(map(int, a.split()))
    myList.append(inList[0])
    myList.append(inList[1])
    x_co.append(myList[n])  # Create ordered list of x values
    y_co.append(myList[n+1]) # Create ordered list of y values
    n = n+2
i = 0
for x in x_co:
    for i in range(0,8):
        if x == x_co[i] and x_co.index(x) != i:
            Rule_vi = True  # Check if peices are horizontally threatened.
i = 0
for y in y_co:
    if Rule_vi == True:
      break
    for i in range(0,8):
        if y == y_co[i] and y_co.index(y) != i:
            Rule_vi = True # Check if pieces are vertically threatened. 
            break
n = 0
i = 0
for n in range(0,8):
    if Rule_vi == True:
        break
    for i in range(0,8):
        if  abs(x_co[n] - x_co[i]) == abs(y_co[n] - y_co[i]) and i != n:
            Rule_vi = True # Check is pieces are diagonally threatened.
            break
if Rule_vi == True:
  print('YES')
else:
  print('NO')


    
