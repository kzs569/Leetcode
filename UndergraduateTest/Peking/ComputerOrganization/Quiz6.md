Quiz 6 - Week 7
===============

1、(5分)处理器设计的五个步骤如下，请正确排序。

1	连接组件建立数据通路

2	为数据通路选择合适的组件

3	集成控制信号，形成完整的控制逻辑

4	分析指令系统，得出对数据通路的需求

5	分析每条指令的实现，以确定控制信号

**42153**

2、(5分)课程中提到的MIPS-lite指令子集（addu，subu，ori，lw，sw，beq）对ALU的需求有哪些？

 **A、 加法**

 **B、 减法**

 **C、 逻辑或**

 **D、 相等**

 E、 逻辑与

 F、 逻辑非

 G、 乘法

 H、 除法

 I、 左移

 J、 右移

3、(5分)下列关于MIPS-lite指令子集对数据通路的需求描述正确的是？

 **A、 add指令与ori指令对寄存器堆的写操作需求不一样**

 **B、 lw指令需要符号扩展部件**

 **C、 lw指令与sw指令都需要数据存储器**

 D、 add指令需要零扩展部件

 E、 sub指令需要符号扩展部件

 F、 ori指令需要符号扩展部件

4、(5分)下列关于运算指令的控制信号描述正确的是？

 **A、 add指令与ori指令的寄存器堆控制信号RegDst不同**

 **B、 add指令与ori指令的ALU源操作数控制信号ALUSrc不同**

 **C、 add指令与ori指令的ALU运算类型控制信号ALUctr不同**

 **D、 add指令的扩展部件控制信号ExtOp不唯一**

 E、 ori指令的扩展部件控制信号ExtOp不唯一

 F、 add指令与ori指令的数据存储器控制信号MemWr可以不相同

5、(5分)下列关于访存指令的控制信号描述正确的是？

 **A、 lw指令与sw指令的ALU运算类型控制信号ALUctr相同**

 **B、 lw指令与sw指令的控制信号MemtoReg可以不相同**

 C、 lw指令与sw指令的寄存器堆控制信号RegDst一定相同

 D、 lw指令与sw指令的扩展部件控制信号ExtOp可以不相同

 E、 lw指令与sw指令的数据存储器控制信号MemWr可以不相同

6、(5分)下列关于beq指令的执行描述正确的是？

 **A、 beq指令的寄存器堆控制信号RegDst是不唯一的**

 **B、 beq指令与lw指令的数据存储器控制信号MemWr是相同的**

 C、 beq指令与add指令的ALU运算类型控制信号ALUctr相同

 D、 beq指令的扩展部件控制信号ExtOp一定为sign

 E、 若ALU计算结果为零，则beq指令不需要执行PC+4操作

7、(5分)在单周期处理器上执行beq指令，使用到了下列哪些部件？

 **A、 寄存器堆**

 **B、 ALU**

 C、 扩展部件（零扩展或符号扩展）

 D、 数据存储器

8、(5分)在单周期处理器上执行add指令，使用到了下列哪些部件？

 **A、 寄存器堆**

 **B、 ALU**

 C、 扩展部件（零扩展或符号扩展）

 D、 数据存储器

9、(5分)在单周期处理器上执行ori指令，使用到了下列哪些部件？

 **A、 扩展部件（零扩展或符号扩展）**

 **B、 寄存器堆**

 **C、 ALU**

 D、 数据存储器

10、(5分)在单周期处理器上执行lw指令，使用到了下列哪些部件？

 **A、 扩展部件（零扩展或符号扩展）**

 **B、 数据存储器**

 **C、 寄存器堆**

 **D、 ALU**

11、(5分)假设单周期处理器五个阶段的延迟分别为200ps（取指）、50ps（读寄存器）、200ps（ALU操作）、300ps（访存）、100ps（写寄存器），则sw指令的总延迟为多少ps？（答案直接填数字，不用带单位）

**答案： 200+50+200+300 = 750**

12、(5分)假设单周期处理器五个阶段的延迟分别为200ps（取指）、50ps（读寄存器）、200ps（ALU操作）、300ps（访存）、100ps（写寄存器），则lw指令的总延迟为多少ps？（答案直接填数字，不用带单位）

**答案： 200+50+200+300+100 = 850**

13、(5分)假设单周期处理器五个阶段的延迟分别为200ps（取指）、50ps（读寄存器）、200ps（ALU操作）、300ps（访存）、100ps（写寄存器），则add指令的总延迟为多少ps？（答案直接填数字，不用带单位）

**答案： 200 + 50 + 200 + 100 = 550**

14、(5分)假设单周期处理器五个阶段的延迟分别为200ps（取指）、50ps（读寄存器）、200ps（ALU操作）、300ps（访存）、100ps（写寄存器），则beq指令的总延迟为多少ps？（答案直接填数字，不用带单位）

**答案： 200 + 50 + 200 = 450**

15、(5分)假设一条指令的32位编码从高到低依次为Ins<31>, Ins<30>, ……, Ins<0>，则产生ExtOp控制信号需要用到指令编码中的多少位？

 **A、 6位**

 B、 12位

 C、 32位

 D、 1位

16、(5分)假设一条指令的32位编码从高到低依次为Ins<31>, Ins<30>, ……, Ins<0>，则产生MemWr控制信号需要用到指令编码中的多少位？

 **A、 6位**

 B、 12位

 C、 32位

 D、 1位

17、(5分)假设一条指令的32位编码从高到低依次为Ins<31>, Ins<30>, ……, Ins<0>，则产生ALUctr[0]控制信号需要用到指令编码中的多少位？

 **A、 12位**

 B、 6位

 C、 7位

 D、 26位

 E、 32位

 F、 14位

18、(5分)假设一条指令的32位编码从高到低依次为Ins<31>, Ins<30>, ……, Ins<0>，则产生RegWr控制信号需要用到指令编码中的多少位？

 **A、 12位**

 B、 6位

 C、 7位

 D、 26位

 E、 32位

 F、 14位
