# Lecture Notes

### Pre-lecture commentary

Lexer/Grammar 

Lexer refers to the tokens

fragments are like macros for regex

tokens vs implicit definitions

regex that defines tokens

Bootstrapping

Which came first? 

C compilers could have a super exploit since the first was written in assembly/B and every subsequent compiler is written in C

## Scopes

places where variables are created/belong to

### global scope
- dynamic scoping -> lisp

    def g(x,y) {w=10; f(x,y);}

    is/should w = 10 be available to f?

- when scopes get created
    
    when a new scope starts, embedded in some other scope
    
    define f(x,y) {}

    def g(x,y) {f(x,y)} f scope technicall a part of g scope

    recursive functions

- what scopes are visible at every point


### implementing scopes

scope: a mapping of variable names to values

stack of scopes

traversing the data is necessary

#### naive implementation

iterate the stack finding the variables

#### functions

while im in the function, 
maybe pointer to top of stack and link to the pointer