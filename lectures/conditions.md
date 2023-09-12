## Conditions in C: When Conditions Become False


Please note that in C, a condition is considered true if it evaluates to a non-zero value and false if it evaluates to zero. The examples provided illustrate the concept of truthiness and falsiness for different data types.

In C, conditions are used to make decisions based on whether an expression is true or false. Below are scenarios in C where conditions become false, including cases involving null values and other data types.

**1. Integer Types:**

- **int, short int, long int, long long int**
  - **False** when the value is 0.
  - **False** when the value is any other integer that evaluates to 0, like `-0`, `0x00`, etc.

    ```c
    int num = 0;
    if (num) {
        // This condition is false because num is 0.
    }
    ```

**2. Floating-Point Types:**

- **float, double, long double**
  - False when the value is 0.0.
  - **False** when the value is any other floating-point value that evaluates to 0.0, like `-0.0`, `0.0f`, etc.

    ```c
    double num = 0.0;
    if (num) {
        // This condition is false because num is 0.0.
    }
    ```

**3. Character Types:**

- **char**
  - **False** when the character is the null character `'\0'`.

    ```c
    char ch = '\0';
    if (ch) {
        // This condition is false because ch is '\0'.
    }
    ```

**4. Other Types:**

- **_Bool**
  - **False** when the value is 0.

    ```c
    _Bool flag = 0;
    if (flag) {
        // This condition is false because flag is 0.
    }
    ```

**5. Pointers:**

- **Any Pointer Type**
  - **False** when the pointer is a null pointer (points to address 0 or is `NULL`).

    ```c
    int *ptr = NULL;
    if (ptr) {
        // This condition is false because ptr is a null pointer.
    }
    ```

These examples cover various data types, including integers, floating-point numbers, characters, and pointers, and demonstrate when conditions become false in C.
