# Go: Unexpected Panic from Nil Map Access

This repository demonstrates a common error in Go programs: panics caused by accessing a nil map.  The `bug.go` file shows the problematic code, while `bugSolution.go` provides a corrected version.

## Problem

In Go, attempting to access a map variable before it's properly initialized (i.e., assigned a value using `make`) results in a runtime panic.  This can lead to unexpected application crashes.

## Solution

The solution involves checking for `nil` before accessing the map or explicitly initializing the map using `make` before any access attempts.  The `bugSolution.go` file demonstrates this solution.

## How to run the code

1. Clone the repository.
2. Navigate to the repository directory.
3. Run the buggy code: `go run bug.go` (This will panic)
4. Run the fixed code: `go run bugSolution.go` (This will run without a panic)