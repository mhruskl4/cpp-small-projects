# Board Game Simulation (C++)

This project implements a board-based game using C++. The board is represented as a two-dimensional linked structure where each cell contains a stack. The program processes player moves and updates the board state accordingly.

## Overview

The board is constructed from an input file. Each cell has a fixed capacity and stores characters using a stack structure. Players interact with the board by providing directional paths, and the system validates and applies each move based on defined rules.

## Data Structures

### Board Representation

The board is implemented as a 2D linked structure. Each node is connected to its neighboring nodes using four pointers: right, left, up, and down.

### Stack

Each node contains a stack that holds characters. The stack has a fixed size and supports standard operations such as push and pop.

## Game Logic

* The player provides a path using characters such as `r`, `l`, `u`, and `d`
* The system navigates through the board based on this path
* A move may fail if:

  * The path is invalid
  * The target cell is full
  * The cell is not available for placement
* If valid, the player's character is pushed onto the stack in that cell

## Files

* Board.cpp: Implements board creation, movement logic, and display functionality
* Board.h: Contains the Board class and node structure
* CharStack.h: Defines the stack used in each cell

## Compilation

Compile the project using:

g++ Board.cpp -o game

## Execution

Run the program:

./game

## Features

* Two-dimensional linked data structure
* Stack-based storage in each cell
* Input-driven movement system
* Dynamic memory management

## Purpose

This project was developed to practice data structures and object-oriented programming concepts in C++.
