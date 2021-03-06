There are `N` dominoes in a line, and we place each domino vertically upright.

In the beginning, we simultaneously push some of the dominoes either to the left or to the right.

![img](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/05/18/domino.png)

After each second, each domino that is falling to the left pushes the adjacent domino on the left.

Similarly, the dominoes falling to the right push their adjacent dominoes standing on the right.

When a vertical domino has dominoes falling on it from both sides, it stays still due to the balance of the forces.

For the purposes of this question, we will consider that a falling domino expends no additional force to a falling or already fallen domino.

Given a string "S" representing the initial state. `S[i] = 'L'`, if the i-th domino has been pushed to the left; `S[i] = 'R'`, if the i-th domino has been pushed to the right; `S[i] = '.'`, if the `i`-th domino has not been pushed.

Return a string representing the final state. 

**Example 1:**

<pre>
<b>Input:</b> ".L.R...LR..L.."
<b>Output:</b> "LL.RR.LLRRLL.."
</pre>

**Example 2:**

<pre>
<b>Input:</b> "RR.L"
<b>Output:</b> "RR.L"
<b>Explanation:</b> The first domino expends no additional force on the second domino.
</pre>

**Note:**

1. `0 <= N <= 10^5`
2. String `dominoes` contains only `'L`', `'R'` and `'.'`

### [Editorial](https://leetcode.com/articles/push-dominoes/)
