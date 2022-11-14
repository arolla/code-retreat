*Coderetreats are free day-long, intensive practice events, focusing on the fundamentals of software development and design. By providing developers the opportunity to take part in focused practice, away from the pressures of "getting things done", the coderetreat format has proven itself to be a highly effective means of learning and nurturing software development skills.* (from https://www.coderetreat.org)

# Structure of a Code-Retreat

- Problem: Conway's Game of Life: https://en.wikipedia.org/wiki/Conway's_Game_of_Life
- Length of each session: 42 minutes
- Prefer using Test-Driven Development (TDD)
- The same exercise is repeated multiple times during the time of the code-retreat
- Short debrief time after each session

**Pair-programming is necessary**

**After each session, change your partner**

**After each session, code must be deleted, not put in a branch, not stashed, just deleted with no trace left**

*The result of each session is the collaborative learnings you experienced with your pairing partner.*

# The Rules of the Conway's Game of Life

The universe of the Game of Life is an infinite, two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, live or dead (or populated and unpopulated, respectively). Every cell interacts with its eight neighbours, which are the cells that are horizontally, vertically, or diagonally adjacent. At each step in time, the following transitions occur:

1. Any live cell with fewer than two live neighbours dies, as if by underpopulation.
1. Any live cell with two or three live neighbours lives on to the next generation.
1. Any live cell with more than three live neighbours dies, as if by overpopulation.
1. Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.


# Potential Constraints for later iterations

- TDD + Ping-Pong (write test / code) 
- TDD As If You Meant It (i.e. Strict TDD)
- Evil partner
- Silent Pairing
- Object Calisthenics
- Immutable
- Choose your Constraint(s)
 - Fluent Style: newX.withYAt(1).withZ()…build();
 - No Mouse, or No IDE (text editor only)
 - No conditional statementsNo loops
 - No TDD
 
 ## TDD As If You Meant It (i.e. Strict TDD) 
 
1. Write exactly one new test. It should be the smallest test which seems to point in the direction of a solution
1. Run the test to make sure it fails
1. Make the test from (1) pass by writing the least amount of implementation code you can IN THE TEST METHOD.
1. Refactor to remove duplication or otherwise as required to improve the design. Be strict about the refactorings. Only introduce new abstractions (methods, classes, etc) when they will help to improve the design of the code. Specifically:
1. ONLY Extract a new method if there is sufficient code duplication in the test methods. When extracting a method, initially extract it to the test class (don't create a new class yet).
1. ONLY create a new class when a clear grouping of methods emerges and when the test class starts to feel crowded or too large.
1. Repeat the process by writing another test (go back to step #1).

## Object Calisthenics

1. Wrap all primitives and strings
1. Use only one dot per line
1. Don’t abbreviate
1. Keep all classes small
1. Don’t use any classes with more than two instance variables
1. Use first-class collections
1. Don’t use any getters/setters/properties

