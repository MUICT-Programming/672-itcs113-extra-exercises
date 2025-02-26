# Fundamentals of C Programming - Practice Questions

## Data Types: `int`, `char`, `float`

1. What is the difference between `int`, `char`, and `float` in C?
2. How much memory does an `int`, `char`, and `float` typically occupy in C?
3. What will be the output of the following code?

   ```c
   char ch = 'A';
   printf("%d", ch);
   ```

4. Which of the following is a valid declaration?  
   a. `int num = 10.5;`  
   b. `char ch = "A";`  
   c. `float f = 12.34;`  
5. What is the output of:

   ```c
   float x = 10 / 3;
   printf("%f", x);
   ```

6. Can we store a `char` value in an `int` variable? Why or why not?
7. What is the difference between `float` and `double` in terms of precision?
8. What is the output of:

   ```c
   char ch = '5';
   int num = ch - '0';
   printf("%d", num);
   ```

9. What is the default data type of a numeric constant without a decimal in C?
10. What will happen if we assign a floating-point value to an `int` variable?

---

## Arithmetic Operations (`+`, `-`, `/`, `*`, `%`)

1. What is the result of `5 / 2` in C?
2. What will be the output of:

   ```c
   int a = 7, b = 2;
   printf("%f", a / b);
   ```

3. Why does `printf("%d", 10 / 3);` not produce `3.3333`?
4. What is the remainder when `19 % 4` is calculated?
5. Can the modulus (`%`) operator be used with `float` data type? Why or why not?
6. What is the output of:

   ```c
   int a = 5;
   printf("%d", a++ * 2);
   ```

7. Rewrite `a = a + 10;` using shorthand notation.
8. What is the difference between `a++` and `++a`?
9. What will be the value of `x` after:

   ```c
   int x = 10;
   x += 5 * 2;
   ```

10. What is the output of:

   ```c
   printf("%d", 10 * 2 / 5 + 3);
   ```

---

## `scanf` and `printf`

1. How do you take an integer input from the user in C?
2. What will happen if `scanf("%d", &x);` is used but `&x` is missing?
3. What format specifier should be used to print a character?
4. What is the output of:

   ```c
   printf("%c", 'A' + 1);
   ```

5. Can `printf` be used to print multiple values at once? Give an example.
6. What is the output of:

   ```c
   printf("%5d", 10);
   ```

7. Why is the `&` operator necessary in `scanf`?
8. What is the correct way to read a string input using `scanf`?
9. What happens if we input a float value when using `scanf("%d", &x);`?
10. What does the escape sequence `\t` do in `printf`?

---

## Conditional Statements (`if`, `if-else`, `chained if-else`)

1. What is the difference between `if` and `if-else`?
2. What is the output of:

   ```c
   if (5 > 3)
       printf("Hello");
       printf("World");
   ```

3. Why does this condition always return true?

   ```c
   if (x = 10)
   ```

4. What is the output of:

   ```c
   int x = 5;
   if (x < 10)
       printf("A");
   else
       printf("B");
   ```

5. How many conditions are evaluated in:

   ```c
   if (x > 10)
       printf("A");
   else if (x == 10)
       printf("B");
   else
       printf("C");
   ```

6. Write a program to check if a number is even or odd using `if-else`.
7. Can `else` exist without `if`?
8. How does short-circuit evaluation work in:

   ```c
   if (x > 0 && y > 5)
   ```

9. What is the difference between `==` and `=` inside an `if` condition?
10. Write an `if-else` condition that checks if a character is a vowel or consonant.

---

## Loops (`for`, `while`, `do-while`)

1. What is the difference between `for`, `while`, and `do-while` loops?
2. What will be the output of:

   ```c
   for (int i = 0; i < 5; i++)
       printf("%d ", i);
   ```

3. Can a `while` loop execute zero times?
4. What is the output of:

   ```c
   int x = 5;
   while (x-- > 0)
       printf("%d ", x);
   ```

5. What is the syntax of a `do-while` loop?
6. What happens if the loop condition is always true?
7. Write a `for` loop that prints numbers from 10 to 1.
8. How do you terminate a loop prematurely?
9. What is the purpose of `continue` in loops?
10. Write a `while` loop to calculate the sum of digits of a number.
11. Write a while statement to print out the numbers with the following patterns:

    ```text
    1, 3, 5, 7, 9
    10, 8, 6, 4, 2
    1, 1, 1, 1, 1, 1, 1, 1, 1, 1
    a, b, c, d, e, f, g, h, i, j, k
    1, 2, 4, 8, 16, 32
    1, 2, 4, 5, 7, 8, 10, 11, 13, 14, 16, 17, 19, 20
    1c, 2f, 3c, 4f, 5c, 6f, 7c, 8f, 9c, 10f
    1a, 2b, 3c, 4d, 5e, 6f, 7g, 8h, 9i, 10j
    ```

