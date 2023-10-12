# _Printf

## Introduction
This repository contains an implementation of the `printf` function in C. The goal of this project is to create a custom `printf` function that can format and print text to the standard output according to a given format string.

## Getting Started
To get started with this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository-url>
2. Compilation:
   ```gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o _printf```
3. Usage Example:
```
x@ubuntu:~/c/printf$ cat main.c

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    _printf("%b\n", 98);
    return (0);
}

x@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 main.c
x@ubuntu:~/c/printf$ ./a.out
1100010
x@ubuntu:~/c/printf$
```

## Features
- [x] Basic Formatting
- Handles format specifiers:
%c: Print a single character.
%s: Print a string.
%%: Print a percent sign.
- [x] Handling Numbers
- Extend printf to handle numeric format specifiers:
%d: Print a signed integer.
%i: Print a signed integer.
- [x] - Binary Conversion
- Implement a custom format specifier:
%b: Convert an unsigned integer to binary.
- [x] More Numeric Conversions
- Handle additional numeric format specifiers:
%u: Print an unsigned integer.
%o: Print an unsigned octal number.
%x: Print an unsigned hexadecimal number (lowercase).
%X: Print an unsigned hexadecimal number (uppercase).
- [x] - Buffer Optimization
- Optimize the code by using a local buffer for printing.
- [x] - Printing Non-Printable Characters
- Implement a custom format specifier:
%S: Print strings with non-printable characters represented as \x followed by the ASCII code in hexadecimal.
- [x] Printing Pointers
Handle the %p format specifier to print pointers.
- [x] - Handling Flag Characters
Handle the flag characters:
- [ ] Print a plus sign for positive numbers.
- space: Print a space before positive numbers.
#: Add "0x" for %p and "0" for %o when appropriate.
- [ ] Length Modifiers
- Handle length modifiers:
l: For long integers.
h: For short integers.
- [ ] Field Width
- Implement support for field width in formatting.
- [ ] Precision
- Implement precision support for numeric format specifiers.
- [ ] Flag Character '0'
- Handle the '0' flag character for padding with zeros.
- [ ] Flag Character '-'
- Handle the '-' flag character for left-justified output.
- [x]  Reversed String
- Implement a custom format specifier:
%r: Print the reversed string.
- [x] Rot13 String
- Implement a custom format specifier:
%R: Print the Rot13'ed string.
- [ ] Final Integration
- Ensure all the above options work together seamlessly.

## Contribution and License
This project is under MIT License. To contribute, fork the repository

## Credits
This project was created by [Lewis Safari](https://github.com/safarilewis).

Enjoy Coding!
Happy coding and have fun working on your custom printf function!
