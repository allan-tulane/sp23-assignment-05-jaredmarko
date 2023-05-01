# CMPS 2200 Assignment 5
## Answers

**Name:** Jared Markowitz


Place all written answers from `assignment-05.md` here for easier grading.





- **1a.**

1. Sort the coins in decreasing order of value
2. Start with the largest coin and use as many of them as needed to make up the remainder of N.
3. Repeat step 2 with the next largest coin, and so on, until N is reached.

This algorithm is optimal because it always produces the minimum number of coins possible. This can be proven by induction. The base case is when N is 0. In this case, no coins are needed. The inductive step is when N is greater than 0. In this case, we can use the greedy algorithm to produce a set of coins that sum to N-1. By the induction hypothesis, this set of coins is optimal. We can then add one more coin of the largest denomination to this set, and this will still be an optimal solution. Therefore, the greedy algorithm is always optimal for producing as few coins as possible that sum to N dollars.

- **1b.**

The work of the algorithm is O(log n), where n is the number of coins. This is because the algorithm sorts the coins in decreasing order of value, which takes O(log n) time. The span of the algorithm is also O(log n), because the algorithm only needs to make one pass over the sorted list of coins.


- **2a.**


One counterexample is the denominations = {1,4,6,8} and N = 10 where the greedy algorithms uses 8, 1, and 1 to get N = 10. The minimum number of coins the greedy algorithms would return would be 3 coins. The actual minimum number of coins is not 3, but 2 as N = 10 could have been made with 4 and 6. Therefore, the greedy algorithm cannot work optimally.



- **2b.**


The work of this algorithm is O(n*m), where n is the number of coins and m is the amount of money. This is because the algorithm needs to create a table of size nm, and it needs to iterate over the table once for each coin.

The span of this algorithm is O(n), where n is the number of coins. This is because the algorithm only needs to make one pass over the table.






