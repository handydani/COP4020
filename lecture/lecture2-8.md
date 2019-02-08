# Lecture Notes

## Ocaml

### Structure matching
```
type = 
Leaf of int
Node of tree1 x tree2
sumleaf (t){
    match t 
    Leaf val => return val
    Node t1,t2 => sumleaft1 + sumleaft2
}
```

### Macros

```
#define if void

```
gcc runs the macro expansion cpp 

macros are kinda like functions but they modify text

they replace structures with something else

```
#ifdef name_of_macro
```

#### templates

vector of ints or doubles or objects

ocaml has this too

c++ is meta programming, code generation

template language is actually turing complete

boost library?

towers of hanoi can be implemented in templates

*quizable*: macros get expanded when the program gets compiled

code in data

treat code as data 

macros treat actions as data
through list of lists structures

set 'name "alin"'

macro expansion in lisp

def macro