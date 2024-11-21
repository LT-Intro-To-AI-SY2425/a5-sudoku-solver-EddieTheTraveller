# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
    When comparing them, it's clear that each one has its own strengths and weaknesses. DFS operates by exploring as far down a branch as possible before backtracking. This could be efficient when it finds a promising path, and DFS tends to use less memory since its only storing nodes along the current path. However, it can get lost in deep paths which would suck. Its useful when you're working with limited memory and a good early exit. BFS explores all depths. It can find things in he fewer nodes but it costs lots of memory. You should use it wen the search space has many deep paths that have dead ends.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
    it impacted it because they explore data strucutres in multiple ways that can be beneficial depending on the amount of data information. Maybe we could've used Minimumm Remaining Value which could help pritioze cells that ave the fewest possible values and speed up the process.



3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
        It might be adapted into making effcicent data structures that can handle larger grids. We could use the Sudoku Solver with bigger datasets and get it to handle more. The lessons could be used in real world scenarios like in Pattern Recognition as this idea present within the solver can be further expanded to identify better strategies and configurations in games or in large data sets in relation to health and science. 
        