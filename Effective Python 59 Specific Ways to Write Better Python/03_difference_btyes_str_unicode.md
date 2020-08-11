# byte, str和unicode的区别

在Python 3，有两种表示字符的序列：`bytes`和`str`。`bytes`包含原生的8位二进制数，而`str`包含`Unicode`字符。

在Python 2，也有两种表示字符的序列：`str`和`unicode`。与Python 3相反，`str`包含8位二进制数，而`unicode`则包含`Unicode`字符。

有很多方式将`Unicode`字符表示为二进制数。最常见就是编码为`UTF-8`。注意，Python 3中的`str`跟Python 2中的`unicode`没有任何联系。要将`Unicode`字符转换成二进制，要用`encode`方法。同样地，要将二进制数据转换成`Unicode`字符，要用`decode`方法。

写Python的时候，将编码和解码写得离接口尽量远是非常重要的。就编码而言，程序应该只以`Unicode`为主而不再考虑其他。这会让你的代码对于文本具有包容性（比如`Latin-1`，`Shift`，`JIS`和`Big5`）的同时，还能严格规范输出文本的编码（最好是`UTF-8`）。

Python两种字符类型的分隔导致两种常见的情况：

1. 经`UTF-8`编码后：操作8位二进制值。
2. 未经任何编码：操作`Unicode`字符。

