# 高效Python：写好Python的59种方式

[原文](https://github.com/SigmaQuan/Better-Python-59-Ways)

## 目录

1. Pythonic思维
    1. 查看使用`Python`的版本
    2. 遵循`PEP 8`规范指南
    3. `byte`, `str`和`unicode`的区别
    4. 写helper函数
    5. 切片
    6. 不要用list[start:end:stride]
    7. 使用列表表达式来代替`map`函数和`filter`函数
    8. 不要在一个列表表达式中使用超过两条式子
    9. 使用`生成器`
    10. 用`enumarate`来代替`range`
    11. 用`zip`来并行处理`iterators`
    12. 不要在`for`和`while`循环和用`else`
    13. 活用`try`/`except`/`else`/`finally`
2. 函数
    14.  用`exception`来返回`None`
    15.  了解`闭包`如何作用于变量作用域
    16.  返回`生成器`而不是`列表`
    17.  # FIXME 迭代参数要谨慎
    18.  # FIXME 用位置参数变量来减少可视化噪声
    19.  使用关键字参数来提供可选项
    20.  # FIXME 用`None`和`Docstrings`来指定动态默认参数
    21.  # FIXME 强制声明关键字参数
3.   类与继承
    22.  # FIXME 通过字典和元组使用helper类
    23. #TODO Use @classmethod polymorphism to construct objects generically
    24. # FIXME 使用`@classmethod`来修饰结构对象
    25. 用`super`初始父类
    26. # FIXME 仅在`mix-in utility`类中使用多重继承
    27. 用`public`属性代替`private`
    28. # FIXME 从`collections.abc`中继承
4.  元类和属性
    29. 直接用`属性`而不是`get`和`set`
    30. 考虑用`@property`而不是重构属性
    31. # FIXME 用`descriptor`来复用`@property`方法
    32. 使用`getattr`, `getattribute`和`setattr`
    33. 用`元类`来验证子类
    34. # FIXME 用`元类`来注册类存在
    35. 用`元类`来注释类属性
5.  递归于并行
    36. 用`subprocess`来管理子进程
    37. 用`线程`来阻塞I/O
    38. # FIXME 使用锁来避免数据冲突
    39. 用队列来协同线程协同
    40. 考虑用协程来并发运行多函数
    41. 考虑`concurrent.futures`来实现真并行
6.  内置模组
    42. 用`functools.wraps`定义函数修饰器
    43. # FIXME 考虑用`contextlib`和statements用于复用`try`/`finally`行为
    44. #TODO Make pickle reliable with copyreg
    45. 用`datetime`来代替`time`
    46. 使用内置算法和数据结构
    47. #TODO Use decimal when precision ia paramount
    48. # FIXME 知道哪里去找建立模组的社区
7.  协作
    49. 给每个函数、类、模组写`docstrings`
    50. 用包来组织模组和提供稳定API
    51. #TODO Define a root exception to insulate callers from APIs
    52. #TODO Know how to break circular dependencies
    53. 用`虚拟环境`来隔离和重用依赖项
8.  生产
    54. # TODO Consider module-scoped code to configure deployment environments
    55. 用`repr`字符串来调试输出
    56. `单元测试`
    57. 用`pdb`实现交互调试
    58. # TODO Profile before optimizing
    59. 用`tracemalloc`来理解内存使用和泄漏