# Lecture 

## Abstract Syntax Trees
- 1+2*3
- leaves come first, operators after
- RPN
- post order traversal
- use a stack, 123* -> 1 -> 1+ -> 7

## OCAML
- type encoding
- sum type use for error
- lisp is like a linked list
- immutable lists (unchanging)
- stacks as a list

### Mutability and aliasing
- having aliases to mutable 

### nonstrict evaluation
- branching 
- lazy evaluation

### unit testing

# key concepts of functional programming
- pure functions
- immutable data
- good software engineering

```ocaml
let a = [20;10;0]
let b = 30::a // this creates a new list, does not change a

```
