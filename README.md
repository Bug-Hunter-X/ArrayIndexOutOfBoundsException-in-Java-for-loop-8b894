# ArrayIndexOutOfBoundsException in Java

This repository demonstrates a common error in Java programming: the `ArrayIndexOutOfBoundsException`. The error occurs when you attempt to access an array element using an index that is out of bounds. This typically happens when the index is negative or greater than or equal to the array's length.

The `Bug.java` file contains code that produces this exception. The `BugSolution.java` file provides a corrected version.

## How to reproduce the bug

1. Clone this repository
2. Compile `Bug.java` using a Java compiler (e.g., `javac Bug.java`)
3. Run the compiled code (e.g., `java Bug`)

You will observe an `ArrayIndexOutOfBoundsException`.

## Understanding the bug

In the original code, the for loop iterates from 0 to `arr.length`.  However, valid array indices range from 0 to `arr.length -1`.  Attempting to access `arr[arr.length]` results in the exception.

## Solution

The corrected code in `BugSolution.java` fixes this by using the condition `i < arr.length` in the for loop, ensuring that the loop iterates only within the valid index range.