## Write a program that receives a number on the input.
If the number is a multiple of 3, it prints "Jugs". 
If the number is a multiple of 5, it prints "Mugs".
If the number is a multiple of 7, it prints "Pugs".

If the number is a multiple of both 3 and 5, it prints "JugsMugs".
If the number is a multiple of both 3 and 7, it prints "JugsPugs".
If the number is a multiple of both 5 and 7, it prints "MugsPugs".
If the number is a multiple of both 3, 5 and 7, it prints "JugsMugsPugs".

Otherwise, it prints the number.

```

INPUT 
15

OUTPUT
JugsMugs

INPUT 
21

OUTPUT
JugsPugs


INPUT 
105

OUTPUT 
JugsMugsPugs

```

n = int(input())
if(n % 3 == 0) and (n % 5 == 0) and (n % 7 == 0):
  print("JugsMugsPugs")
elif(n % 3 == 0 ) and (n % 5 == 0):
  print("JugsMugs")
elif(n % 3 == 0)  and (n % 7 == 0):
  print("JugsPugs")
elif(n % 5 == 0) and (n % 7 == 0):
  print("MugsPugs")
elif(n % 3 == 0):
  print("Jugs")
elif(n % 5 == 0):
  print("Mugs")
elif(n % 7 == 0):
  print("Pugs")
else:
  print(n)
