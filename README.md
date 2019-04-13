# Arithmetic Expressions

## Learning Goals

* Trace Resolution of Variables to Scalar Values to Return Value
* Recognize `+` as the symbol for addition
* Demonstrate the addition operator
* Recognize `-` as the symbol for subtraction
* Demonstrate the subtraction operator
* Recognize `*` as the symbol for multiplication
* Demonstrate the multiplication operator
* Recognize `/` as the symbol for division
* Demonstrate the division operator
* Identify how division in Python differs from normal division

## Introduction

When we first introduced _expressions_, we presented a series of _operators_
and their corresponding _operations_ that were familiar from basic arithmetic:

|Operator|Operation|Note|
|--------|---------|----|
| `+` | Addition ||
| `-` | Subtraction ||
| `*` | Multiplication | We use `*` instead of `×` because it looks like `x`-the-letter|
| `/` | Division | We use `/` instead of `÷` because that's not on a keyboard|
| `**` | Exponentiation | We use `**` instead of `^` because that means something else in programming languages|
| `()` | Association | Expressions inside of `()` get evaluated earlier|

When we learned about these _operators_ and their part in _expressions_, we
didn't know how to use the _variable assignment_ and _variable lookup_
_expressions_ yet. We knew how _operators_ worked with _constant expressions_:
`5 + 1`. How do these expressions work with variables?

## Trace Resolution of Variables to Scalar Values to Return Value

In this section we're going to trace this expression of "variables" until we
get a return value. Consider:

```Python
x = 5
y = 1
x + y #=> ???
```

Our mission is to calculate the value of adding `x` and `y`.

We know how to handle the first two lines: these are simple uses of the
_assignment expression_ which assigns two _scalar values_, `Integer` values to
the variables `x` and `y`:

```Python
x = 5
y = 1
```

Let's consider what happens in the last expression, step-by-step


```Python
x + y #=> ???
```

|Expression|Action|
|----------|------|
| `x + y`  | Variable lookup: `x`, resolves to `5`|
| `5 + y`  | Variable lookup: `y`, resolves to `1`|
| `5 + 1`  | Two constant, scalar, `Integer`s; apply `+` operation|
| `6`      | Addition produces `6`, no operators to apply, constant expression|

Similar logic follows for all of the basic arithmetic operators. While our
examples will use simple expressions with _operators_ and _values_ you should
try setting the numbers to _variables_ and enjoy experimenting in your
conversation with Python.

## Recognize `+` as the Symbol for Addition

Addition's symbol should look familiar. The symbol that is used to perform this
operation is (`+`).

## Demonstrate the Addition Operator

To get a feel for performing addition operations in Python, let's experiment. Open
up the Python interpreter by opening your terminal; type `the Python interpreter` and hit enter and type the commands
below:

```Python
10 + 1 #=> 11
```

```Python
5 + -1 #=> 4
```

## Recognize `-` as the Symbol for Subtraction

Like addition, the symbol for subtraction (`-`) is also the same as in common
arithmetic.

## Demonstrate the Subtraction Operator

Let's experiment again. Open the Python interpreter and type these commands below:

```Python
4 - 13 #=> -9
```

And don't forget that losing negative things is a positive!

```Python
11 - -11 #=> 22
```

## Recognize `*` as the Symbol For Multiplication

The symbol for the multiplication is (`*`) so that we don't confuse it with the
letter `x`.

## Demonstrate the Multiplication Operator

Use the Python interpreter and try typing the following the multiplication commands:

```Python
10 * 10 #=> 100
```

```Python
11 * -11 #=> -121
```

If everything was typed correctly, your results should be `100` and `-121`.
Nothing out of the ordinary, right?


## Recognize `/` as the Symbol For Division

The symbol for the division (`/`) is a forward slash. There's no handy `÷`
character on most keyboards, so programmers adopted `/`.

## Demonstrate the Division Operator

Open up the Python interpreter and try typing the following the division commands:

```Python
20 / 2 #=> 10.0
```
```Python
8 / 3 #=> 2.6666666666666665
```

```Python
4.0 / 13  #=> 0.3076923076923077
```

Notice that we're using `Integer`s for division here, but we will **always**
get back a `Float`.

## Conclusion

Wow that was amazing! We took three lessons to learn three expressions, but in
this lesson we added 4 more! We can now use the Python interpreter as a
calculator &mdash; many programmers keep the Python interpreter open when doing
some mathematics...or when splitting the bill for a lunch order.

Amazingly, our ability to "converse" with Python is on or about 2nd grade in the
US education system (7 years of age). We went from conversational "babies" to
basic school-children in 2 lessons! We're about to take another multi-year leap
by learning to be formal about logic: something that most humans don't get
skilled at until around 5th grade according to most psychologists (or 25 years
of age, according to most parents).
