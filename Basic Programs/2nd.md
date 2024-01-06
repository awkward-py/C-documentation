### 1. Hello World:

```c
#include <stdio.h>

int main() {
    // This program prints the message "Hello, World!" to the console
    printf("Hello, World!\n");
    return 0;
}
```

**Explanation:**
- `#include <stdio.h>`: This line includes the standard input/output library, allowing the use of functions like `printf`.
- `int main()`: The main function, where the program starts execution.
- `printf("Hello, World!\n");`: Prints the message to the console.
- `return 0;`: Indicates successful execution.

### 2. Input and Output:

```c
#include <stdio.h>

int main() {
    // This program takes input from the user and prints it
    int num;
    
    printf("Enter a number: ");
    scanf("%d", &num);
    
    printf("You entered: %d\n", num);
    
    return 0;
}
```

**Explanation:**
- `int num;`: Declares an integer variable.
- `printf("Enter a number: ");`: Prompts the user to enter a number.
- `scanf("%d", &num);`: Reads an integer from the user.
- `printf("You entered: %d\n", num);`: Prints the entered number.

### 3. Arithmetic Operations:

```c
#include <stdio.h>

int main() {
    // This program performs basic arithmetic operations
    int a = 5, b = 3;
    
    printf("Sum: %d\n", a + b);
    printf("Difference: %d\n", a - b);
    printf("Product: %d\n", a * b);
    printf("Quotient: %d\n", a / b);
    
    return 0;
}
```

**Explanation:**
- `int a = 5, b = 3;`: Initializes two integer variables.
- `printf("Sum: %d\n", a + b);`: Prints the sum of `a` and `b`.
- Similarly, prints the difference, product, and quotient.

### 4. Conditional Statements:

```c
#include <stdio.h>

int main() {
    // This program checks if a number is even or odd
    int num;
    
    printf("Enter a number: ");
    scanf("%d", &num);
    
    if (num % 2 == 0) {
        printf("Even number\n");
    } else {
        printf("Odd number\n");
    }
    
    return 0;
}
```

**Explanation:**
- `if (num % 2 == 0)`: Checks if the entered number is divisible by 2 (even).
- `else`: Handles the case if the number is not even (odd).

### 5. Loops - Printing Numbers 1 to 5:

```c
#include <stdio.h>

int main() {
    // This program uses a loop to print numbers from 1 to 5
    for (int i = 1; i <= 5; ++i) {
        printf("%d ", i);
    }
    
    printf("\n");
    
    return 0;
}
```

**Explanation:**
- `for (int i = 1; i <= 5; ++i)`: A loop that iterates from 1 to 5.
- `printf("%d ", i);`: Prints the current value of `i`.
- `printf("\n");`: Adds a newline after printing the numbers.

### 6. Functions - Sum of Two Numbers:

```c
#include <stdio.h>

// Function to add two numbers
int add(int a, int b) {
    return a + b;
}

int main() {
    // This program uses a function to find the sum of two numbers
    int num1 = 5, num2 = 3;
    
    printf("Sum: %d\n", add(num1, num2));
    
    return 0;
}
```

**Explanation:**
- `int add(int a, int b)`: Defines a function named `add` that takes two integers and returns their sum.
- `printf("Sum: %d\n", add(num1, num2));`: Calls the `add` function to find and print the sum of `num1` and `num2`.
