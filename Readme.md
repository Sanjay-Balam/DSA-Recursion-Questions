# 1. A Video Game Level Design Puzzle (Sudoku Solver)

### Problem Statement
Imagine you're a game developer working on a puzzle-solving video game. One of the game's levels involves solving a number-based puzzle, inspired by Sudoku. The puzzle is a **9x9 grid**, where some numbers are missing, and the player needs to complete the grid by filling in the missing numbers. 

As the developer, your job is to create an algorithm to ensure that each puzzle has a **unique solution**, and the player must fill the grid following specific rules.

In your puzzle-based game, you have a **9x9 grid** that represents an incomplete Sudoku-like challenge for the player. Your task is to write a program that automatically solves this grid, so when the player completes the level, it meets all the following game rules:

1. Each number from **1 to 9** must appear exactly once in every row of the grid.
2. Each number from **1 to 9** must appear exactly once in every column of the grid.
3. Each number from **1 to 9** must appear exactly once in every 3x3 sub-grid (imagine a 9x9 grid is divided into 9 smaller 3x3 grids).
4. Any **empty spot (marked as 0)** in the grid represents a missing number that the player must fill in.
5. The numbers that are already in the grid cannot be replaced by the player.

In essence, you need to ensure that the grid can be completed with the proper numbers, and each level has a **unique solution**.

### Input:
- A **9x9 matrix (grid[][])** where some cells contain numbers between 1 and 9, and other cells contain `0` (representing an empty space that needs to be filled).

### Output:
- A solved version of the Sudoku grid, where all empty spaces (`0`s) are replaced with numbers between 1-9, following the game's rules.

### Example:

#### Input:
```plaintext
grid[][] = {
    {5, 3, 0, 0, 7, 0, 0, 0, 0},
    {6, 0, 0, 1, 9, 5, 0, 0, 0},
    {0, 9, 8, 0, 0, 0, 0, 6, 0},
    {8, 0, 0, 0, 6, 0, 0, 0, 3},
    {4, 0, 0, 8, 0, 3, 0, 0, 1},
    {7, 0, 0, 0, 2, 0, 0, 0, 6},
    {0, 6, 0, 0, 0, 0, 2, 8, 0},
    {0, 0, 0, 4, 1, 9, 0, 0, 5},
    {0, 0, 0, 0, 8, 0, 0, 7, 9}
}
```


#### Output:
```plaintext
grid[][] = {

    {5, 3, 4, 6, 7, 8, 9, 1, 2},
    {6, 7, 2, 1, 9, 5, 3, 4, 8},
    {1, 9, 8, 3, 4, 2, 5, 6, 7},
    {8, 5, 9, 7, 6, 1, 4, 2, 3},
    {4, 2, 6, 8, 5, 3, 7, 9, 1},
    {7, 1, 3, 9, 2, 4, 8, 5, 6},
    {9, 6, 1, 5, 3, 7, 2, 8, 4},
    {2, 8, 7, 4, 1, 9, 6, 3, 5},
    {3, 4, 5, 2, 8, 6, 1, 7, 9}
}
```


# Chess Puzzle Challenge (N-Queens Puzzle Solver)

### Introduction
Imagine you're designing an AI for a chess strategy game where the player is tasked with solving a classic chess puzzle. The challenge is to place **n queens** on an **n x n** chessboard such that no two queens threaten each other. This means queens cannot be placed in the same row, column, or diagonal.

Your task as the developer is to generate **all valid board configurations** for a given chessboard size, ensuring that no two queens can attack each other. Each solution will represent the row position of each queen in a distinct configuration of the chessboard.

### Problem Statement
The **n-queens puzzle** involves placing `n` queens on an **n x n** chessboard so that no two queens can attack each other. Given an integer `n`, the task is to find **all distinct solutions** to this puzzle.

Each solution should represent a valid configuration of queens. The solution is a permutation of `[1, 2, 3, ..., n]` in **increasing order**, where each number in the permutation represents the row position of the queen in the corresponding column.

### Rules of the Puzzle
1. **No two queens can attack each other**:
   - No two queens can be placed in the same row.
   - No two queens can be placed in the same column.
   - No two queens can be placed on the same diagonal.

### Input
- An integer `n` representing the size of the chessboard (i.e., the board will have **n rows** and **n columns**).

### Output
- A list of all **distinct board configurations** where queens are placed according to the puzzle's rules.
- Each configuration is represented by a permutation of numbers, where each number denotes the row position of the queen in the corresponding column.

### Example

