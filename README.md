# Parking Lot Puzzle

This is a solution for the Parking Lot Puzzle, which is a classic artificial intelligence problem. The goal of this
puzzle is to move the red car to the exit by sliding the other cars up and down or left and right. The puzzle is solved
when the red car reaches the exit.

The solution is implemented in Python and consists of three files: `main.py`, `algorithms.py`, and `parking_state.py`.
The `main.py` file is the entry point of the program, and it reads the input from the user and calls
the `a_star_algorithm()` function defined in the `algorithms.py` file. The `a_star_algorithm()` function uses the A*
search algorithm to find the shortest path from the initial state to the goal state. The `parking_state.py` file defines
the `ParkingState` class, which represents a state of the puzzle.

## How to Run the Program

To run the program, you need to have Python 3 installed on your computer. You can download Python 3 from the official
website (https://www.python.org/downloads/).

1. Download the three Python files (`main.py`, `algorithms.py`, and `parking_state.py`) and save them in a directory.
2. Open a terminal or command prompt and navigate to the directory where the files are saved.
3. Run the command `python main.py` to start the program.
4. Enter the input for the parking lot puzzle as described below.

## Input Format

The input for the parking lot puzzle consists of several test cases, each represented by a set of lines. The first line
of each test case contains an integer `n` (1 ≤ `n` ≤ 100), which represents the number of cars in the puzzle. The second
line contains three integers `x`, `y`, and `car_num`, separated by spaces. `x` and `y` represent the width and height of
the parking lot, respectively (1 ≤ `x`, `y` ≤ 6), and `car_num` represents the number of cars in the puzzle (
2 ≤ `car_num` ≤ 13).

The next `car_num` lines contain the information of each car. Each line contains four values separated by
spaces: `row`, `col`, `pos`, and `length`. `row` and `col` represent the position of the upper-left corner of the car in
the parking lot (1 ≤ `row` ≤ `y`, 1 ≤ `col` ≤ `x`), `pos` represents the orientation of the car (`h` for horizontal
or `v` for vertical), and `length` represents the length of the car (2 ≤ `length` ≤ 3).

Here is an example of the input format for one test case:

```
1
6 6 13
3 1 h 2
1 1 v 2
1 2 v 2
1 4 h 3
2 3 h 2
2 5 h 2
3 4 v 2
4 2 v 2
5 3 h 2
5 5 v 2
5 6 v 2
6 1 h 2
6 3 h 2
```

This input represents a parking lot with a width of 6, a height of 6, and 13 cars. The red car is located at position (
3, 1) and has a length of 2. There are 12 other cars in the parking lot, each with a length of 2 or 3.

## Output Format

For each test case, the program outputs a single line containing the cost of the shortest path from the initial state to
the goal state. The cost represents the number of moves required to move the red car to the exit.

Here is an example of the output format for one test case:

```
Test #1: 16
```

This output means that the shortest path from the initial state to the goal state requires 16 moves.

## Conclusion

The parking lot puzzle is a classic artificial intelligence problem that can be solved using the A* search algorithm.
The solution presented in this readme file consists of three Python files: `main.py`, `algorithms.py`,
and `parking_state.py`. The program reads the input from the user, solves the puzzle using the A* search algorithm, and
outputs the cost of the shortest path from the initial state to the goal state. To run the program, you need to have
Python 3 installed on your computer and follow the input and output format described above.

This solution can be extended in several ways, such as implementing other search algorithms, optimizing the heuristic
function, or adding a graphical user interface to visualize the puzzle.