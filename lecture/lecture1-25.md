# Lecture Notes

## Ocaml

* ML programming language
* supports functional programming and more
* static type system w *type inference*
* everything is an expression
* interpreter and a compiler
* parenthesis around things is optional
* 2 semicolons to show end of code ;;
* unit is the equivalent of a void
* ocaml is strongly types, it will infer the type
* "let" versus "let in"
* functions treated as first class citizens
* currying
* partial function that remembers the first paramater and is ready to get the second, nth
* instead of statements we program with expressions
* same ideas are in different functional languages
* you have to write rec to denote a recursive function
* easy to get stack overflow so there are optimizations
* tail recursive versions of a function can convert the tail call to a loop which avoids stack overflow
* functions which manipulate other functions to operate
* functions that can return function
* closures capture some of the environment and references the environment in which it was defined
* ocaml has theoretical foundation for types
* algebraic data types are composite types
* shape could be a circle of int, square of int, or rectangle of (int * int)
* pattern matching 

## Ocaml code

```ocaml
print_string "Hello\n";;

# let x = 10;;
val x : int = 10

# x=0;;
- : bool = false

# let y = 3 in y * y;;
- : int = 9

# let add x y = x + y;;
val add : int -> int -> int = <fun>

# add 1;;

# let f = add 2;;
# f 3;;
5
# f 20;;
22

# if (x>5) then 3 else "3";;
Error

# let z = if (x>1) then 2 else 3;;
val z : int = 2

# let double x = 2*x;;

# double 3;;
int = 6

# let triple x = 3*x;;

# let apply f x = f x;;

// f must be a fxn 
// 'a 'b are parameterized types

# apply double 3;;
int = 6

# apply double;;
int -> int = <fun>

# double triple 3;;
Error

# double (triple 3);;

# double triple;;
Error

# let ff = (fun x -> x*x);;
ff : int -> int = <fun>

# let add2 = (fun x y -> x+y);;
// add2 and ff are lambda notation 

# let p = apply (fun x -> x*x) 3;;
p : int = 9

open Core.Std

# let a = [1;2;3;4]

# let p = List.map (fun x -> 3*x) a
val a : list [3;6;9;12]

# 

```