# Hi! Welcome to the repo!<br>
The polycarbonate language is a language I intend on working on after community college.<br>
You may be asking... Why does this repo exist then? Why not create it after? Well, while I do intend on working on it
after communtiy college, I would still like to establish a historical specification for future me to follow. Polycarbonate is meant to be an esoteric language, and I intend on implementing it the OCaml programming language.

<br>

## Variables
Variables in polycarbonate can only consist of singular letters. For example: `a`, `b` or greek letters such as `α`, or `β`. We will define a sample variable `β` to bind β to the number three. This could be written as:
```apl
β = 0 + ... + 0 + 3 + 0 + ... + 0
```
(Yes, those infinite series of zeroes is required on both the left and the right hand side).
<br>

A builtin function is allowed to check the type of this:<br>
```apl
α = t(β) # t(any) is therefore, a reserved function - and reserved functions cannot be overloaded or redfined. 
```


<br>

## Functions
A function looks simple. it can start with any letter, and may take any amount of arguments (im not THAT evil...)
<br>
<br>
Consider a function a(t), which represents the equation of a standard parabola with no transformations applied on it:
```apl

let a(t) ->
    | r t^2


# Passing arguments is also simple:

α = a(3) # α is binded by the value of 9.
```
