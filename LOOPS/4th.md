### 1. For Loop:

**Definition:**
A `for` loop in C is used to execute a block of code repeatedly for a specific number of times. It consists of three parts: initialization, condition, and increment/decrement.

**Explanation:**
```c
#include <stdio.h>

int main() {
    // AwkwardPy with a for loop to print numbers 1 to 5
    printf("AwkwardPy ");
    
    // Initialization: int i = 1;
    // Condition: i <= 5;
    // Increment: ++i
    for (int i = 1; i <= 5; ++i) {
        printf("%d ", i);
    }
    
    printf("\n");
    
    return 0;
}
```

In this example, uses a `for` loop to print numbers from 1 to 5. The loop initializes `i` to 1, repeats as long as `i` is less than or equal to 5, and increments `i` after each iteration.

### 2. While Loop:

**Definition:**
A `while` loop in C is used to execute a block of code repeatedly as long as a specified condition is true.

**Explanation:**
```c
#include <stdio.h>

int main() {
    // while loop to print numbers 1 to 5
    printf("AwkwardPy while loop: ");
    
    // Initialization: int i = 1;
    while (i <= 5) {
        printf("%d ", i);
        // Increment: ++i
        ++i;
    }
    
    printf("\n");
    
    return 0;
}
```

In this example, uses a `while` loop to print numbers from 1 to 5. The loop checks the condition `i <= 5` and repeats the code block as long as the condition is true.

### 3. Do-While Loop:

**Definition:**
A `do-while` loop in C is similar to the `while` loop but guarantees that the block of code is executed at least once, even if the condition is initially false.

**Explanation:**
```c
#include <stdio.h>

int main() {
    // with a do-while loop to print numbers 1 to 5
    printf("AwkwardPy do-while loop: ");
    
    // Initialization: int i = 1;
    do {
        printf("%d ", i);
        // Increment: ++i
        ++i;
    } while (i <= 5);
    
    printf("\n");
    
    return 0;
}
```

In this example, uses a `do-while` loop to print numbers from 1 to 5. The loop executes the code block and then checks the condition `i <= 5`. If true, it repeats the loop.
