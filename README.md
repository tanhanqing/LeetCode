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
            

## 杂

log a N = log a b * log b N  =  k log b N  所以底不重要

在递归函数中   考虑 时间复杂度 + 空间复杂度 （递归深度问题）

[l ... r]求中点 为了避免整形溢出  l+(r - l)/2

## 数组基本问题

[27移除元素](https://leetcode-cn.com/problems/remove-element) 

           说明:
           为什么返回数值是整数，但输出的答案是数组呢?
           请注意，输入数组是以“引用”方式传递的，这意味着在函数里修改输入数组对于调用者是可见的。
           你可以想象内部操作如下:
           // nums 是以“引用”方式传递的。也就是说，不对实参作任何拷贝
           int len = removeElement(nums, val);
           // 在函数里修改输入数组对于调用者是可见的。
           // 根据你的函数返回的长度, 它会打印出数组中该长度范围内的所有元素。
           for (int i = 0; i < len; i++) {
               print(nums[i]);
           }
           [java传值还是传引用](https://www.cnblogs.com/chen-kh/p/6696303.html)
           所以这里，我们把这种传递也理解为”值传递“只不过这里的值，是一个”引用”的值！也就是我们把实际参数（一个引用）拷贝一份赋值给形式参数，形式参数进行操作。当形式参数对本身的对象进行了变动操作，这里的效果跟引用传递是相同的。但是一旦给形式参数进行赋值类型的操作，这个赋值操作并不会像C语言的引用那样，把这个赋值的效果反映在函数运行结束之后！！
           

[88合并两个有序数组](https://leetcode-cn.com/problems/merge-sorted-array)

[215数组中的第K个最大元素](https://leetcode-cn.com/problems/kth-largest-element-in-an-array) 

[167两数之和 II - 输入有序数组](https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted)


## 对撞指针问题

[125验证回文串](https://leetcode-cn.com/problems/valid-palindrome)

           方法：      Character.isLetterOrDigit(cha[i]) 可以判定是不是数字或字母 
                      Character.toLowerCase(cha[i])  可以将字符转为小写
           注意： 为了防止单数字符串 我采用了
                      if(l == r - 2 || l == r - 1){
                           if(arr[l] == arr[r]){
                               return true ;
                           }else{
                               return false;
                           }
                       }
                  其实考虑清楚可以发现，因为比对完成后 ，会i++ ,同时j-- ，意味着会同时指向字符串中心，已经避免了单数字符串，所以上面的方法是多余的

[344反转字符串](https://leetcode-cn.com/problems/reverse-string)

[11盛最多水的容器](https://leetcode-cn.com/problems/two-sum)

[345反转字符串中的元音字母](https://leetcode-cn.com/problems/reverse-vowels-of-a-string)


## 滑动窗口问题

[3无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters)

[209长度最小的子数组](https://leetcode-cn.com/problems/minimum-size-subarray-sum/description/)

[438找到字符串中所有字母异位词](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string/description/)

[76最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring/description/)

## set，map数据结构使用

[350两个数组的交集 II](https://leetcode-cn.com/problems/intersection-of-two-arrays-ii/description/)



## 查找表

[454四数相加2](https://leetcode-cn.com/problems/4sum-ii)

[49. 字母异位词分组](https://leetcode-cn.com/problems/group-anagrams/description/)

[447. 回旋镖的数量](https://leetcode-cn.com/problems/number-of-boomerangs/description/)

[149. 直线上最多的点数](https://leetcode-cn.com/problems/max-points-on-a-line/description/)























