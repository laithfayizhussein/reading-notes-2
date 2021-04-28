# “Complexity is anything that makes software hard to understand or to modify." — John Outerhout
## What is functional programming:
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data .
-  pure functions:
    - It returns the same result if given the same arguments (it is also referred as deterministic).
    - It does not cause any observable side effects.
    - Reading Files: If our function reads external files, it’s not a pure function — the file’s contents can change.
    - Random number generation: Any function that relies on a random number generator cannot be pure.
- every function is isolated and unable to impact other parts of our system.
## Immutability:
- Unchanging over time or unable to be changed.
-  its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
## Referential transparency:
- If a function consistently yields the same result for the same input, it is referentially transparent.
> pure functions + immutable data = referential transparency
## Functions as first-class entities:
- fer to it from constants and variables
- pass it as a parameter to other functions
- return it as result from other functions

