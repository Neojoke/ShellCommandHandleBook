# BNF范式（巴科斯范式）

###### \(BNF: Backus-Naur Form 的缩写\)

巴科斯范式是用于描述计算机语言语法的符号集。shell命令行经常使用的man手册，SYNOPSIS主要使用该范式来描述语法和用法。

不仅如此，由于UNIX的巨大成功以及以后的影响力，BNF范式广泛应用于编程语言领域，几乎大部分的编程语法手册都默认以BNF范式为标准，辅助语法描述的符号以BNF范式为标准，对于初学者而言，阅读编程手册首先要了解的是要学习描述语法的符号是什么，才能够明白语法规则。

```
SYNOPSIS
     grep [-abcdDEFGHhIiJLlmnOopqRSsUVvwxZ] [-A num] [-B num] [-C[num]] [-e pattern] [-f file] [--binary-files=value]
          [--color[=when]] [--colour[=when]] [--context[=num]] [--label] [--line-buffered] [--null] [pattern]
          [file ...]
```

### 范式内容：

* 在双引号中的字\("word"\)代表着这些字符本身。而double\_quote用来代表双引号。
* 在双引号外的字（有可能有下划线）代表着语法部分。
* 尖括号\( &lt;&gt; \)内包含的为必选项。
* 方括号\( \[ \] \)内包含的为可选项。
* 大括号\( { } \)内包含的为可重复0至无数次的项。
* 竖线\( \| \)表示在其左右两边任选一项，相当于"OR"的意思。
* ::= 是“被定义为”的意思。



