# AssemblyPractice
This repo contains a number of coding exercises completed in C and in MIPS

## Lucas sequences

The focus of these exercises is on [Lucas sequences](https://en.wikipedia.org/wiki/Lucas_sequence), a set of integer sequences that satisfy the following recurrence relation for some coefficients `P` and `Q`:

`L(n) = P*L(n-1) - Q*L(n-2)`

The initial terms `L(0)` and `L(1)` along with the coefficients `P` and `Q` are provided as input. Changing these values will change the Lucas sequence.

## Exercise 1

### Find the maximum number in a sequence

A jumbled Lucas sequence is provided. The program simply traverses this sequence and outputs the largest number.

## Exercise 2

### Define a function to compute L(n)

The next exercise is to define a function to compute a Lucas sequence according to the recurrence relation given above. Compute the Lucas sequence until you reach `L(n)`, and output the entire Lucas sequence from `L(0)` to `L(n).`

Acceptable Assumptions: The maximum value of `n` will be 99, the value of `n` will be nonnegative, and the provided inputs will not produce a sequence with any elements that are outwith the four byte integer range.

This exercise can be done recursively or iteratively.

## Exercise 3

### Determine if a Lucas number is happy

The next exercise is to determine if a given Lucas number is a [happy number](https://en.wikipedia.org/wiki/Happy_number), which is a number that eventually reaches `1` when replaced by the sum of the square of each digit. For instance, `13` is a happy number because `1² + 3² = 10`, and `1² + 0² = 1`.

The input Lucas number is in the `lucas_number` variable. Assume that this number is nonnegative. The output is either `happy` or `sad.`

## Exercise 4

### Compute the Fibonacci word sequence

The final exercise is to compute and print the [Fibonacci word](https://en.wikipedia.org/wiki/Fibonacci_word) sequence, given values for `n` and the initial terms `F(0)` and `F(1)`. Unlike the Fibonacci number sequence, which has integer elements, the elements of the Fibonacci word sequence are strings. For example, given the inputs `4`, `a` and `b`, the output would be: `a` `b` `ab` `bab` `abbab` Assume that the maximum value of `n` will be 25 and that the value of `n` will be nonnegative. Assume that the initial terms `F(0)` and `F(1)` will only be one character long. The MIPS read function will populate the `parameters` array with the values of `n`, `F(0)` and `F(1)`, in this order. The C read function will populate three variables, named `n`, `F(0)` and `F(1)`.
