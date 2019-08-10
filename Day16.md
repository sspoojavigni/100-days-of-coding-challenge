## Given the year number. You need to check if this year is a leap year. If it is, print LEAP, otherwise print COMMON.

```

Example input
2012

Example output
LEAP

```

year = int(input())

if year % 4 == 0 and year % 100 != 0:
    print("LEAP")
elif year % 100 == 0:
    if year % 400 ==0:
     print("LEAP")
    else:
     print("COMMON")
else:
  print("COMMON")
  
