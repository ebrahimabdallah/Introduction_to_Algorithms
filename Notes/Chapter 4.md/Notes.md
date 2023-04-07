# chapter 4 introduction to algorhithms

* In this chapter, we turn to a new type of problem-solving method, which is the Divide and Conquer method, in which we divide large, complex problems into simpler and sub-problems that are easy to solve.

* Divide and Conquer is best suited for problems that can be divided into independent subproblems
 
* what is the difference bettween a dynamic programmind and Divide and Conquer . . ? 

 * Divide and Conquer is best suited for problems that can be divided into independent subproblems, while Dynamic Programming is best suited for problems that can be broken down into overlapping subproblems that can be solved independently and then combined to find the optimal solution.
 -----------

**Divide** the problem into a number of subproblems that are smaller instances of the same problem.

**Conquer** the subproblems by solving them recursively.

**Combine** the solutions to the subproblems into the solution for the original problem.

**The divide-and-conquer** paradigm is a problem-solving technique that involves breaking a problem down into smaller sub-problems that are easier to solve, solving each sub-problem **recursively**, and then combining the solutions to the sub-problems to obtain a solution to the original problem

* three methods for solving **recurrences**:-

1) substitution method.
2) recursion-tree method.  
3) master method. 

# The maximum-subarray
 problem is a problem in computer science that requires finding the largest sum of contiguous elements in an array of integers

* divide and conquer --> at every level the max subarray-sum is one of three: 
1) the max of the right  
2) the max of the left  
3) the max crossing right and left

* **disadvantage** of the divide-and-conquer algorithm for the maximum-subarray problem is that it may require a large amount of memory when working with very large arrays.

* Another potential disadvantage  of this algorithm is that it may not always provide the optimal solution
* **FIND-MAX-CROSSING-SUBARRAY and FIND-MAXIMUM-SUBARRAY** are two algorithms used in problems of finding the largest subarray within a larger array.

* FIND-MAXIMUM-SUBARRAY is used to find the largest subarray within a complete array
* FIND-MAX-CROSSING-SUBARRAY is used to find the largest subarray that extends across the middle of the array

* ***
* # Strassen’s algorithm 
* The algorithm works by dividing the input matrices into smaller submatrices, and then recursively computing the products of these submatrices
******
 # substitution method
 * solving two steps:
1. Guess the solution 
2. Use mathematical induction to find the constants and show that the solution works

* **The substitution** method relies on guessing the form of the solution __(Unfortunately, there is no general way to guess the correct solutions) __ which can be difficult in some cases.

- It cannot be used when there are multiple roots to the recurrence equation, or when the solution consists of different recurrences
****
# master method
* The master method is a technique for solving recurrence relations 
* T(n) = aT(n/b) + f(n)
- Find two important conditions __ (a >= 1, b > 1)

*  master method has three cases 
*****
# Tree
* Recursion-tree method: converts the recurrence into nodes whose values are the cost at the levels of the recurision
