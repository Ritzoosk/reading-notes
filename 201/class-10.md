# JS
## JavaScript book, Ch. 10, “Error Handling & Debugging”
- pg 450
- order of execution, functions, arith, etc
- execution context
>GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.

FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.

EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function
called eva l {) (which is not covered in this book). 

- Scope
>GLOBAL SCOPE
If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.

FUNCTION-LEVEL SCOPE
When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope. 
- THE STACK pg 455 pdf 462

## Context Exe
- prepare
 - scope create
 - var, funcs and args created
 - "this" val is determind

- Execute
 - assign vals
 - ref funcs
 - exe statments
- error type tbl pg 459 / 466

## how to find consoles and use them for certain browsers (circa2011)
- pg 464 / 471 to pg 470 / 477
 - chrome
 - IE
 - FF
 - Opra
 - Safari

 ## stepping through code
- pg 477

## throwing errors
- pg 483 / 490

## tips
- 484

## Common errors
- 485
