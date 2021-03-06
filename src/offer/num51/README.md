## 数组中重复的数字

**题目**

在一个长度为n的数组里的所有数字都在0到n-1的范围内。 数组中某些数字是重复的，但不知道有几个数字是重复的。也不知道每个数字重复几次。
请找出数组中任意一个重复的数字。
 例如，如果输入长度为7的数组{2,3,1,0,2,5,3}，那么对应的输出是第一个重复的数字2
 
**测试地址**
[数组中重复的数字](https://www.nowcoder.com/practice/623a5ac0ea5b4e5f95552655361ae0a8?tpId=13&tqId=11203&tPage=3&rp=3&ru=/ta/coding-interviews&qru=/ta/coding-interviews/question-ranking)

## 解题思路

这道题，如果采用排序的方式，比较相邻的元素是可以出结果的，时间复杂度是o(lgN)
如果采用HashMap的形式，时间复杂度与空间复杂度都是o(N)

因为这道题给出的元素都是在0 到N- 1之间，于是有时间复杂度为o(N),空间复杂度是o(1)的算法

如果数组是有序的，那么第i的位置的元素一定是i ,所以先判断第i的位置的元素是不是i，如果是，则继续判断i + 1的元素。
如果不是，则该数字为m，则判断numbers[m]与number[i]是否相等，如果不相等，则交换两者的顺序.
使得第m的位置，数字是m。然后继续比较Number[i]与i是不是相等。也就是回到了第一步。