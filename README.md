## Symbolic Differentiation in Racket

### Overview: 

An implementation of a Symbolic Differentiator in Racket which supports the following:

- Differentiating mathematical expressions.
- Simplifying expressions.
- Different mathematical operations.
- Output representation.
- Transforming output into different notations (infix, prefix).
- Error handling.

### Usage:

The code can be used in one of two ways:

- It can either be simply copy-pasted into DrRacket to be run as a standalone program, for which the unit tests should be somewhat sufficient to display the general functionality and some edge cases for each function in the progoram.

- Or it can be copy-pasted into DrRacket and extended by further testing for any function in the program. However, please note that not all funcitons were implemented to be used by a user, in which case the user might be faced with unexpected behaviour. The user can always refer the unit tests following a function to learn about how it can be used if they wish to use such functions for different purposes. The functions that were meant to be used by the user are the ones that I consider to be the "main" functions which display the general purpose of the program, namely: `derivative-final`, `simplify-final`, `gradient`, `to-infix` and `variables-of`. These functions will raise errors if called with improper input syntax. The validity of the input syntax can be checked with the function `verify-expression-integrity` prior to using any of the above functions, or any other function which accepts input of the same form to avoid errors.

### Code Overview: 

The first thing one might notice about the program is the sheer size of it, which may seem daunting at first but rest assured, it's not 800+ lines of pure logic. The code was simply a linear solution to the problem statement, that is, for each part of the assignment you will find the corresponding function implemented (with 2 exceptions to be mentioned later) along with helper functions to make the code more readable/maintainable. Any updates to previous functions (e.g. derivative, simplify) were implemented as new functions while keeping the original functions in the code, which contributed heavily to the size of the program. 

The program also has what could be called Unit Tests. Unless a function is overly simple, it is likely to be followed by some tests to present its usage and correctness. All the tests and results are printed to standard output.

### Author Contact Info:
    Name: Jaffar Totanji
    Email: jaafarti@gmail.com
    Telegram: @KuroHata7


##### P.S: This work was done as a solution to an assignment given to me as part of the Programming Paradigms course at IU.
