## If you adopted the "Follow the Left Wall" algorithm, you will complete Level 10. 

````

level_10_code = """ while (notDone()) {
if (isPathLeft()) {
turnLeft();
}
if (isPathForward()) {
moveForward();
} else {
turnRight();
}
} """
remaining_blocks = 4 
print("JavaScript code for Level 10")
print(level_10_code)
print("Number of blocks remaining", remaining_blocks)


````
