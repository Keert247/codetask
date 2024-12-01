# FibonacciSeries

 The HashMap "fibmap" stores previously computed Fibonacci numbers that improve performance and reduce calculations
 The method fibonacciseries(int n) computes Fibonacci numbers recursively which results in efficiency.
 The function checks if n is negative and throws an IllegalArgumentException if it has.

base test Cases:

fibonacciseries(0)
 return 0
 fibonacciseries(1) 
return 1

Recursive part :
fib(n) = fib(n-1) + fib(n-2)

Time Complexity: O(n)
The function makes n recursive calls, and for each call it either computes the value or retrieves it from the map 
and calculate each Fibonacci number only once.

Space Complexity: O(n)
The HashMap stores the Fibonacci values for each index from 0 to n, the space complexity due to the HashMap is O(n) it stores up to n Fibonacci numbers.
The recursion depth is at most n because the Fibonacci function is called recursively for n-1 and n-2 in a linear manner. The recursive call stack contributes an additional O(n) 

--------------------------------------------------------------------------
# Balanced Substring

A substring is considered balanced if:

It contains exactly two distinct characters.
Each of these characters appears an equal number of times.
Features
Identify all longest balanced substrings from the input
Handle cases where no balanced substrings exist


it finds all possible substrings of the input string.
For each substring, it checks if it is balanced
-The substring should have exactly two distinct characters
-Both characters should occur the same number of time
-Tracks the longest balanced substrings
Output: An array containing all the longest balanced substrings.

Method implementaion :
getBalancedSubstrings(String s)

Iterates over all substrings of s using nested loops.
For each substring, calls the isBalanced method to determine if it's balanced.
Keeps track of the maximum length of balanced substrings that is found already
Returns all substrings which matches the maximum length.


isBalanced(String substring) :
Checks if a substring is balanced.
Counts the frequency of each character in the substring using a HashMap.
Validates if there are exactly two distinct characters, and their frequencies are equal.


Time Complexity : O(n cube)  complexity for checking all substrings
Space Complexity:O(n square) the space required to store substrings in longsubstr 




