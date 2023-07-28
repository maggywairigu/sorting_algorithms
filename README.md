# Toggle Navigation - Sorting Algorithms & Big O

![Toggle Navigation](https://your-project-image-url)

Welcome to the Toggle Navigation project for Sorting Algorithms and Big O! This project is to be completed in teams of 2 people, and your team members are Margaret Maina. In this project, you will learn about various sorting algorithms, the Big O notation to evaluate the time complexity of algorithms, and how to select the best sorting algorithm for a given input.

## Learning Objectives

By the end of this project, you should be able to explain the following concepts without the help of Google:

1. At least four different sorting algorithms
2. What is the Big O notation, and how to evaluate the time complexity of an algorithm
3. How to select the best sorting algorithm for a given input
4. What is a stable sorting algorithm

## Requirements

### General

- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 20.04 LTS using gcc, with the options `-Wall -Werror -Wextra -pedantic -std=gnu89`.
- All your files should end with a new line.
- A `README.md` file at the root of the project folder is mandatory.
- Your code should follow the Betty style. It will be checked using `betty-style.pl` and `betty-doc.pl`.
- You are not allowed to use global variables.
- Each file should contain no more than 5 functions.
- Unless specified otherwise, you are not allowed to use the standard library. Functions like `printf`, `puts`, and others are forbidden.
- The prototypes of all your functions should be included in your header file called `sort.h`.
- Don't forget to push your header file.
- All your header files should be include guarded.
- A list/array does not need to be sorted if its size is less than 2.
- There should be one project repository per group. If you clone/fork/whatever a project repository with the same name before the second deadline, you risk a 0% score.

### Resources

Before starting the project, make sure to read or watch the following resources:

- Sorting algorithm
- Big O notation
- Sorting algorithms animations

### Data Structure and Functions

For this project, you are provided with the following `print_array` and `print_list` functions:

```c
#include <stdlib.h>
#include <stdio.h>

/**
 * print_array - Prints an array of integers
 *
 * @array: The array to be printed
 * @size: Number of elements in @array
 */
void print_array(const int *array, size_t size)
{
    size_t i;

    i = 0;
    while (array && i < size)
    {
        if (i > 0)
            printf(", ");
        printf("%d", array[i]);
        ++i;
    }
    printf("\n");
}

#include <stdio.h>
#include "sort.h"

/**
 * print_list - Prints a list of integers
 *
 * @list: The list to be printed
 */
void print_list(const listint_t *list)
{
    int i;

    i = 0;
    while (list)
    {
        if (i > 0)
            printf(", ");
        printf("%d", list->n);
        ++i;
        list = list->next;
    }
    printf("\n");
}
```

The files `print_array.c` and `print_list.c` (containing the `print_array` and `print_list` functions) will be compiled with your functions during the correction.

## Sorting Algorithm Tasks

The project consists of several tasks where you will implement various sorting algorithms and analyze their Big O notations. Here are the tasks you need to complete:

1. Bubble sort
2. Insertion sort
3. Selection sort
4. Quick sort
5. Shell sort - Knuth Sequence
6. Cocktail shaker sort (Advanced)
7. Counting sort (Advanced)
8. Merge sort (Advanced)
9. Heap sort (Advanced)
10. Radix sort (Advanced)
11. Bitonic sort (Advanced)
12. Quick Sort - Hoare Partition scheme (Advanced)
13. Dealer (Advanced)

Please refer to each individual file for the specific instructions and requirements for each task.

## Running and Testing

To test your sorting algorithms with big sets of random integers, you can use the website [Random.org](https://www.random.org/). The provided `main.c` files in the examples are for reference only, and you don't need to push them to your repository.

## How to Use This Repository

This repository contains all the required files for the Toggle Navigation - Sorting Algorithms & Big O project. Each task is implemented in a separate file, and the header file `sort.h` contains the function prototypes.

To compile the programs, you can use the provided `gcc` command:

```
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 -o <output_file> <source_file.c>
```

To test your sorting algorithms, you can create your own `main.c` files or use the provided examples as a reference.

## Conclusion

This project will help you gain a deeper understanding of sorting algorithms and their time complexities. Completing each task successfully will improve your problem-solving skills and knowledge of data structures and algorithms.

Good luck with your project, and happy coding!

## Authors

- [Margaret Maina](https://github.com/maggywairigu)

(C) 2023 ALX. All rights reserved