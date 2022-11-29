# CS1D Pacman

## TODO - FirstName LastName

Please update with your information.

## Assignment Description

Generate and solve a maze that contains walls and clear paths for PacMan to traverse using the shortest path algorithms covered in class.

## A.) Generate the Maze

Choose the width and height of the maze you'd like to generate. The range is from 10-50 cells wide and 10-50 cells tall. Choose which algorithm you'd like to use to generate a maze.

 - Depth-First Search
 - Kruskal's algorithm, to randomly remove walls so long as they do not cause the maze to become imperfect (introduce two separate paths connecting any two cells
 - Union-Find

Generate a new maze, which will clear out any existing maze and its solution.

## B.) Solve the Maze

Choose what algorithm you'd like to use to solve a maze.

- Depth-First Search
- Dijkstra's Shortest Path
- A*

Control whether or not the process of generating and solving mazes will be animated (depends on the gui).

## Requirements

This project requires you to complete two tasks:

1. Write a maze generator to randomly generate a maze of arbitrary size, with the result required to be a perfect maze. You can optionally write as  many additional maze generators as you'd like.

2. Write a maze solver that uses a recursive, depth first algorithm to traverse and solve a maze of arbitrary size, with the solution extending from the maze's starting cell to it's ending cell without crossing any walls. You can optionally write as many maze solvers as you like.

You can receive a perfect score on this project while implementing only a single maze generator and a single maze solver, writing additional ones will receive extra credit!

Please make sure to follow good CS hygiene--write your code in `src` with proper division of header files, cpp files, input/output test cases, and a `Makefile`. Please make sure you push all code to your repo by the homework deadline.

# Decrypted-X GODOT based Pacman GUI
The following instructions and GUI were developed by former CS1D 2022 graduate [Decrypted-X](https://github.com/Decrypted-X/). Please follow the details below on how to utilize.

## Installing the Application

You can download the binaries for Windows, Linux, or macOS in the bin folder of the project and run the game directly
using the binaries. If your machine is unable to run the application, you can try compiling the code yourself to run the
application in the Godot Engine editor.

## Running the project in Godot

You can follow the more generalized, official tutorial
[here](https://docs.godotengine.org/en/stable/tutorials/scripting/gdnative/gdnative_cpp_example.html) if you need any
extra help.

To run the project directly in the Godot Engine, you must first download the engine from their
[website](https://godotengine.org/download) and then do the following:

* Follow the official Godot documentation to set up compiling for either
[Windows](https://docs.godotengine.org/en/stable/development/compiling/compiling_for_windows.html),
[Linux](https://docs.godotengine.org/en/stable/development/compiling/compiling_for_x11.html), or
[macOS](https://docs.godotengine.org/en/stable/development/compiling/compiling_for_osx.html).

* Clone this repository.

* Then compile the godot-cpp bindings with the following commands. Replace ```<platform>``` with windows, linux, or osx
depending on your OS.

    ```
    cd godot-cpp
    scons platform=<platform> generate_bindings=yes target=release
    cd ..
    ```

* Once the godot-cpp bindings are done compiling, you can compile the project with the following commands:

    ```
    cd cs1d_pacman
    scons platform=<platform> target=release
    cd ..
    ```

After the godot-cpp bindings and the project are compiled, you can then run the project in the Godot Engine. You just
run the Godot Engine and import the project by selecting the ```project.godot``` file in the ```cs1d_pacman/project/```
directory. Click the Run button at the top right of the Godot Engine editor to run the game.
