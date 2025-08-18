# Introduction

## Concept
The C programming language is a general-purpose, high-level language that is widely used for system programming, application development, and embedded systems. Developed in the early 1970s, C provides low-level access to memory and is known for its efficiency and performance. It serves as the foundation for many modern programming languages and is essential for understanding computer science principles.

## Example
A simple example of a C program that prints "Hello, World!" to the console:

1. Create a file with ".c" extention, we will create **hello.c** file.
2. Open **hello.c**.
3. Write your code.
```c
#include <stdio.h>

int main() {
    printf("Hello, World!");
    return 0;
}
```
4. Open the terminal.
5. Compile the program, run command: `gcc hello.c -o hello`.
6. Run the program, run command: `./hello`.
7. Output:
 
```
Hello, World!
```

In this example, we include the standard input-output library `#include <stdio.h>`.   
Define the main function `int main(){}`.    
Use printf to display a message `printf("Hello, World!");`.   

## Practice

Write a C program that prints "C Language" to the console.

```c
#include <stdio.h>

int main() {
    // Add your code here
    return 0;
}
```
- Compile.
- Run.
- Output:

```
C Language
```
