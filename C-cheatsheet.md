### C Programming Cheat Sheet

#### 1. Basics
   - **Program Structure**: 
     ```c
     #include <stdio.h>
     
     int main() {
         // Code
         return 0;
     }
     ```
   - **Comments**:
     ```c
     // Single-line comment
     /* Multi-line comment */
     ```

#### 2. Data Types
   - **Primitive Types**:
     - `int` – Integer (whole numbers)
     - `float` – Floating-point number (single precision)
     - `double` – Double precision floating-point
     - `char` – Single character
     - `void` – No value (used in functions)

   - **Modifiers**:
     - `short`, `long`, `signed`, `unsigned`
     - Example: `long int`, `unsigned char`

#### 3. Variables and Constants
   - **Variable Declaration**:
     ```c
     int x = 10;
     float y = 3.14;
     ```
   - **Constant Declaration**:
     ```c
     const int z = 100;
     ```

#### 4. Input/Output
   - **Input** (`scanf`):
     ```c
     int x;
     scanf("%d", &x);
     ```
   - **Output** (`printf`):
     ```c
     int x = 10;
     printf("Value: %d", x);
     ```

#### 5. Operators
   - **Arithmetic**: `+`, `-`, `*`, `/`, `%`
   - **Relational**: `==`, `!=`, `>`, `<`, `>=`, `<=`
   - **Logical**: `&&`, `||`, `!`
   - **Bitwise**: `&`, `|`, `^`, `~`, `<<`, `>>`
   - **Assignment**: `=`, `+=`, `-=`, `*=`, `/=`, `%=` 

#### 6. Control Structures*
   - **If-else**:
     ```c
     if (condition) {
         // Code
     } else {
         // Code
     }
     ```
   - **Switch**:
     ```c
     switch (expression) {
         case value1:
             // Code
             break;
         case value2:
             // Code
             break;
         default:
             // Code
     }
     ```

   - **Loops**:
     - **For loop**:
       ```c
       for (int i = 0; i < 10; i++) {
           // Code
       }
       ```
     - **While loop**:
       ```c
       while (condition) {
           // Code
       }
       ```
     - **Do-while loop**:
       ```c
       do {
           // Code
       } while (condition);
       ```

#### 7. Functions
   - **Syntax**:
     ```c
     returnType functionName(parameters) {
         // Code
         return value;
     }
     ```
   - **Example**:
     ```c
     int add(int a, int b) {
         return a + b;
     }
     ```

#### 8. Pointers
   - **Declaration**:
     ```c
     int *ptr;
     ```
   - **Assigning Address**:
     ```c
     int x = 10;
     int *ptr = &x;
     ```
   - **Dereferencing**:
     ```c
     printf("%d", *ptr);  // Output: 10
     ```

#### 9. Arrays
   - **Declaration**:
     ```c
     int arr[5];
     ```
   - **Initialization**:
     ```c
     int arr[] = {1, 2, 3, 4, 5};
     ```
   - **Accessing Elements**:
     ```c
     printf("%d", arr[0]);  // Output: 1
     ```

#### 10. Strings
   - **Declaration**:
     ```c
     char str[20];
     ```
   - **Initialization**:
     ```c
     char str[] = "Hello";
     ```
   - **Standard Library Functions**: `strlen()`, `strcpy()`, `strcmp()`

#### 11. Structures
   - **Declaration**:
     ```c
     struct Person {
         char name[50];
         int age;
     };
     ```
   - **Accessing Members**:
     ```c
     struct Person p1;
     p1.age = 25;
     ```

#### 12. File Handling
   - **Opening a File**:
     ```c
     FILE *fptr = fopen("filename.txt", "r");
     ```
   - **Closing a File**:
     ```c
     fclose(fptr);
     ```
   - **Reading/Writing**:
     ```c
     fprintf(fptr, "Hello World!");
     fscanf(fptr, "%s", str);
     ```

#### 13. Dynamic Memory Allocation
   - **`malloc` and `free`**:
     ```c
     int *ptr = (int*) malloc(sizeof(int));
     free(ptr);
     ```
   - **`calloc`**:
     ```c
     int *ptr = (int*) calloc(10, sizeof(int));
     ```
   - **`realloc`**:
     ```c
     ptr = (int*) realloc(ptr, 20 * sizeof(int));
     ```

#### 14. Preprocessors
   - **Macros**:
     ```c
     #define PI 3.14159
     ```
   - **Conditional Compilation**:
     ```c
     #ifdef DEBUG
         // Debugging code
     #endif
     ```

#### 15. Error Handling
   - **Using `errno`**:
     ```c
     if (file == NULL) {
         printf("Error opening file: %s", strerror(errno));
     }
     ```

#### 16. Recursion
   - **Example**:
     ```c
     int factorial(int n) {
         if (n == 0) return 1;
         return n * factorial(n - 1);
     }
     ```

#### 17. Command Line Arguments
   - **Main Function Signature**:
     ```c
     int main(int argc, char *argv[]) {
         // Code
     }
     ```

#### 18. Common Standard Library Functions
   - **Math functions**: `sqrt()`, `pow()`, `abs()`
   - **String functions**: `strlen()`, `strcpy()`, `strcat()`
   - **I/O functions**: `printf()`, `scanf()`, `fgets()`, `fputs()`

#### 19. Type Casting
   - **Example**:
     ```c
     float f = (float) 5 / 2;  // Result: 2.5
     ```

