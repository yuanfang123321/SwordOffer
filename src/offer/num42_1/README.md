# 左旋转字符串

**题目**


汇编语言中有一种移位指令叫做循环左移（ROL），现在有个简单的任务，就是用字符串模拟这个指令的运算结果。
对于一个给定的字符序列S，请你把其循环左移K位后的序列输出。
例如，字符序列S=”abcXYZdef”,要求输出循环左移3位后的结果，即“XYZdefabc”。是不是很简单？OK，搞定它！

**测试地址**
[左旋转字符串](https://www.nowcoder.com/practice/12d959b108cb42b1ab72cef4d36af5ec?tpId=13&tqId=11196&tPage=3&rp=3&ru=/ta/coding-interviews&qru=/ta/coding-interviews/question-ranking)

## 解题思路

时间复杂度o(N)
这道题解题的思路在于我们将字符串分成2部分，前一部分n位，后一部分是剩下的部分。
分别对这两部分进行翻转，然后在对整体翻转，就是结果