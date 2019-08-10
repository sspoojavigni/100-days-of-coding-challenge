## Given a month - an integer from 1 to 12, print the number of days in it in the year 2017.

```
Example input #1
1
(January)

Example output #1
31

Example input #2
2
(February)

Example output #2
28

```


a = int(input())
if a == 2:
	print("28")
elif a == 7 or a == 8:
	print("31")
elif a < 7:
	if a % 2 == 0:
		print("30")
	else:
		print("31")
elif a > 8:
	if a % 2 == 0:
		print("31")
	else:
		print("30")
