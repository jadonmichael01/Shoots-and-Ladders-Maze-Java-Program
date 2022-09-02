# Shoots-and-Ladders-Maze-Java-Program
In this project, I implemented a Java program that finds the shortest path that a hare needs to take to go through 
a grid-shape maze. The hare enters the maze from a specific square (start) and leaves the maze at another specific 
square.
Implemented a txt file as a Maze map that contains multiple rows and columns. 
Implemented a recursive operation to solve the maze based on the maze's cells.
The table cell contains unique strings: 
str.equals(“S”): cell is the start square where hare starts the journey. This cell is always at row 0 and column 0 (unless you want to do the extra-credit part of the assignment).
str.equals(“T”): cell is the target square where hare ends the journey. This cell is always at the last row and last column (unless you want to do the extra-credit part of the assignment).
str.equals(“N”): cell has no special property. Hare can move either one square to the right or one square to the bottom of the map (unless you want to do the extra-credit part of the assignment).
str.equals(“DE”): cell is a dead-end which means that if hare enters this cell, there is no way out of it.
str.contains(“W”): cell is a waiting square! If hare enters this cell, it needs to stay and wait in the cell for a specific units of time before leaving it. The length of waiting time is determined by the number that comes after ‘W’ (e.g. “W5” means that hare needs to stay and wait for 5 consequent steps before moving out of the cell).
str.contains(“XR”): cell is a no-right square! If hare enters this cell, it can’t exit by moving to the right square.
!str.contains(“XR”) && str.contains(“R”): cell has a ladder on it! If hare enters this cell, it can either move normally (one step to the neighboring squares) or use the ladder to move multiple squares to the right. The length of ladder comes after the letter ‘R’ (e.g. “R3” means that there is a horizontal ladder of length 3).
str.contains(“XD”): cell is a no-down square! If hare enters this cell, it can’t exit by moving down.
!str.contains(“XD”) && str.contains(“D”): cell has a ladder on it! If hare enters this cell, it can either move normally (one step to the neighboring squares) or use the ladder to move down multiple squares. 
