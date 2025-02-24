# Lesson 2: Basic Syntax

## Data Types

C provides several data types, which can be categorized into the following types:
1. **Basic Data Types**: `int`, `char`, `float`, `double`
2. **Derived Data Types**: `array`, `pointer`, `structure`, `union`
3. **Enumeration Data Type**: `enum`
4. **Void Data Type**: `void`

### Basic Data Types
- **int**: Used to store integers.
- **char**: Used to store characters.
- **float**: Used to store single-precision floating-point numbers.
- **double**: Used to store double-precision floating-point numbers.

### Example Code
```c name=data_types.c
#include <stdio.h>

int main() {
    int integer = 10;
    char character = 'A';
    float single_precision = 5.75;
    double double_precision = 10.25;

    printf("Integer: %d\n", integer);
    printf("Character: %c\n", character);
    printf("Float: %.2f\n", single_precision);
    printf("Double: %.2lf\n", double_precision);

    return 0;
}
```

## Variables and Constants

Variables are used to store data that can be changed during program execution. Constants are used to store data that cannot be changed once defined.

### Declaring Variables
```c
int age;
float salary;
char grade;
```

### Declaring Constants
```c
const int MAX_AGE = 100;
const float PI = 3.14159;
```

### Example Code
```c name=variables_constants.c
#include <stdio.h>

int main() {
    int age = 25;
    const float PI = 3.14159;

    printf("Age: %d\n", age);
    printf("PI: %.5f\n", PI);

    age = 30; // Valid
    // PI = 3.14; // Invalid, PI is a constant

    return 0;
}
```

## Operators

C provides various operators for performing operations on variables and constants. These operators can be categorized into the following types:
1. **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
2. **Relational Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`
3. **Logical Operators**: `&&`, `||`, `!`
4. **Assignment Operators**: `=`, `+=`, `-=`, `*=`, `/=`, `%=`
5. **Increment and Decrement Operators**: `++`, `--`
6. **Bitwise Operators**: `&`, `|`, `^`, `~`, `<<`, `>>`

### Example Code
```c name=operators.c
#include <stdio.h>

int main() {
    int a = 10, b = 20;
    int result;

    // Arithmetic Operators
    result = a + b;
    printf("a + b = %d\n", result);

    result = a - b;
    printf("a - b = %d\n", result);

    result = a * b;
    printf("a * b = %d\n", result);

    result = b / a;
    printf("b / a = %d\n", result);

    result = b % a;
    printf("b %% a = %d\n", result);

    // Relational Operators
    printf("a == b: %d\n", a == b);
    printf("a != b: %d\n", a != b);
    printf("a > b: %d\n", a > b);
    printf("a < b: %d\n", a < b);
    printf("a >= b: %d\n", a >= b);
    printf("a <= b: %d\n", a <= b);

    // Logical Operators
    printf("(a < b) && (a > 0): %d\n", (a < b) && (a > 0));
    printf("(a > b) || (a < 0): %d\n", (a > b) || (a < 0));
    printf("!(a > b): %d\n", !(a > b));

    // Assignment Operators
    a += b;
    printf("a += b: %d\n", a);

    a -= b;
    printf("a -= b: %d\n", a);

    a *= b;
    printf("a *= b: %d\n", a);

    a /= b;
    printf("a /= b: %d\n", a);

    a %= b;
    printf("a %%= b: %d\n", a);

    // Increment and Decrement Operators
    a++;
    printf("a++: %d\n", a);

    b--;
    printf("b--: %d\n", b);

    // Bitwise Operators
    printf("a & b: %d\n", a & b);
    printf("a | b: %d\n", a | b);
    printf("a ^ b: %d\n", a ^ b);
    printf("~a: %d\n", ~a);
    printf("a << 2: %d\n", a << 2);
    printf("a >> 2: %d\n", a >> 2);

    return 0;
}
```

This lesson provides an overview of the basic syntax in C, including data types, variables, constants, and operators. Practice writing and running the provided example codes to reinforce your understanding.

In the next lesson, we will cover control structures, including conditional statements and loops.