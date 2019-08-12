## - Write a program that receives a number on the input and prints values from 1 to   
that number subjected to the conditions below. 
- It also should receive another value 'rev' (0 or 1) on the input. 

For every number in the given range, 
  - If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
  - If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
  - If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".

  - If the number is a multiple of both 3 and 5, it prints "JugsMugs".
        - also if number contains 3 and 5, it prints "JugsMugs"
  - If the number is a multiple of both 3 and 7, it prints "JugsPugs".
        - also if number contains 3 and 7, it prints "JugsPugs"
  - If the number is a multiple of 3, 5 and 7, it prints "JugsMugsPugs".
        - also if number contains 3, 5 and 7, it prints "JugsMugsPugs"

Otherwise, it prints the number.

REVERSE REQUIREMENT:
If the boolean 'rev' is True (or 1), then reverse the order of printing. 
   - "PugsJugsMugs" for multiples of 3, 5 and 7
   - "PugsMugs" for multiple of 3 and 7
   - "MugsJugs" for multiple of 3 and 5 
   - "PugsJugs" for multiple of 5 and 7

```
 
INPUT 
5
0
OUTPUT
1
2
Jugs
4
Mugs

INPUT 
15
1
OUTPUT
1
2
Jugs
4
Mugs
Jugs
Pugs
8
Jugs
Mugs
11
Jugs
Jugs
Pugs
MugsJugs

```

a=str(input())
rev=int(input())
s=""
i=1

while (i<=int(a)):
  if("3"in str(i) or int(i)%3==0):
    s1=s+"Jugs"
  else:
    s1=s
  if("5" in str(i) or int(i)%5==0):
    s2=s1+"Mugs"
    if rev==1:
      s2="Mugs"+s1
  else:
    s2=s1
  if("7"in str(i) or int(i)%7==0):  
    s3=s2+"Pugs"
    if rev==1:
      s3="Pugs"+s2
  else:
    s3=s2
  if ("3" not in str(i) and int (i)%3!=0) and ("5" not in str(i) and int(i)%5!=0) and ("7" not in str(i) and int (i)%7!=0):
    s3=i
  i=i+1  
  print (s3)



