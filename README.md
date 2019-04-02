# 编译原理实验课代码

## Lexer

对Pascal源程序进行词法分析的词法分析器。

**内部码对照表**

| 内码 | 单词       | 内码 | 单词      | 内码 | 单词 | 内码 | 单词    |
| ---- | ---------- | ---- | --------- | ---- | ---- | ---- | ------- |
| 1    | PROGRAM    | 2    | CONST     | 3    | VAR  | 4    | INTEGER |
| 5    | LONG       | 6    | PROCEDURE | 7    | IF   | 8    | THEN    |
| 9    | WHILE      | 10   | DO        | 11   | READ | 12   | WRITE   |
| 13   | BEGIN      | 14   | END       | 15   | ODD  | 16   | +       |
| 17   | -          | 18   | *         | 19   | /    | 20   | =       |
| 21   | <>         | 22   | <         | 23   | <=   | 24   | >       |
| 25   | >=         | 26   | ,         | 27   | .    | 28   | ;       |
| 29   | :          | 30   | :=        | 31   | (    | 32   | )       |
| 33   | 无符号整数 | 34   | 标识符    | 35   | #    |      |         |

**代码实现流程图**

![代码实现流程图](https://fries-image.oss-cn-hangzhou.aliyuncs.com/github/lexer_process.png)