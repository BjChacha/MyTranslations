# 一、Pythonic思维

## 前言

多年来，Python社区用`Pythonic`一词来形容"编程语言的习惯由用户来定义"这种代码风格。`Pythonic`不是为了面向编译器，而是为协同合作。Python的代码会更偏向于显式、简单和高可读性。

用过其他语言（比如C++,Java）的程序员可能会将之前的习惯带到Python里。而新手则会舒服很多，因为Python中大量概念都是非常直观易懂。对于每个人来说，将Python写得`Pythonic`非常重要。这种习惯会影响以后写的每道程序。

## 1. 查看使用Python的版本

> $ python --version  
> Python 3.7.4

```python
import sys
print(sys.version_info)
# sys.version_info(major=3, minor=7, micro=4, releaselevel='final', serial=0)
print(sys.version)
# 3.7.4 (default, Aug  9 2019, 18:34:13) [MSC v.1915 64 bit (AMD64)]
```

## 要记住

1. 目前主要使用两个版本：Python 2和Python 3。

2. 几个知名的Python运行平台：CPython，Jython，IronPython，PyPy等等。

3. 确认命令行运行Python的版本是否符合预期。

4. 最好使用Python 3，因为这是目前Python社区的主要关注对象。