12. Write a program to print all even numbers between 1 to n.
13. Write a program to print all odd numbers between 1 to n.
14. Write a program to sum all numbers between 1 to n.
15. Write a program to sum all even numbers between 1 to n.
16. Write a program to print Factorial of n (e.g. 5 = 1 x 2 x 3 x 4 x 5 ).
17. Write a program that repeatedly receives the numbers (0 to 9) from the user. It will stop when the user inputs `'q'`.
18. Write a program that repeatedly receives the negative numbers. It will stop when the user inputs a positive number.
19. Write a program that repeatedly receives the numbers and find the average until users inputs `'q'`.
20. Write a program that receive and validate a customer ID to be between 100 and 999 (inclusive). If not, continue to ask for a customer ID until a user has input the valid one. Finally, print out the valid customer ID.
21. Write a program that receives an input n from users where n is 2 to 9 (inclusively) then calculate the area of a square size n. You must validate n before calculating; otherwise, keep asking users to input a new valid n.

---

## Nested Loops

1. What is a nested loop in C?
2. How many times does the inner loop execute in the following code?

   ```c
   for (int i = 0; i < 3; i++)
       for (int j = 0; j < 4; j++)
           printf("* ");
   ```

3. Write a nested loop to print a right-angled triangle of stars.
4. What will be the output of the following nested loop?

   ```c
   for (int i = 1; i <= 3; i++) {
       for (int j = 1; j <= i; j++) {
           printf("%d ", j);
       }
       printf("\n");
   }
   ```

5. How can you modify a nested loop to print an inverted right-angled triangle?
6. Write a program using nested loops to print a multiplication table for numbers 1 to 5.
7. Can a `while` loop be nested inside a `for` loop? Provide an example.
8. What happens if both loops in a nested loop have the same control variable?
9. How do you traverse a 2D array using nested loops?
10. What is the time complexity of a nested loop where both loops iterate `n` times?
11. Write a nested loop to print the following pyramid pattern:

    ```text
       *
      ***
     *****
    ```

12. How can you use multiple inner loops to create a diamond pattern?
13. Modify a nested loop to print the following number pattern:

    ```text
    1
    1 2
    1 2 3
    1 2 3 4
    ```

14. Write a program using nested loops to generate a checkerboard pattern using `*` and spaces.
15. How do you print a hollow square pattern with nested loops?
16. Write a nested loop to print a Pascal’s Triangle pattern.
17. How can you use nested loops to generate a Fibonacci triangle?
18. Modify a nested loop to print a mirrored right-angled triangle:

    ```text
         *
       **
     ***
    ****
    ```

19. Write a nested loop to print a full pyramid of numbers:

    ```text
       1
      2 2
     3 3 3
    4 4 4 4
    ```

20. Create a nested loop that prints a pattern where each row contains the row number repeated:

    ```text
    1
    2 2
    3 3 3
    4 4 4 4
    ```

21. Write a nested loop to print a solid square pattern of `*` characters.

   ```text
   ****
   ****
   ****
   ****
   ```

22. Modify the square pattern to print a hollow square with `*` on the borders.

   ```text
   ****
   *  *
   *  *
   ****
   ```

23. How can you change the loop to print a square with numbers instead of `*`?

   ```text
   1111
   2222
   3333
   4444
   ```

24. Write a program to print a checkerboard pattern using `*` and spaces.

   ```text
   * * * *
    * * * *
   * * * *
    * * * *
   ```

25. How do you modify the square pattern to use numbers increasing from left to right?

   ```text
   1234
   1234
   1234
   1234
   ```

26. Write a nested loop to print a full pyramid of numbers where each row contains the row number repeated.

   ```text
       1
      222
     33333
    4444444
   ```

27. How do you modify the pyramid pattern to print numbers in increasing order across each row?

   ```text
       1
      1 2
     1 2 3
    1 2 3 4
   ```

28. Write a program to print an inverted pyramid of numbers.

   ```text
   4444444
    33333
     222
      1
   ```

29. Modify the pyramid pattern to print the sum of the row index at each position.

   ```text
       1
      2 3
     3 4 5
    4 5 6 7
   ```

30. How can you use nested loops to center-align a pyramid pattern?

    ```text
        1
       121
      12321
     1234321
    ```

