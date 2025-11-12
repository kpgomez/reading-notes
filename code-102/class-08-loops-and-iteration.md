# Class 08

## Loops and Iteration

[Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

'Loops offer a qucky and easy way to do something repeatedly'

'A *for* loop repeats until a specified condition evaluates to false'

Example syntax of a for statement

for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement

'When a for loop executes, the following occurs:

The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
The statement executes. To execute multiple statements, use a block statement ({ }) to group those statements.
If present, the update expression incrementExpression is executed.
Control returns to Step 2.'

A while statement executes its statements as long as a specified condition evaluates to true

a while statements looks like below

while (condition)
    statement

if the conditions becomes false, the statement *within* the loop stops executing and the control passes to the statement following the loop

**The condition test occurs before the statement in the the loop executed**


## Expressions and operators

[Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

'Expression is a valid unit of code that resolves to a value'
2 types; ones with *side effects* and ones that *evaluate* only

'All complex expressions are joined by an operator'

The precedence of operators is same as in Math class

A binary operator needs two operands, one before and one after

A unary operator needs one operand, either before or after the operator

++ -- are the only postfix unary operators

### Assignment operators

'An assignment operator assigns a value to its left operand based on the value of its right operand'

### Comparison operators

'A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values'

'The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons'

# Things I want to know

- 
-