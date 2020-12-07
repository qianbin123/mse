> 复习资料

`抽象数据类型（Abstract Data Type，ADT）`

> 抽象数据类型可以用以下的三元组来表示：

```c

// ADT抽象数据类型名{
//     数据对象：<数据对象的定义>
//     数据关系：<数据关系的定义>
//     基本操作：<基本操作的定义>
// } ADT抽象数据类型名

```

```c

// ADT List{
//   数据对象：D={ai|ai∈Elemset, i=1,2,…,n, n≥0}
//   数据关系：R={<ai−1,ai>|ai−1,ai∈D, i=2,…,n}
//   基本操作：
//   InitList(&L)
//       操作结果：构造一个空的线性表 L
//   DestroyList(&L)
//       初始条件：线性表已存在
//       操作结果：销毁线性表L
//   ClearList(&L)
//       初始条件：线性表已存在
//       操作结果：置线性表L为空表
//   ListEmpty(L)
//       初始条件：线性表已存在
//         操作结果：若线性表L为空表，则返回TRUE，否则返FALSE
//   ListLenght(L)
//       初始条件：线性表已存在
//       操作结果：返回线性表L数据元素个数
//   GetElem(L, i, &e)
//       初始条件：线性表已存在（1≥i≥ListLenght(L)）
//       操作结果：用e返回线性表L中第i个数据元素的值
//   locatElem(L, e, comare())
//       初始条件：线性表已存在，comare()是数据元素判定函数
//         操作结果：返回线性表L中第1个与e满足关系comare()数据元素的位序
//   PriorElem(L, cur_e, &pre_e)
//       初始条件：线性表已存在
//         操作结果：若cur_e是线性表L的数据元素，且不是第一个，则用pre_e返回它的前驱，否则操作失败，pre_e无义
//   NextElem(L, cur_e, &next_e)
//       初始条件：线性表已存在
//         操作结果：若cur_e是线性表L的数据元素，且不是第最后一个，则用next_e返回它的后继，否则操作失败，next_无定义
//   ListInsert(&L, i, e)
//       初始条件：线性表已存在（1≥i≥ListLenght(L)+1）
//         操作结果：在线性表L中第i个数据元素之前插入新元素e，长度加1
//   ListDelete(&L, i, &e)
//       初始条件：线性表已存在（1≥i≥ListLenght(L)）
//         操作结果：删除线性表L中第i个数据元素，用e返回其值，长度减1
//   ListTraverse(L, visit())
//       初始条件：线性表已存在
//         操作结果：依次对线性表L的每个数据元素调用visit()数，一旦visit()失败，则操作失败
// }ADT List

```
