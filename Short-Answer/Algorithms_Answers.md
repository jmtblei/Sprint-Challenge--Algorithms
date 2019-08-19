Add your answers to the Algorithms exercises here.

## exercise 1
a) O(n)
the algorithm jumps by n^2 each time, but the while loop will run n time

b) O(n^3)
it's a triple for loop so it will run n time, but because it's nested we multiply each instance

c) O(n)
recursion will call itself running it down in n time

## exercise 2
you can take a linear or a binary approach 

linear approach:
-start at floor 1 and drop the egg
-given n floors, you repeat the drop until the egg breaks
-the _f_ floor is the floor the egg breaks
time complexity will be O(n) because your text runs n times

binary approach:
-we drop the egg at an arbitrary floor value (n stories)
-if the egg breaks, we create a pivot at (n stories)/2, ignoring the upper half of the pivot.
-if the egg doesn't break, we ignore the bottom half of the pivot.
-we will run the test drop with those conditions until we find floor _f_ where the egg breaks
time complexity will be O(log n)