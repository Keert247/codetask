# FibonacciSeries

 The HashMap "fibmap" stores previously computed Fibonacci numbers that improve performance and reduce calculations
 The method fibonacciseries(int n) computes Fibonacci numbers recursively which results in efficiency.
 The function checks if n is negative and throws an IllegalArgumentException if it is.

Base Cases:

fibonacciseries(0)
 return 0
 fibonacciseries(1) 
return 1

Recursive part :
fib(n) = fib(n-1) + fib(n-2)

Time Complexity: O(n)
Space Complexity: O(n)
