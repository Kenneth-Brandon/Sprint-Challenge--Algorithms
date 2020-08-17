#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)
O(n) - For n * n * n = n^3, as n gets bigger, the amount of loops in the while loop increases exponentially. However, in the loop, value a increases by a + n * n in each iteration, which reduces the amount of loop down to n * n * n / (a+ n * n), which is less than n. We can drop whatever constant n has after and call it O(n) complexity.

b)
O(log n) - First for loop has the time complexity of O(n). The inner while loop can be considered O(log n) because value j is doubling in each iteration. Doubling/halving behavior always gets O(log n) time complexity since the amount of change is increasing/decreasing in double/half amount of the input.

c)
O(n) - This is a recursive operation. The function calls itself only once with (n - 1) parameter in its return statement. Therefore, the stack size will be directly proportional to the input size since the base case is n = 0.

## Exercise II

My strategy would be to use a binary search.

First take the number of floors in this n-story building and divide it by 2 to find the middle n // 2 Drop an egg from that floor. If it breaks (returns True), find the new middle by using the old middle (result of n // 2) as the new n (n // 2) // 2 Drop an egg from this floor. If it breaks (returns True), repeat the process of finding the new middle and dropping eggs until the egg can fall without breaking (returns False)

Time complexity of a binary search is O(log n)
