# 工作日志

## 五月

**5.5**

完成 mean 即平均值函数和相关测试。

检查到 Jason 的 sum 函数忘记对不规则矩阵情况的考虑。

但无论是 Jason 的 sum 还是我的 mean 函数都无法对 Tensor 结构进行操作，很奇怪。补充：事实上现阶段函数不考虑兼容 Tensor 结构，这是以后的事。

以后可以考虑添加功能，如果输入的第一个参数是矩阵，则可以增加第二个参数，作为 axis 参数，可以参考 numpy 或者 matlab。

写了一个 median 即中位数函数的草稿，本来想用 JS 自带的排序函数，但总觉得不对劲，它默认这个数组是排序好的：\[3, 34, 5\]，就离谱。

**5.6**

代码要求发生了变化，这次可能会长期固定了，修改所有代码。

完成 median 和 mean 函数的最终版本.

解决掉 Tensor 结构的不兼容问题。

**5.9**

写 log 函数，初稿完成，默认的是自然对数，但结果竟然是多维的。而且问题在于不能重载，不知道为什么，先起个 private_log 函数名凑合用。

log函数无限期暂停，重载和矩阵/向量除法设计有问题，需要修正。

完成 multinomial 函数，就是一些数字和的阶乘，除以每个数字的阶乘。剩下的函数恐怕就没有简单到一天搞定的了。

**5.10**

修改 multinomial 函数，这次有了新要求。

写 reshape 函数。

打算修改所有 math 库函数的报错信息，以适应最新要求，这个可能工程量有点大。

**5.11**

重构 math 函数

**5.12**

重构 math 函数

**5.13**

重构 math 函数，上次弄丢了不少东西，因为版本问题，重新写了一遍

**5.16**

重构 math 函数

**5.17**

终于重构完了所有 math 函数，明天写新的函数
