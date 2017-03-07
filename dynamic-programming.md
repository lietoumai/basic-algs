# Dynamic Programming - 动态规划算法

**核心思想**：动态规划（DP，Dynamic Programming）是算法设计方法之一，其本质是对问题**状态的定义**和**状态转移方程的定义**。动态规划是通过**拆分问题**，定义问题状态和状态之间的关系，使得问题能够以**递推**（或者说分治）的方式去解决。因此，如何拆分问题是动态规划的核心。

摘自[维基百科](https://en.wikipedia.org/wiki/Dynamic_programming)：
> **Dynamic programming** (also known as dynamic optimization) is a method for solving a complex problem by **breaking it down into a collection of simpler subproblems**, solving each of those subproblems just once, and storing their solutions – ideally, using a memory-based data structure. 

## 概念介绍

1. 什么是状态的定义？

 重新抽象问题，描述问题的状态。

2. 什么是状态转移方程？
 
 上述状态定义好之后，状态和状态之间的关系式，就叫做**状态转移方程**，即是带有条件的递推式。
 
## 适用情况

- **最优子结构**性质。如果问题的最优解所包含的子问题的解也是最优的，我们就称该问题具有最优子结构性质（即满足最优化原理）。最优子结构性质为动态规划算法解决问题提供了重要线索。
- **无后效性**。即子问题的解一旦确定，就不再改变，不受在这之后、包含它的更大的问题的求解决策影响。
- **子问题重叠**性质。子问题重叠性质是指在用递归算法自顶向下对问题进行求解时，每次产生的子问题并不总是新问题，有些子问题会被重复计算多次。动态规划算法正是利用了这种子问题的重叠性质，对每一个子问题只计算一次，然后将其计算结果保存在一个表格中，当再次需要计算已经计算过的子问题时，只是在表格中简单地查看一下结果，从而获得较高的效率。


## Reference

1. [Dynamic programming - From Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Dynamic_programming)