#### Input:
```plaintext
n = 4
```
Output:
```js
[
    [2, 4, 1, 3],
    [3, 1, 4, 2]
]
```

### Explanation


Here is how the content can be written in a README.md format:

markdown
Copy code
# N-Queens Puzzle Solver - Real-World Scenario: Chess Puzzle Challenge

### Introduction
Imagine you're designing an AI for a chess strategy game where the player is tasked with solving a classic chess puzzle. The challenge is to place **n queens** on an **n x n** chessboard such that no two queens threaten each other. This means queens cannot be placed in the same row, column, or diagonal.

Your task as the developer is to generate **all valid board configurations** for a given chessboard size, ensuring that no two queens can attack each other. Each solution will represent the row position of each queen in a distinct configuration of the chessboard.

The **n-queens puzzle** involves placing `n` queens on an **n x n** chessboard so that no two queens can attack each other. Given an integer `n`, the task is to find **all distinct solutions** to this puzzle. <br>

Each solution should represent a valid configuration of queens. The solution is a permutation of `[1, 2, 3, ..., n]` in **increasing order**, where each number in the permutation represents the row position of the queen in the corresponding column.

### Rules of the Puzzle
1. **No two queens can attack each other**:
   - No two queens can be placed in the same row.
   - No two queens can be placed in the same column.
   - No two queens can be placed on the same diagonal.

### Input
- An integer `n` representing the size of the chessboard (i.e., the board will have **n rows** and **n columns**).

### Output
- A list of all **distinct board configurations** where queens are placed according to the puzzle's rules.
- Each configuration is represented by a permutation of numbers, where each number denotes the row position of the queen in the corresponding column.

### Example

#### Input:
```js
n = 4
```
Output:

```js
[
    [2, 4, 1, 3],
    [3, 1, 4, 2]
]
```
### Explanation:
For n = 4, there are 2 valid solutions:

The configuration [2, 4, 1, 3] means:
- Queen is placed at row 2 in column 1.
- Queen is placed at row 4 in column 2.
- Queen is placed at row 1 in column 3.
- Queen is placed at row 3 in column 4.

The configuration [3, 1, 4, 2] means:

- Queen is placed at row 3 in column 1.
- Queen is placed at row 1 in column 2.
- Queen is placed at row 4 in column 3.
- Queen is placed at row 2 in column 4.

### Constraints
The value of n will be a positive integer and can vary depending on the difficulty level of the chess puzzle (commonly between 1 and 10 for typical games). <br>

### Objective
Write a function that generates all possible distinct solutions for the n-queens puzzle. Each solution should represent a valid configuration where no two queens can attack each other.

### Chessboard Visualization
For the solution [3, 1, 4, 2] (for n=4), the chessboard would look like this: <br>

```
_ Q _ _
_ _ _ Q
Q _ _ _
_ _ Q _
```

# 3.Robot Pathfinding in a Warehouse (Rat in a Maze)

Imagine you are controlling a small autonomous delivery robot navigating through a large warehouse. The warehouse floor is represented as a grid of cells where each cell is either clear (open for movement) or blocked by an obstacle (like shelves, crates, or walls). The robot starts at the top-left corner of the warehouse `(0, 0)` and needs to deliver a package to the bottom-right corner `(n-1, n-1)`.

The warehouse is represented as a square matrix `mat` of size `n x n`:
- **1** represents an open space where the robot can move freely.
- **0** represents an obstacle or blocked area where the robot cannot pass.

## Problem Statement
Your task is to guide the robot and find **all possible routes** it can take to reach the destination while avoiding obstacles. The robot can move in four directions:
- **U** (Up)
- **D** (Down)
- **L** (Left)
- **R** (Right)

### Rules
1. The robot cannot move to a cell with a `0` (blocked cell).
2. The robot cannot visit any cell more than once in a single path.
3. If the starting point `(0, 0)` is blocked (`0`), the robot cannot move at all, and there is no valid path.
4. If no valid path exists to reach the destination, return an empty list.

## Objective
Write a function that finds all valid routes the robot can take to travel from the starting point `(0, 0)` to the delivery point `(n - 1, n - 1)` and returns a list of all possible paths. Each path should be represented as a string of directions (`U`, `D`, `L`, `R`) indicating the robot’s movement along the route.

### Input
- A square matrix `mat` of size `n x n` where:
  - **1** indicates an open space.
  - **0** indicates an obstacle.

### Output
- A list of all valid paths from the start `(0, 0)` to the destination `(n - 1, n - 1)`.
- If no valid path exists, return an empty list.

### Example

