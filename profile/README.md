# Hi! Welcome to the repo!<br>
The polycarbonate language is a language I intend on working on after community college.<br>
You may be asking... Why does this repo exist then? Why not create it after? Well, while I do intend on working on it
after communtiy college, I would still like to establish a historical specification for future me to follow. Polycarbonate is meant to be an esoteric language, and I intend on implementing it the OCaml programming language.

<br>

## Variables
Variables in polycarbonate can only consist of singular letters. For example: `a`, `b` or greek letters such as `α`, or `β`. We will define a sample variable `β` to bind β to the number three. This could be written as:
```hs
β = 0 + ... + 0 + 3 + 0 + ... + 0
```
(Yes, those infinite series of zeroes is required on both the left and the right hand side).

In this example, `3` is defined as:
```apl
3 = 0 + ... + 0 + 1 + 2 + 0 + ... + 0
```

with `1` being defined as:
```apl
0 + ... + 0 + 1 + 0 + 0 + ... + 0
```
and `2` being defined as:
```apl
0 + ... + 0 + 1 + 1 + 0 + ... + 0
```

We then define both those 1's to be defined using our definition of `1` above.
This definition is required to be written in order for the reader to understand the concept of self-ref variables.

<br>

A builtin function is allowed to check the type of this:<br>
```hs
α = t(β) # t(any) is therefore, a reserved function - and reserved functions cannot be overloaded or redfined. 
```


<br>

## Functions
A function looks simple. it can start with any letter, and may take any amount of arguments (im not THAT evil...)
<br>
<br>
Consider a function a(t), which represents the equation of a standard parabola with no transformations applied on it:
```hs

let a(t) ->
    | r t^2


# Passing arguments is also simple:

α = a(3) # α is binded by the value of 9.
```
<br>

<br><br>
## "Self ref" variables can be understood by this example:
we define b to be a variable bounded by 1.
```apl
b = 1
```

Now, to increment, a poor soul would do the following due to the lack of increment operators:
```apl
b = b + 1
```

This isn't doing what you expect it to do. What you instead wrote was:
```apl
b = 1
b = b + 1

b = (b + 1) + 1
b = (b + 1) + 1
b = (b + 1) + 1
b = (((b + 1) + 1) + 1) + 1

b = (((b + 1) + 1) + 1) + 1
b = (((((b + 1) + 1) + 1) + 1) + 1)
b = ((((((b + 1) + 1) + 1) + 1) + 1) + 1)
b = (((((((b + 1) + 1) + 1) + 1) + 1) + 1) + 1)
b = ((((((((b + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1)
b = (((((((((b + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1)
b = ((((((((((b + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1)
b = (((((((((((b + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1)
b = ((((((((((((b + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1) + 1)
```

How we approach "incrementing" a variable is unknown for now. Sorry!
<br>

## As always, this isn't final
Just like nature, things change. With the speed in which these changes will (or will not) occur being unknown. With nature, we define the beauty of languages as a half and half, with one half of a language being successful and the other half being a total failure. Both are okay! Hopefully, once I transfer from community college - I'd have met some other individuals who share
a similar passion to this language, like I do. Do not expect the syntax to remain the same!
