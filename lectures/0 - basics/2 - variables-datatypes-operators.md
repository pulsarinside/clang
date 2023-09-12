## Variables, Data Types, and Operators in C

### Integer Types

- **int**
  - Size: Typically 4 bytes on most systems
  - Default Value: 0
  - Example:
    ```c
    int number = 42;
    ```

- **short int**
  - Size: Typically 2 bytes
  - Default Value: 0
  - Example:
    ```c
    short int temperature = -10;
    ```

- **long int**
  - Size: Typically 4 or 8 bytes
  - Default Value: 0
  - Example:
    ```c
    long int population = 7000000000;
    ```

- **long long int**
  - Size: Typically 8 bytes
  - Default Value: 0
  - Example:
    ```c
    long long int bigNumber = 9876543210;
    ```

### Floating-Point Types

- **float**
  - Size: Typically 4 bytes
  - Default Value: 0.0
  - Example:
    ```c
    float pi = 3.14159265359;
    ```

- **double**
  - Size: Typically 8 bytes
  - Default Value: 0.0
  - Example:
    ```c
    double salary = 55000.50;
    ```

- **long double**
  - Size: System-dependent (usually larger than `double`)
  - Default Value: 0.0
  - Example:
    ```c
    long double preciseValue = 123456789.987654321;
    ```

### Character Types

- **char**
  - Size: Typically 1 byte
  - Default Value: '\0' (null character)
  - Example:
    ```c
    char grade = 'A';
    ```

### Other Types

- **_Bool**
  - Size: Implementation-defined
  - Default Value: 0 (false)
  - Example:
    ```c
    _Bool isTrue = 1;
    ```

### Modifiers

- **signed**
  - Can be applied to integer types like `int`, `short int`, etc., to indicate that the type can represent both positive and negative values (default behavior).

- **unsigned**
  - Can be applied to integer types to indicate that the type should only represent non-negative values (i.e., no sign bit).

### Operators

C provides various operators to perform operations on variables and data. Here are some common operators:

- **Arithmetic Operators:** `+`, `-`, `*`, `/`, `%`
- **Comparison Operators:** `==`, `!=`, `<`, `>`, `<=`, `>=`
- **Logical Operators:** `&&`, `||`, `!`
- **Assignment Operators:** `=`, `+=`, `-=`, `*=`, `/=`, `%=`
- **Increment and Decrement Operators:** `++`, `--`
- **Bitwise Operators (for integers):** `&`, `|`, `^`, `~`, `<<`, `>>`
- **Ternary Operator:** `? :` (conditional operator)

These are some of the fundamental data types, operators, and their default values in C. Understanding them is essential for writing C programs effectively.
