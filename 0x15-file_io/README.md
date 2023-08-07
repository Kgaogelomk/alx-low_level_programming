This project aims to implement a function that reads a text file and prints its contents to the POSIX standard output. The function, `read_textfile`, takes the name of the file to be read and the number of letters to be read and printed as arguments.

## Requirements

- Ubuntu 20.04 LTS
- gcc compiler with the options: `-Wall -Werror -Wextra -pedantic -std=gnu89`
- Text file to read
- main.h header file

## Function Prototype

c
ssize_t read_textfile(const char *filename, size_t letters);


## Function Signature

The `read_textfile` function has the following signature:

c
ssize_t read_textfile(const char *filename, size_t letters);


- `filename`: Name of the file to be read.
- `letters`: Number of letters to read and print.

## Return Value

- The `read_textfile` function returns the actual number of letters read and printed.
- If the file cannot be opened or read, it returns 0.
- If `filename` is NULL, it returns 0.
- If the write operation fails or does not write the expected amount of bytes, it returns 0.

## Allowed Editors

You can use the following editors for this project:

- vi
- vim
- emacs

## Compilation

All files in this project should be compiled using the gcc compiler with the options `-Wall -Werror -Wextra -pedantic -std=gnu89`.

## Files

The project consists of the following files:

- `main.c` (example main file for testing, not required to push)
- `main.h` (header file with function prototype)
- `read_textfile.c` (implementation of the `read_textfile` function)

## Development Requirements

- Use the Betty style for code formatting.
- Limit the number of functions in each file to a maximum of 5.
- Do not use global variables.
- Use only the following C Standard Library functions: `malloc`, `free`, and `exit`.
- Allowed system calls: `read`, `write`, `open`, and `close`.
- `_putchar` function is allowed to be used.
- Do not include or push `_putchar.c`.

## Usage

To test the `read_textfile` function, you can use the provided `main.c` file (not required to push). Make sure to include the `main.h` header file in your program.

The `read_textfile` function reads the specified file and prints its contents to the standard output. The name of the file and the desired number of letters to read and print should be passed as arguments to the function. The function returns the actual number of letters read and printed. If any errors occur during file opening, reading, or writing, the function returns 0.

## Example

c
#include "main.h"

int main(void)
{
    ssize_t letters_read;

    letters_read = read_textfile("input.txt", 100);
    printf("Number of letters read and printed: %ld\n", letters_read);
    return (0);
}


## Conclusion

This O/I Coding project provides a function `read_textfile` that can read a text file and print its contents to the POSIX standard output. The implementation adheres to all the specified requirements and restrictions outlined in the task description.

