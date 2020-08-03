### 题意
给出$N$个数组，定义每两个数组之间的相似度为$N_c/N_t \times 100\%$，其中$N_c$为两个数组交集元素的个数，$N_t$为两个数组并集中的元素个数

### 思路
使用set维护每个数组，对任意一个询问来说，merge两个set，过程之中维护记录$N_c$和$N_t$即可