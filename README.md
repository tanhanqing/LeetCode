# LeetCode

解决LeetCode问题记录

总结自 leetcode题库分门别类详细解析

[这里有LeetCode全解法](https://github.com/liuyubobobo/Play-Leetcode)


## 前言

算法有多种渠道-排序而言

大量重复数据 - 三路快排

近乎有序数据 - 插入排序

取值范围有限数据 - 计数排序

稳定的排序 - 归并排序

链表的排序 - 归并排序

不足以加载到内存中 - 外部排序

## 时间复杂度 O（n）

最好使用 nlogn 甚至更小的 时间复杂度，因为这类方法在数据规模非常大时的效率非常高 ，迫不得已才使用n2级别的算法

二分查找  O（logn）

查询最大最小 O(n)

归并排序 (nlogn)

选择排序 （n2)

## 数据规模

一般来说算法都需要在1s内解决问题，所以问题的时间复杂度决定了解决的速度

仅仅计算加法 10^9  ->  4s  时间

10^8 -> 0.4s 
           
            即O（n）级别的算法可以处理10^8 数据量

            O(nlogn)级别算法可以处理10^7 数据量

            O(n2) 级别 可以处理10^4 数据量