31. Write a nested loop to print Floyd’s Triangle using consecutive numbers.

    ```text
    1
    2 3
    4 5 6
    7 8 9 10
    ```

32. Modify Floyd’s Triangle to use only even numbers.

    ```text
    2
    4 6
    8 10 12
    14 16 18 20
    ```

33. Write a program to print an inverted Floyd’s Triangle.

    ```text
    7 8 9 10
    4 5 6
    2 3
    1
    ```

34. How do you modify Floyd’s Triangle to print each row in reverse order?

    ```text
    1
    3 2
    6 5 4
    10 9 8 7
    ```

35. Create a nested loop that prints Floyd’s Triangle but replaces odd numbers with `*`.

    ```text
    *
    2 *
    4 * 6
    * 8 * 10
    ```

36. Write a nested loop to print an 8x8 chessboard pattern with `*` and spaces.

    ```text
    * * * * * * * *
     * * * * * * * *
    * * * * * * * *
     * * * * * * * *
    ```

37. Modify the chessboard pattern to allow user-defined dimensions.
38. How can you change the chessboard pattern to print numbers instead of `*`?

    ```text
    1 2 3 4 5
     6 7 8 9 10
    11 12 13 14 15
     16 17 18 19 20
    ```

39. Write a program to create a dynamic chessboard where alternate cells contain random numbers.
40. Modify the chessboard pattern to print a hollow chessboard outline with `*` only on the borders.

    ```text
    ********
    *      *
    *      *
    ********
    ```

41. Write a nested loop to print a diamond pattern using `*`.

    ```text
       *
      ***
     *****
      ***
       *
    ```

42. Modify the diamond pattern to print numbers increasing from the center outward.

    ```text
       1
      123
     12345
      123
       1
    ```

43. How can you create a nested loop to print a hollow diamond pattern?

    ```text
       *
      * *
     *   *
      * *
       *
    ```

44. Write a program that generates a diamond pattern where even-numbered rows contain `#` instead of `*`.
45. Modify the diamond pattern to create a double-layered diamond with alternating characters.

    ```text
       *
      *#*
     *#*#*
      *#*
       *
    ```

## 1D Arrays

1. How do you declare a 1D array in C?
2. How do you initialize a 1D array with specific values?
3. Write a program to find the largest element in a 1D array.

   ```text
   Enter the number of elements: 5
   Enter elements: 10 25 67 34 89
   Largest element: 89
   ```

4. How do you take input into an array using a loop?
5. Write a program to reverse a 1D array.

   ```text
   Original array: 1 2 3 4 5
   Reversed array: 5 4 3 2 1
   ```

6. How do you calculate the sum of all elements in a 1D array?

   ```text
   Enter elements: 5 10 15 20 25
   Sum of elements: 75
   ```

7. Write a function to find the average value of a 1D array.
8. How do you search for a specific element in a 1D array?

   ```text
   Enter elements: 3 6 9 12 15
   Enter element to search: 9
   Element found at index 2
   ```

9. Write a program to sort a 1D array in ascending order.

   ```text
   Unsorted array: 5 2 8 1 3
   Sorted array: 1 2 3 5 8
   ```

10. How can you copy one array into another using a loop?

## 2D Arrays

1. How do you declare a 2D array in C?
2. How do you initialize a 2D array with specific values?
3. Write a program to print the elements of a 2D array in row-major order.

   ```text
   1 2 3
   4 5 6
   7 8 9
   ```

4. How do you take input into a 2D array using nested loops?
5. Write a program to find the largest element in a 2D array.

   ```text
   Enter matrix:
   3 8 2
   6 7 9
   1 4 5
   Largest element: 9
   ```

6. How do you calculate the sum of all elements in a 2D array?

   ```text
   Enter matrix:
   1 2 3
   4 5 6
   7 8 9
   Sum of all elements: 45
   ```

7. Write a function to find the sum of each row in a 2D array.

   ```text
   Row 1 sum: 6
   Row 2 sum: 15
   Row 3 sum: 24
   ```

8. How do you search for a specific element in a 2D array?

   ```text
   Enter matrix:
   3 5 7
   2 8 6
   1 4 9
   Enter element to search: 8
   Element found at row 2, column 2
   ```

9. Write a program to find the transpose of a 2D array.

   ```text
   Original matrix:
   1 2 3
   4 5 6
   7 8 9
   Transposed matrix:
   1 4 7
   2 5 8
   3 6 9
   ```

10. How can you multiply two 2D matrices using nested loops?

      ```text
      Matrix A:
      1 2
      3 4
      Matrix B:
      5 6
      7 8
      Resultant Matrix:
      19 22
      43 50
      ```
