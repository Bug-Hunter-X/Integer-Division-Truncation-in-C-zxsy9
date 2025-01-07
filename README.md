# Integer Division Truncation in C
This example demonstrates a common issue in C programming involving integer division. Integer division truncates the fractional part of the result, which can lead to unexpected results if not handled correctly.

## Bug Description
The code performs integer division between two integers. Due to the nature of integer division, the fractional part is discarded, potentially leading to inaccuracies in calculations.

## Solution
To obtain the more precise result, the variables should be declared as floating-point numbers (float or double). This will allow for the fractional part of the result to be preserved.  Another option is to perform the calculation using floating-point variables and cast them to integer if an integer is desired.

## How to Reproduce
1. Compile the `bug.c` file.
2. Run the compiled program.
3. Observe that the output is 2, not 2.0, due to truncation of the fractional part.  Compile and run `bugSolution.c` to see the correct output. 