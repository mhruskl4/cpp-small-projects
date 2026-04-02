# Number Guessing Game (C++)

This project is a number guessing game implemented in C++.
The program tries to find a secret 2-digit number using feedback logic.

---

## How it works

* The user enters a **game ID**
* The system generates a **secret number**
* The user makes guesses
* The program gives feedback for each digit:

| Symbol | Meaning                         |
| ------ | ------------------------------- |
| F      | Correct digit                   |
| G      | Guess is lower than the secret  |
| L      | Guess is higher than the secret |

---

## Logic

The program uses **linked lists** to keep track of:

* Possible digits
* Impossible digits

Each guess updates these lists until the correct number is found.

---

## Files

* `hw2.cpp` → Main program logic 
* `feedback.cpp` → Feedback calculation 
* `feedback.h` → Function definitions 

---

## How to run

1. Compile the code:

```bash
g++ Source.cpp feedback.cpp -o game
```

2. Run:

```bash
./game
```

---

## Features

* Input validation
* Linked list data structure
* Dynamic memory management
* Step-by-step narrowing of possible digits

---

## Mehir Uşaklı


