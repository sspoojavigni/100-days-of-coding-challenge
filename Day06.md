## Given the integer N - the number of seconds that is passed since midnight - how many full hours and full minutes are passed since midnight.

```
Example input
3900

Example output
1 65

```


 a = int(input())
 print(a)
number_seconds = int(input())
hour = (number_seconds//60)
seconds = (hour//60)
print(seconds,hour)
