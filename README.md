# Type 'string[]' is not assignable to type 'string'
This bug demonstrates a common TypeScript error: providing an array of strings to a function expecting a single string.  The solution involves either modifying the function's signature to accept an array or iterating through the array to apply the function to each element.

## How to Reproduce
1. Clone this repository.
2. Compile and run the code in `bug.ts` using a TypeScript compiler (tsc) and Node.js.
3. Observe the type error.

## Solution
The solution, implemented in `bugSolution.ts`, addresses this by iterating through the array and applying the function individually to each string element.