# 力扣每日一题 0115 不同的子序列


[题目链接](https://leetcode-cn.com/problems/distinct-subsequences/)

<!--more-->

读题，易知：

1. 若 t 是 s 的子序列，则 m（s 的长度）大于等于 n（t 的长度），即当 m 小于 n 时直接返回 0。
2. 在 m 大于等于 n 的条件下，用 dp[i][j] 来表示 s[i:] 的子序列中 t[j:] 的个数。
3. 首先考虑边界情况：
    1. 当 j = n 时，t[j:] 为空串，由于空串是任何字符串的子串，因此，对任意$0 \le i \le m$