#### Input
```plaintext
mat = [
    [1, 0, 0, 0],
    [1, 1, 0, 1],
    [0, 1, 0, 0],
    [1, 1, 1, 1]
]

Output

```js
    ["DDRR", "DRRD"]
```
### Explanation
- The robot has two valid routes to reach the destination:
  - Route 1: Move Down → Down → Right → Right (path: DDRR).
  - Route 2: Move Down → Right → Right → Down (path: DRRD).

### Edge Cases
- If the starting point `(0, 0)` is blocked (`0`), the robot cannot move, and the function should return an empty list.
- If the destination `(n - 1, n - 1)` is blocked, there is no valid path.
The robot cannot revisit the same cell in a single path.


# 4. Knight's Journey in a Chess Tournament - Minimum Steps to Target

In a chess tournament, a knight is positioned on a chessboard, and it needs to reach a specific target position. Your task is to determine the minimum number of moves the knight will take to reach the target position from its initial position.

The chessboard is a square grid, and the knight can move in an "L" shape, which consists of two squares in one direction and then one square perpendicular to that direction. The knight’s moves can be represented as follows:
- Move two squares forward and one square left.
- Move two squares forward and one square right.
- Move two squares backward and one square left.
- Move two squares backward and one square right.
- Move one square forward and two squares left.
- Move one square forward and two squares right.
- Move one square backward and two squares left.
- Move one square backward and two squares right.


Given:
- The size of the chessboard `n x n`.
- The initial position of the knight `(x1, y1)` and the target position `(x2, y2)`.

Your task is to find the minimum number of steps required for the knight to reach the target position. If it is not possible to reach the target position, return `-1`.

### Input
- Two integers `n` (the size of the chessboard), `x1`, `y1` (initial position of the knight), and `x2`, `y2` (target position of the knight). Note that the coordinates are given in 1-based indexing.

### Output
- An integer representing the minimum number of steps the knight will take to reach the target position. Return `-1` if the target cannot be reached.

### Example

#### Input
```plaintext
n = 8
x1 = 1
y1 = 1
x2 = 8
y2 = 8
```

#### Output
```js
    6
```

### Explanation
The knight can reach the target position in a minimum of 6 moves by following the optimal path.`

### Edge Cases
- If the knight starts at the target position `(x1, y1) == (x2, y2)`, the number of moves required is `0`.
- If the target position is out of the bounds of the chessboard, return `-1`.




# 5. Word Segmentation (Word Break Problem)

Imagine you're working on a text processing application that needs to determine if a given string can be broken down into meaningful words based on a provided dictionary. Your task is to figure out if the string can be segmented into a space-separated sequence of valid words found in the dictionary.


Given:
- A string `s` that may contain words concatenated together.
- A dictionary containing `n` words.

Your goal is to check if the string `s` can be segmented into a sequence of one or more dictionary words. You can use each word from the dictionary any number of times and in any order.

### Input
- A string `s` (1 ≤ |s| ≤ 10^4), which contains only lowercase English letters.
- A dictionary of `n` words, where each word is also a lowercase English letter string.

### Output
- Return `1` if it is possible to break the string `s` into a sequence of dictionary words, otherwise return `0`.

### Example

#### Input
```plaintext
s = "leetcode"
dictionary = ["leet", "code"]
```

#### Output
```js
    1
```

### Explanation
The string "leetcode" can be segmented into "leet" and "code", both of which are valid words in the dictionary. <br>

### Edge Cases
- If the string `s` is empty, return `1` since an empty string can be considered as being segmented.
- If the dictionary is empty and s is not, return 0 since no segmentation is possible.

###Application
- This problem can be applied in various scenarios, such as:

    - Text analysis tools that validate if a given input can form valid sentences.
    - Autocomplete systems that predict user inputs based on a set of predefined words.


# 6. Scrambled String Checker - Are Two Strings Related?

Imagine you are developing a text transformation application that processes strings to check if one can be transformed into another through a series of scrambling operations. Your task is to determine whether one string is a scrambled version of another by analyzing their structure.


Given:
- Two strings `S1` and `S2` of equal length.

- Check if `S2` is a scrambled form of `S1`. A scrambled string is defined based on the following criteria:

- You can represent the string as a binary tree by partitioning it into two non-empty substrings recursively.
- To scramble the string, you can choose any non-leaf node and swap its two children.

For example, given the string `coder`, you can represent it in a binary tree and produce various scrambled forms. For instance:
1. By swapping the children of the node `co`, you can generate the scrambled string `ocder`.
2. Further swapping the children of `der` and `er` can yield `ocred`.

