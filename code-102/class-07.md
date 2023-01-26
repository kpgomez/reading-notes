# Class 07

## Control Flow

[Source](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)

- The control flow is the order in which statements are executed

Types of Control Structures
- Conditionals
- Loops include for, while, do....while, continue, break, for...in, for...of
- Functions 

Example of a Conditional Statement

if (isEmpty(field)) {
  promptUser(); <-- Function call
} else {
  submitForm(); <-- Function call
}

## Functions

[Source](https://www.w3schools.com/js/js_functions.asp)

In order to use a f(x), it must be defined first

- Function *parameters* are listed inside the () in the function definition

- Function *arguments* are the values received by the function when it is invoked

parameters/arguments behave as *local* variables when inside the function aka {}

// code here can NOT use carName

function myFunction() { let carName = "Volvo"; // code here CAN use carName} <-- function call is within the {}

// code here can NOT use carName

>Since local variables are only recognized inside their >functions, variables with the same name can be used in >different functions.

>Local variables are created when a function starts, and >deleted when the function is completed.

Functions can be used just like variables in

- Formulas
- Assignments
- Calculations

The () invokes the f(x)
No () will return the f(x) object instead of the f(x) result

## Operators

[Source](https://www.w3schools.com/js/js_operators.asp)

- Assignment operators include =, +=, -=, *=, /=, %=, **=
- Arithmetic operators include + addition, * multiplication,- subtraction, ** exponents, / division, & modulus, ++ increment, -- decrement

x += y is the same as x = x + y
x ** y is the same as x = x ** y

+ operator is also used for concatentation of strings (+= can be used here too!)

adding number and string will return a string

- Comparison operators include == equal to, === equal value and equal type, != not equal to, !== not equal value or not equal type, >, <, >=, <=, ? ternary operator

- Logical operators include && logical and, || logical or, ! logical not
- Conditional operators
- Type operators include typeof which returns the type and instanceof which returns true if obj is instance of obj type (classes?)

# Things I want to know

- document.getElementById("demo").innerHTML = toCelsius(77); <-- Need to learn more about the structure of this statement
- I don't understand Bitwise operators at all!
- where are the conditional operators?
