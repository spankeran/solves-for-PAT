### 题意
如果两个$10$进制数的数位和相等则称其为$friend$ $number$，数位和被称为$friend's$ $ID$，求$N$个数中所有不同的$friend's$ $ID$

### 思路
本质就是将$N$个数的$10$进制数位相加，求去重后的数位和，用set维护即可