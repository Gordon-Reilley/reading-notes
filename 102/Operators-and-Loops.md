# Operators and Loops

## Assignment Operator 

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x. If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression. If an expression does not evaluate to an object, then assignments to properties of that expression do not assign.

## Comparison Operators

A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison.

## Loops

Loops offer a quick and easy way to do something repeatedly. You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.

### For Statement

A **for** loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.When a *for* loop executes, the following occurs:

1. The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
3. The statement executes. To execute multiple statements, use a block statement ({ }) to group those statements.
4. If present, the update expression incrementExpression is executed.
5. Control returns to Step 2.

### While Statement

A **while** statement executes its statements as long as a specified condition evaluates to true. If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop. The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while. To execute multiple statements, use a block statement ({ }) to group those statements.

[Back To Home](../README.md)