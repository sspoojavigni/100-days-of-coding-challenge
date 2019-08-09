## After you complete the 10th level, what is the JavaScript code you got? 

```

level_10_code = """ while (notDone()) {
  moveForward();
  if (isPathLeft()) {
    if (isPathForward()) {
      if (isPathRight()) {
        turnRight();
      } else {
        turnLeft();
      }
    } else {
      turnLeft();
    }
  } else {
    if (isPathRight()) {
      turnRight();
    }
  }
} """
remaining_blocks = 0 
print("JavaScript code for Level 10")
print(level_10_code)
print("Number of blocks remaining", remaining_blocks)

```
