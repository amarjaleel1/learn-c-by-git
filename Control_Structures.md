# Lesson 3: Control Structures

## Conditional Statements

### How to Use Conditional Statements
Conditional statements allow you to make decisions in your code based on certain conditions. The primary conditional statements in C are `if`, `if-else`, and `switch`.

### Why Use Conditional Statements
Conditional statements are used to execute different code blocks based on different conditions. This helps in controlling the flow of the program and making it more dynamic and responsive.

### Where to Use Conditional Statements
Use conditional statements when you need to perform different actions based on different conditions. For example, checking user input, validating data, or controlling program flow.

### When to Use Conditional Statements
Use conditional statements whenever you need to make decisions in your code. They are essential for implementing logic that depends on dynamic conditions.

### Example Code
```c name=conditional_statements.c
#include <stdio.h>

int main() {
    int num = 10;

    // if statement
    if (num > 0) {
        printf("Number is positive.\n");
    }

    // if-else statement
    if (num % 2 == 0) {
        printf("Number is even.\n");
    } else {
        printf("Number is odd.\n");
    }

    // switch statement
    switch (num) {
        case 10:
            printf("Number is ten.\n");
            break;
        case 20:
            printf("Number is twenty.\n");
            break;
        default:
            printf("Number is neither ten nor twenty.\n");
            break;
    }

    return 0;
}
```

## Loops

### How to Use Loops
Loops allow you to execute a block of code multiple times. The primary loops in C are `for`, `while`, and `do-while`.

### Why Use Loops
Loops are used to perform repetitive tasks efficiently. They reduce code duplication and make programs more concise and manageable.

### Where to Use Loops
Use loops when you need to repeat a block of code multiple times. For example, iterating over arrays, processing lists, or performing tasks until a condition is met.

### When to Use Loops
Use loops whenever you need to perform repetitive tasks or iterate over collections of data. They are essential for tasks that require repetition and iteration.

### Example Code
```c name=loops.c
#include <stdio.h>

int main() {
    // for loop
    for (int i = 0; i < 5; i++) {
        printf("For loop iteration: %d\n", i);
    }

    // while loop
    int j = 0;
    while (j < 5) {
        printf("While loop iteration: %d\n", j);
        j++;
    }

    // do-while loop
    int k = 0;
    do {
        printf("Do-while loop iteration: %d\n", k);
        k++;
    } while (k < 5);

    return 0;
}
```

This lesson provides an overview of control structures in C, including conditional statements and loops. Practice writing and running the provided example codes to reinforce your understanding.

In the next lesson, we will cover functions, including how to define and call functions, function arguments, and return values.