# Kotlin ConcurrentModificationException Example

This repository demonstrates a common error in Kotlin: the `ConcurrentModificationException` that can arise when modifying a collection (like a `MutableList` or `MutableSet`) while iterating over it using a standard `for` loop.

The `bug.kt` file shows the problematic code. The `bugSolution.kt` file provides a solution using iterators or `removeIf` which avoid this exception.

## How to Reproduce

1. Clone this repository.
2. Open `bug.kt` in a Kotlin IDE.
3. Run the `main` function.
4. Observe the `ConcurrentModificationException` being thrown.

## Solution

The solution involves avoiding direct modification within the loop.  Use an iterator or the safer `removeIf` function.