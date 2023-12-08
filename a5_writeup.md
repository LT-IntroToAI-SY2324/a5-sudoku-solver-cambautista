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

 Both DFS and BFS are similar. They each go through each scenarios to figure out what values can be implemented until they find one that works. The only difference between both is that DFS utilizes a stack that takes the last thing in the list out first while BFS uses queues that pop out the first thing in the list. Sometimes BFS can be more efficient.


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

  Like mentioned above, stacks and queues affected the order elements were popped out but did not affect the functionality. Deques could have been used. They can add or remove elements from either the beginning or end. This hybrid version could have combined both the DFS and BFS functions.



3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

 The sudoku solver could be adapted for larger puzzles by allowing the board to be bigger than 9. This can be done by implementing code that allows for the user to input the grid size number which is then put into a variable. We can learn to create systems or methods that can help us solve problems more efficiently instead of spending a long time guessing and checcking.

