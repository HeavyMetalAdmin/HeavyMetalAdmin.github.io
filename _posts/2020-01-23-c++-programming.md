---
title: C++ Programming
date: 2020-01-23 10:45:00
categories: [Languages,C++]
tags: [overview]
seo:
  date_modified: 2020-01-24 11:48:25 -0500
---
# C++ Programming

## Structure

- **//** = comment
- '**#**' = directives, instructs compiler to include the code from the referenced library
- **namespace** = group a set of classes, functions, etc. under a name
- **;** = terminator, at the end of the command
- **main** = where the program execution starts, first code executed
- **{}** = contain the body of the function that they are nested under
- **cout** = standard output, prints to console
- **return** = can have different values and functions

## Variables & Types

- Variables are portions of the memory where values are stored
  - Has a unique identifier or name
  - Global variable
    - Declared in the body of the source code
    - Can be referred anywhere
  - Local variable
    - Declared inside the body of functions
    - Can only be referred in THAT function
- Small list of variables
  - ![Table-1](\assets\img\posts_data\c++\Table-1.png)

## Input / Output

- **cout** is the standard output and prints to console
- **<<** tells the compiler to insert the next data into the stream
- **endl** = new line character, flushes the buffer
- **cin**  is the standard input, takes user input into the stream
  - Must be stored in a variable
- **cin.ignore()** is used to clean the buffer and keep the console opened

## Operators

- ### 4 Main Classes of Operators:

  - **Arithmetic**
    - ![Math-1](\assets\img\posts_data\c++\Math-1.png)
    - Increment operator **(++)** = adds 1 to its operand
      - Can precede or follow an operand
        - **(x++)**
          - Operations preformed before obtaining the value of the operand
          - ![Operator-1](\assets\img\posts_data\c++\Operator-1.png)
        - **(++x)**
          - Operations preformed after obtaining the value of the operand
          - ![image-20200117082232834](\assets\img\posts_data\c++\image-20200117082232834.png)
    - Increment operator**(++)** adds 1 to its operand
    - Decrement operator**(--)** subtracts 1 from its operand
  - **Relational**
    - Defines relationship between two values
    - ![Relationship-1](\assets\img\posts_data\c++\Relationship-1.png)
    - Used to evaluate a comparison between two expressions, returns a Boolean value
      - ![Bool-1](\assets\img\posts_data\c++\Bool-1.png)
  - **Logical**
    - Defines previous relationships must be connected
    - ![Relationship-2](\assets\img\posts_data\c++\Relationship-2.png)
    - Any value other than zero is **TRUE**
      - 1 for returned value
    - Zero is **FALSE**
      - 0 for returned value
    - bool data type is used to express TRUE or FALSE statements, automatically converts 0 to FALSE and 1 to TRUE
    - ![Bool-2](\assets\img\posts_data\c++\Bool-2.png)
  - **! =** only has one operand (right) and it inverses this value to determine if it's true or false
  - **&& (AND)** =  evaluates two expressions to obtain the relational results
    - **TRUE** if both operands are **TRUE**
    - **FALSE** if one operand is **FALSE**
  - **|| (OR)** = evaluates two expressions to obtain the relational results
    - **TRUE** if either operand is **TRUE**
    - **FALSE** if *BOTH* are **FALSE**
  - **Bitwise**
    - Operations refer to testing, setting, or shifting the actual bits in the byte or word
    - ![Operations-1](\assets\img\posts_data\c++\Operations-1.png)

- **lvalue** is ANY label that appears on the left of a assignment statement, variable name

- **rvalue** is ANYTHING to the right of a assignment statement, value assigned to the variable

## Iteration & Conditional Structures

**Three main groups of statements:**

**Selection**

- **if**
  - If the expression is evaluated to true the **IF** expression is executed, otherwise the **ELSE** expression is executed
  - One or the other, both codes are never executed
  - Can be nested statements
  - ![Nsted-1](\assets\img\posts_data\c++\Nested-1.png)
- **switch**
  - Evaluates expression in order against a list of values
  - Only the block of code that matches is executed
  - **MUST** be an integer or constant
  - ![Statements-2](\assets\img\posts_data\c++\Statements-2.png)
  - Value of the expression is tested against all case statements, when a match is found that block is executed until the break the statement
  - If no value is matched the default statement is executed, if this is not put it in nothing happens

**Iteration**

- **while**
  - ![While-1](\assets\img\posts_data\c++\While-1.png)
  - statement = can be empty, single, or a block of statements
  - condition = can be any expression, and is true as long is any non-zero value is present
  - loop continues while the condition evaluates to true
  - when loop evaluates to false, the execution goes to the line of code after the loop
- **for**
  - ![for-1](\assets\img\posts_data\c++\For-1.png)
  - initialization = assignment statement that sets the starting value of the loop control variable
  - condition = determines when the loop ends
  - increment = determines how the control variable changes each iteration 
  - ![Loop-1](\assets\img\posts_data\c++\Loop-1.png)
    - Starts with 2, goes until a =50, increases the control by 2
  - Infinite loop created by for(;;), while stop for a break condition
- **do-while**
  - ![do-while](\assets\img\posts_data\c++\d0-while.png)
  - loop checks are checked at the end of the loop
  - executes at least once

**Jump**

- **break**
  - Can be used in loops and switch statements
  - When encountered the execution jumps to the code following the switch statement
  - used in conjunction with loop statements
  - 
- **continue**
  - used in conjunction with loop statements
  - forces code to continue to next iteration of a loop
- **goto**
  - can make program unreadable
  - requires a label
  - label = identifier followed by a colon
    - *label :* 
  - cannot jump between functions
  - must be in the same block of statements as the goto statement
- **return**
  - used to return from function
  - may or may not have value associated
  - function stops executing when it encounters the first return

## Pointers

- variable that holds a memory address, this address is the location of another object in memory
- must be written in a specific format
  - type = base type of the pointer (int, char ...)
    - defines the type of variable the pointer can point to
  - name = name (identified) of the variable
- ![Pointers-1](\assets\img\posts_data\c++\Pointers-1.png)
- Special pointer operators:
  - (*) = returns the value located at the address
  - & = returns the memory address of the variable

## **Arrays**

- Collection of variables of the same type
- Elements are access by an index
- ![Arrays-1](\assets\img\posts_data\c++\Arrays-1.png)
- type = declares the type of array
- size = defines the length of the array
- 0 is the first element in the index

