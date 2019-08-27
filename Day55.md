## Write a function second_biggest_value which accepts three integers, and does the following:
returns the second biggest value among the three
returns “NA” if there are two or more equal values

Come up with a solution which does not use sorting!


```

Example

(1, 2, 3) -> 2
(3, 1, -1) -> 1
(3, 5, -1) -> 3
(3, -1, -1) -> "NA"

```
def second_biggest_value(x,y,z):
  s= max(x,y,z)
  s1=min(x,y,z)
  if x==y or y==z or x==z:
    return "NA"
  elif((x!=s) and (x!=s1)):
    return x
  elif((y!=s) and (y!=s1)):
    return y
  elif((z!=s) and (z!=s1)):
    return z
  else:
    return "NA"
