### 题意
有两种排序方法：插入排序和归并排序，给定原序列和在某种策略下已经进行几步操作的序列，求运用的是何种策略，并输出在该种策略下再进行一步操作的结果

### 思路
首先是如何判断是那种排序，我的思路是从初始元素开始找到不满足升序的第一个元素，然后从这个元素开始与初始数组比较，一旦出现不相同的情况就是归并排序，反之则是插入排序。判断出是何种排序之后，只需要按照各自的原理再模拟一步即可

但这个题是有歧义的，比如说下面这个例子：

```
6
2 1 6 5 4 3
1 2 5 6 3 4
```

你输出`1 2 5 6 3 4`或者`1 2 3 4 5 6`都是可以说通的，但根据我的观察，$PAT$要的是前一种，所以我的代码过不去最后一个测试点。。。我也不想再改了，这题是有问题的。。。