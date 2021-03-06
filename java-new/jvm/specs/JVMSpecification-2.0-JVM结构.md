# JVMSpecification-2.0-JVM结构


> 要正确实现Java虚拟机，您仅需要能够读取class文件格式并正确执行其中指定的操作。不是Java虚拟机规范的一部分的实现细节将不必要地限制实现者的创造力。例如，运行时数据区域的内存布局，使用的垃圾收集算法以及Java虚拟机指令的任何内部优化（例如，将它们转换为机器代码）都由实现者自行决定。

## 2.1 class file format

## 2.2 数据类型

> 像Java编程语言一样，Java虚拟机可对两种类型进行操作：原始类型 和引用类型。相应地，可以将两种类型的值存储在变量中，作为参数传递，由方法返回并对其进行操作：原始值和参考值。

> Java虚拟机希望几乎所有类型检查都在运行时之前完成，通常由编译器完成，而不必由Java虚拟机本身完成。基本类型的值不需要被标记或无需检查即可在运行时确定其类型，或与引用类型的值区分开。相反，Java虚拟机的指令集使用旨在对特定类型的值进行运算的指令来区分其操作数类型。例如，iadd，ladd，fadd和 dadd都是Java虚拟机指令添加两个数值，并产生数值结果，这些指令分别针对不同的操作数类型： int，long，float，和double。有关Java虚拟机指令集中的类型支持的摘要，请参见 §2.11.1。

> Java虚拟机包含对对象的显式支持。对象可以是动态分配的类实例，也可以是数组。对对象的引用被认为具有Java虚拟机类型reference。类型的值reference可以认为是指向对象的指针。可能存在对一个对象的多个引用。对象始终通过reference的值进行操作，传递和测试 







