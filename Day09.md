## If you adopted the "Follow the Right Wall" algorithm, you will complete Level 10. 

````

level_10_code = """ while (notDone()) {
if (isPathRight()) {
turnRight();
}
if (isPathForward()) {
moveForward();
} else {
turnLeft();
}
} """
remaining_blocks = 4
print("JavaScript code for Level 10")
print(level_10_code)
print("Number of blocks remaining", remaining_blocks)

````
