### 题意
有一个链表，每个节点包括`key`键值和`next`指针，要求输出按照`key`排序的结果

### 思路
有脏节点（不在链表中的节点），所以需要一个vector存储有效节点，只需从head开始遍历加入vector即可，然后对vector数组进行排序输出