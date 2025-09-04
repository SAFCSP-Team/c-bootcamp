
# Conditional statements

Conditional statements in programming are similar to making decisions or following routines in daily life, for example, if it’s sunny, you wear sunglasses; otherwise, you carry an umbrella. They help determine which specific statements, instructions, or function calls are executed within a program based on given conditions.

Types of Conditional Statements:
* if Statement
* if-else Statement
* else if statements
* switch Statement
  
### Conditional Statements

* The `if` statement executes a block of code if a condition is true.

```c
#include <stdio.h>

int main()
{
    int number = 5;

    // Check if number is positive
    if (number > 0) 
    {
        printf("The number is positive.\n");
    }

    return 0;
}
```

* The `if-else` statement executes one block of code if a condition is true and another block if it is false.

```c
#include <stdio.h>

int main()
{
    int number = -5;

    // block of code to be executed if the condition is true
    if (number > 0)
    {
        printf("The number is positive.\n");
    } 

    // block of code to be executed if the condition is false
    else
    {
        printf("The number is not positive.\n");
    }

    return 0;
}
```

* The `else if` statement is checking multiple conditions in sequence. If the first condition is false, it checks the next condition, and so on.

```c
#include <stdio.h>

int main()
{
    int number = -9;


    // block of code to be executed if condition1 is true
    if (number > 0)    // condition1
    {
        printf("The number is positive.\n");
    }

   // block of code to be executed if the condition1 is false and condition2 is true
    else if (number < 0) // condition2
    {
        printf("The number is negative.\n");
    }

   // block of code to be executed if the condition1 is false and condition2 is false
    else
    {
        printf("The number is zero.\n");
    }

    return 0;
}

```

* The `switch` statement is used for multiple conditions based on fixed values. then compares the value of an expression with the values in each `case`. If a match is found, the corresponding block of code is executed.
  
```c
#include <stdio.h>

int main()
{
    int day = 3;

    switch (day)
    {
    case 1:
        printf("Monday\n");
        break;
    case 2:
        printf("Tuesday\n");
        break;
    case 3:
        printf("Wednesday\n");
        break;
    default:
        printf("Invalid day\n");
    }

    return 0;
}
```

> Note: the break keyword terminates the execution of the current case block and prevents fall-through to the next case.


### Practice

Write a program that checks if a number is odd or even using an `if-else` statement.

```c
#include<stdio.h>

int main(){
    // add your code here 
    return 0;
}
```
