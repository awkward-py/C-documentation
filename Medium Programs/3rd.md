### 1. Calculate Factorial:

```c
#include <stdio.h>

// Function to calculate factorial
int factorial(int n) {
    if (n == 0 || n == 1) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}

int main() {
    // This program calculates the factorial of a number
    int num;
    
    printf("Enter a number: ");
    scanf("%d", &num);
    
    printf("Factorial of %d: %d\n", num, factorial(num));
    
    return 0;
}
```

**Explanation:**
- `factorial(int n)`: A recursive function to calculate the factorial of a number.
- `if (n == 0 || n == 1)`: Handles the base case for factorial (0! and 1! are both 1).
- `return n * factorial(n - 1);`: Recursive call to calculate factorial.

### 2. Reverse a Number:

```c
#include <stdio.h>

// Function to reverse a number
int reverseNumber(int num) {
    int reversed = 0;

    while (num != 0) {
        reversed = reversed * 10 + num % 10;
        num /= 10;
    }

    return reversed;
}

int main() {
    // This program reverses a given number
    int num;
    
    printf("Enter a number: ");
    scanf("%d", &num);
    
    printf("Reversed number: %d\n", reverseNumber(num));
    
    return 0;
}
```

**Explanation:**
- `reverseNumber(int num)`: A function to reverse a given number.
- `while (num != 0)`: Loop iterates until the number becomes 0.
- `reversed = reversed * 10 + num % 10;`: Builds the reversed number digit by digit.

### 3. Find Prime Numbers in a Range:

```c
#include <stdio.h>

// Function to check if a number is prime
int isPrime(int num) {
    if (num < 2) {
        return 0;
    }

    for (int i = 2; i <= num / 2; ++i) {
        if (num % i == 0) {
            return 0;
        }
    }

    return 1;
}

int main() {
    // This program finds prime numbers in a given range
    int start, end;
    
    printf("Enter the range (start and end): ");
    scanf("%d %d", &start, &end);
    
    printf("Prime numbers in the range [%d, %d]: ", start, end);

    for (int i = start; i <= end; ++i) {
        if (isPrime(i)) {
            printf("%d ", i);
        }
    }

    printf("\n");
    
    return 0;
}
```

**Explanation:**
- `isPrime(int num)`: A function to check if a number is prime.
- `for (int i = 2; i <= num / 2; ++i)`: Loop to check divisibility from 2 to num/2.
