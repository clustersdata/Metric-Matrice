# Metric-Matrice
Metric Matrice
描述
Given as input a square distance matrix, where a[i][j] is the distance between point i and point j, determine if the distance matrix is "a  metric" or not.

A distance matrix a[i][j] is a metric if and only if

    1.  a[i][i] = 0

    2, a[i][j]> 0  if i != j

    3.  a[i][j] = a[j][i]

    4.  a[i][j] + a[j][k] >= a[i][k]  i ¹ j ¹ k

输入
The first line of input gives a single integer, 1 ≤ N ≤ 5, the number of test cases. Then follow, for each test case,
* Line 1: One integer, N, the rows and number of columns, 2 <= N <= 30
* Line 2..N+1: N lines, each with N space-separated integers 
(-32000 <=each integer <= 32000).
输出
Output for each test case , a single line with a single digit, which is the lowest digit of the possible facts on this list:
* 0: The matrix is a metric
* 1: The matrix is not a metric, it violates rule 1 above
* 2: The matrix is not a metric, it violates rule 2 above
* 3: The matrix is not a metric, it violates rule 3 above
* 4: The matrix is not a metric, it violates rule 4 above
样例输入
2
4
0 1 2 3
1 0 1 2
2 1 0 1
3 2 1 0
2
0 3
2 0
样例输出
0
3
