# 2. 遵循PEP 8规范指南

## 空格

空格在Python语法中非常重要。Python程序员深知空格对于代码清晰度的影响。

1. 缩进用`spaces`不用`tabs`。（现在编辑器普遍支持tab自动转化为space）
2. 每级缩进用4个`spaces`。
3. 每行长度至多79个字符。
4. 较长的条件表达式分行时也要缩进4个`spaces`。
5. 在文件中，函数和类之间相隔2行。
6. 在类中，方法之间相隔1行。
7. 不要在列表索引、函数调用、关键字传参中使用空格。
8. 变量前后有且仅有1个`space`。

## 命名

PEP 8推崇一种独特的命名方式，以区别其他语言。

1. 函数、变量和属性应该用`lowercase_underscore`格式。
2. 保护性属性应该用单下划线`_leading_underscore`格式。
3. 私有属性应该用双下划线`__double_leading_underscore`格式。
4. 类和#TODO exceptions应该用大写开头`CapitalizedWord`格式。
5. 模组级常量应该用全大写`ALL_CAPS`格式。
6. #FIXME 类方法应该用`self`作为第一个参数

## 表达式与语句

Python禅宗之道：最好有且只有一种方式去实现一个功能。

1. 用内联否定（if a is not b）而不是# FIXME 肯定的否定（if not a is b）。
2. 不要用`length`（if len(somelist) == 0）来判断空值（比如`[]`或`''`）。用`if not somelist`，假定空值是`False`（注意这里并不等价）。
3. 同样地，可以假定非空值是`True`。
4. 避免用单行来写`if`，`for`，`while`和`except`表达式。将其展开成多行会更加清晰。
5. 永远把`import`写在文件开头。
6. `import`一个模组，要用# FIXME 绝对名称而不是相对名称。比如要`from bar import foo`而不是`import foo`。
7. 如果一定要相对`import`，请用`from . import foo`。
8. `import`需以以下顺序分区：标准库模组->第三方库模组->自己的模组。每区内按开头字母排序。

## 要记住

1. 永远遵循`PEP 8`代码风格去写Python代码。
2. 用同种代码风格有助于庞大的Python社区内协同合作。
3. 采用一致的风格会让你修改自己的代码更加轻松。