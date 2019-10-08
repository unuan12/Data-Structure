### 1. 树、二叉树和二叉查找树
树由节点与弧组成，树的递归定义：

1.1. 空结构是一颗空树；

1.2. 如果$t_1,...,t_k$是不相交的树，那么，以$t_1,...,t_k$的根作为子节点的数据结构也是一棵树；

1.3. 只有通过第1步和第2步产生的数据结构才是树。

每个节点都可以从根节点经一个唯一的弧序列到达，此弧序列被称为**路径**，**路径中弧的数量称为路径的长度**。

节点的**层次**是从根节点到该节点的路径的长度加$1$，也就是该路径上节点的数量。

如果除最后一个层次外，其他层次上的所有节点都有两个子节点，那么，第一层有$1=2^0$个节点，第二层有$2 = 2^1$个节点，第三层有$4 = 2^2$个节点，一般地，第$i+1$层有$2^i$个节点。满足条件的树称为完全二叉树(complete binary tree)。

对于非空二叉树来说，若其所有的非终端节点刚好有两个非空子节点，则叶节点的数目$m$大于非终端节点的数目$k$，并且$m = k+1$。

二叉查找树特性：对于树中的每个节点$n$，其左子树中的值小于节点$n$中的值$v$，其右子树的值大于节点$n$中的值$v$。