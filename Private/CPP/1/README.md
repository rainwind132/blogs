# 预备知识

## C++ 简史

### C 语言

贝尔实验室需要一种语言用于开发 UNIX 系统，这种语言必须简洁，能够生成简洁、快速的程序，并能有效地控制硬件。

传统上，程序员使用汇编语言来满足这些需求，汇编语言依赖于计算机的内部机器语言。然而，汇编语言是低级（low-level）语言，即直接操作硬件，如直接访问 CPU 寄存器和内存单元。因此汇编语言针对于特定的计算机处理器，要将汇编程序移植到另一种计算机上，必须使用不同的汇编语言重新编写程序。

UNIX 是为在不同的计算机（或平台）上工作而设计的，这意味着它是一种高级语言。高级（high-level）语言致力于解决问题，而不针对特定的硬件。一种被称为 `编译器` 的特殊程序将高级语言翻译成特定计算机的内部语言。这样，就可以通过对每个平台使用不同的编译器来在不同的平台上使用一个高级语言程序了。于是，C 语言诞生了。

### C++

C++ 是 C 语言的超集，这意味着任何有效的 C 程序都是有效的 C++ 程序。

### 本书遵循的 C++ 标准

当代的编译器都对 C++98 提供了很好的支持，本书详尽的介绍了 C++98，并涵盖了 C++11 新增的一些特性。


## 程序创建的技巧

运行 C++ 程序的步骤：

  1. 编写程序的源代码。
  2. 编译源代码，将源代码翻译为主机使用的内部语言 —— 机器语言。
  3. 将目标代码与其他代码链接起来，链接指的是将目标代码同使用的函数（如其他库）的目标代码以及标准的启动代码（startup code）组合起来，生成程序的运行阶段版本。包含该最终产品的文件被称为可执行代码。

![image](http://shadows-mall.oss-cn-shenzhen.aliyuncs.com/images/assets/cpp/1.png)


源代码文件的扩展名（如下图）：

![image](http://shadows-mall.oss-cn-shenzhen.aliyuncs.com/images/assets/cpp/2.png)


## 总结

随着计算机的功能越来越强大，计算机程序越来越庞大而复杂。为应对这种挑战，计算机语言也得到了改进，以便编程过程更加简单。C 语言新增了诸如控制结构和函数等特性，以便更好的控制程序流程，支持结构化和模块化程度更高的方法；而 C++ 增加了对面向对象编程和泛型编程的支持，这有助于提高模块化和创建可重用代码，从而节省编程时间并提高程序的可靠性。

C++ 的流行导致大量用于各种计算平台的 C++ 实现得以面世；而 IOS C++ 标准（C++98/03 和 C++11）为确保众多实现的相互兼容提供了基础。这些标准规定了语言必须具备的特性、语言呈现出的行为、标准库函数、类和模板，旨在实现该语言在不同计算平台和实现之间的可移植性。

要创建 C++ 程序，可创建一个或多个源代码文件，其中包含了以 C++ 语言表示的程序。这些文件是文本文件，它们经过编译和链接后将得到机器语言文件，后者构成了可执行的程序。上述任务通常是在 IDE 中完成的，IDE 提供了用于创建源代码文件的文本编辑器、用于生成可执行文件的编译器和链接器以及其他资源，如项目管理和调试功能。然而，这些任务也可以在命令行环境中通过合适的工具来完成。