**Note:** A scrambled string is not the same as an anagram, as the order of character partitions matters.

## Input
- Two strings `S1` and `S2` (1 ≤ |S1|, |S2| ≤ 10^4), where |S1| = |S2|.

## Output
- Print `"Yes"` if `S2` is a scrambled form of `S1`, otherwise print `"No"`.

## Example

### Input
```plaintext
S1 = "coder"
S2 = "ocder"
```

#### Output
```js
    "Yes"
```

### Explanation
The string `ocder` can be obtained by scrambling the string `coder`.

### Edge Cases
- If the two strings are identical, they are trivially scrambled versions of each other.
- If the strings have different character frequencies, they cannot be scrambled forms.

### Application
- This problem can be applied in various scenarios, such as:

    - Text encryption and transformation systems that need to validate string relationships.
    - Natural language processing tasks that analyze sentence structures for variations.


# 7. Palindromic Partition Finder (palindromic partitions)

Imagine you are developing a text analysis tool that explores the beauty of symmetry in language. Your task is to find all possible ways to partition a given string into segments where each segment is a palindrome. A palindrome is a sequence of characters that reads the same backward as forward.



- Find and print all possible palindromic partitions of the string `S`. Each partition should consist of substrings that are palindromes.

## Input
- A string `S` (1 ≤ |S| ≤ 20), which contains only lowercase English letters.

## Output
- Print all possible palindromic partitions of the string, with each partition on a new line.

## Example

### Input
```plaintext
S = "geeks"
```

#### Output
```js
    g e e k s
    g ee k s
```

### Explanation
- The output represents all possible ways to partition the string "geeks" into palindromic segments. In this case, "g", "ee", and "k" are palindromes, while single characters are also considered palindromes.



# 8. Reversing a Doubly Linked List - Rewinding Your Journey

Imagine you're planning a road trip using a navigation app that tracks your route in a doubly linked list format. Each location you visit is represented as a node in the list, allowing you to navigate both forward and backward. Your task is to reverse this **doubly linked list**, where each node contains a **value** representing a location (like a city or landmark), a pointer to the **previous node** (the last location visited), and a pointer to the **next node** (the next location to be visited). 

The goal is to reverse the doubly linked list and return the head of the new reversed list. This will enable your navigation app to guide the user back along their previous route seamlessly.

## Input
- The head of the doubly linked list.

## Output
- The head of the reversed doubly linked list.

## Example

### Input
```
Original Doubly Linked List:
Head -> Paris <-> Rome <-> Berlin <-> Tokyo <-> Sydney
```

### Output
```
Reversed Doubly Linked List:
Head -> Sydney <-> Tokyo <-> Berlin <-> Rome <-> Paris
```

## Explanation
- In the original list, the route is from Paris to Sydney. After reversing, the route changes to start from Sydney and ends at Paris, effectively allowing the user to retrace their journey.

## Edge Cases
- An empty list should return `null` (or `None` in Python), indicating there are no locations to reverse.
- A single-node list should return the same node as the head, as there’s nowhere else to go.



# 9. Sorting a Stack - Organizing Your Books

Imagine you have a stack of books piled up in your room, and you want to organize them so that the tallest book is on top. Given a stack represented as a sequence of integers, where each integer signifies the height of a book, your task is to sort this stack so that the top of the stack has the greatest element. 

For instance, if your stack is represented as `3 2 1`, the goal is to ensure that when sorted, the stack looks like `3 2 1`, with the tallest book (3) at the top, followed by the shorter books (2 and 1).

## Input
- A stack represented as a list of integers.

## Output
- A sorted stack with the greatest element at the top.

## Example

### Input
```
Stack: 3 2 1
```

### Output
```
Sorted Stack: 3 2 1
```

# 10. Raising a Number to the Power of Its Reverse

Imagine you are working with a digital display that shows numbers, and you have a special device that can boost the power of any number based on its reverse. For instance, if you enter a number \( N \) into the device, it calculates the reverse of that number \( R \) and then raises \( N \) to the power of \( R \). However, because the resulting number can become extremely large, the device only displays the result modulo \( 10^9 + 7 \).



## Input
- Two integers, \( N \) (the original number) and \( R \) (the reversed number).

## Output
- The result of \( N \) raised to the power of \( R \) modulo \( 10^9 + 7 \).

## Example

### Input
```
N = 2, R = 2
```

### Output
```
4
```

### Input
```js
Input:
N = 12, R = 21
```

### Output
```js
864354781
```
### Explanation
- The reverse of 12 is 21and 1221 when divided by 1000000007 gives remainder as 864354781.
