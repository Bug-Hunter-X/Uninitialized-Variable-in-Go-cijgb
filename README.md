# Uninitialized Variable Bug in Go

This repository demonstrates a common error in Go: using an uninitialized variable.  Uninitialized numerical variables will have a default value of zero, but this might not be obvious and can lead to subtle bugs if you're not careful. 

## The Problem

The `bug.go` file shows a simple program that prints the value of an uninitialized integer variable `i`. The output is unexpected because the variable is not initialized before it is printed, resulting in the default zero value being displayed before the assignment of 10. 

## The Solution

`bugSolution.go` demonstrates the correct approach.  The variable `i` is explicitly initialized to a value (0 in this case), making the program's behavior predictable and preventing potential errors.