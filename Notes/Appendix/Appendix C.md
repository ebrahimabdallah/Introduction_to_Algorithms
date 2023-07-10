* This appendix reviews elementary combinatorics and probability theory

* Counting theory tries to answer the question **(How many)** without actually enumerating all the choices.

* The rule of sum says that the number of ways to choose one element from one
of two disjoint sets is the sum of the cardinalities of the sets.

--> if A = {1, 2, 3} and B = {4, 5}, then the number of ways to choose one element from either A or B

* the Rule of Product to determine the total number of possible outcomes by multiplying the number of choices at each step.

* A string over a finite set S is a sequence of zero or more elements of S

-->A string of length k is sometimes called a k-string.

-->A string is a sequence of zero or more characters from some finite set 

-->A substring s0 of a string s
is an ordered sequence of consecutive elements of s

-->A k-substring of a string
is a substring of length k


* **permutation** 
- is an ordered arrangement of the elements of S, where each element appears exactly once.

- for example:-

- S = {1, 2, 3}==>(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)

- number of permutations of a set S of size n is n!, which is the product of all positive integers up to n. This follows from the Rule of Product, 

- The number of k-permutations of an n-set is


- k-permuation from string of length S==> n*(n-1)*(n-2)...(n-k+1) = n!/(n-k)! = nPk

* **Combinations**
- an n-set S is simply a k-subset of S
- The order of the elements in a k-combination does not matter, and each element can only appear once in a given combination

- S = {1, 2, 3, 4} and k = 2, then the 2-combinations of S are ==>
{1, 2}, {1, 3}, {1, 4}, {2, 3}, {2, 4}, {3, 4}

- the total number of k-combinations of an n-set S can be computed using the binomial coefficient
- n choose k = n! / (k! * (n-k)!)

* **Binomial coefficients**
- read "n choose k"
- A special case of the binomial expansion occurs when x = y = 1 :2^n = summation of nCk from 0 to n

* **A probability** distribution Pr on a sample space S is a mapping from events of S to real numbers, which satisfies the following probability axioms:

1- Non-negativity: For any event E in S, Pr(E) is a non-negative real number, i.e., Pr(E) ≥ 0

2- Normalization: The probability of the entire sample space S is 1, i.e., Pr(S) = 1

3- Additivity: For any finite or countable sequence of pairwise disjoint events E1, E2, E3, ..., the probability of their union is equal to the sum of their individual probabilities

* A probability distribution is discrete if it is defined over a finite or countably infinite
sample space

* **Bayes's theorem** is a fundamental concept in probability theory that describes the relationship between conditional probabilities

- P(A|B) = P(B|A) * P(A) / P(B)
