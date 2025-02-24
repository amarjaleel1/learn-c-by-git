# Lesson 1: Introduction to C

## History and Importance of C
C is a general-purpose programming language developed in 1972 by Dennis Ritchie at Bell Labs. It has influenced many other programming languages, such as C++, Java, and Python. C is widely used in system programming, developing operating systems, and embedded systems due to its efficiency and control over hardware.

## Setting Up the Development Environment
To write and run C programs, you need to set up a C development environment on your system. This typically involves installing a C compiler and an Integrated Development Environment (IDE). Some popular compilers and IDEs are:
- GCC (GNU Compiler Collection)
- Clang
- Code::Blocks
- Visual Studio Code

## Writing Your First C Program
Let's write a simple C program that prints "Hello, World!" to the console.

```c name=hello_world.c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

To compile and run this program using GCC, follow these steps:
1. Save the code in a file named `hello_world.c`.
2. Open a terminal and navigate to the directory where the file is saved.
3. Compile the program using the command: `gcc hello_world.c -o hello_world`
4. Run the compiled program using the command: `./hello_world`