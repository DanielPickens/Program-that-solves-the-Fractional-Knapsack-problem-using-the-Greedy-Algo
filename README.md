# Program-that-solves-the-Fractional-Knapsack-problem-using-the-Greedy-Algo
Greedy algo method used to solve the Knapsack fractional algorithm



Problem Description

In the fractional knapsack problem, we are given a set of n items. Each item i has a value v(i) and a weight w(i) where 0 <= i < n. 

We are given a maximum weight W. 
The problem asked me  to find how much of each item we should take such that the total weight does not exceed W and the total value is maximized. Thus, we want to find f ( our variable measuring the fractional notation) such that sum of v(i)f(i) over all i is maximized, w(i)f(i) <= W for all i and 0 <= f(i) <= 1 for all i.

Problem Solution
1. The function fractional_knapsack is defined.
2. It takes three arguments: two lists value and weight; and a number capacity.
3. It returns (max_value, fractions) where max_value is the maximum value of items with total weight not more than capacity.
4. fractions is a list where fractions[i] is the fraction that should be taken of item i, where 0 <= i < total number of items.
5. The function works by choosing an item from the remaining items that has the maximum value to weight ratio.
6. If the knapsack can include the entire weight of the item, then the full amount of the item is added to the knapsack.
7. If not, then only a fraction of this item is added such that the knapsack becomes full.
8. The above three steps are repeated until the knapsack becomes full, i.e. the total weight reaches the maximum weight.


RUNTIME TES CASES: 
ase 3:
Enter number of items: 1
Enter the values of the 1 item(s) in order: 5
Enter the positive weights of the 1 item(s) in order: 10
Enter maximum weight: 5
The maximum value of items that can be carried: 2.5
The fractions in which the items should be taken: [0.5]
