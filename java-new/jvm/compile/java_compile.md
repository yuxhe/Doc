# JAVA 编译器

## 概述

在JAVA中的编译, 主要分为三种类型

1. `.java`编译成`.class`,我们称它为 前端编译器, 我们使用的`javac`就是一个前端编译器
2. `.class`编译成本地机器码, 一般用在运行时即时编译, 常说的JIT就是这个意思. Hotspot中的C1,C2 编译器就属于这种.
3. `.java`直接编译成本地机器码, 我们有时会在文献中看到 AOT 编译器(Ahead of Time Compiler)就是这个意思. 就像GO语言中`.go`文件直接编译成本地机器码一样.








