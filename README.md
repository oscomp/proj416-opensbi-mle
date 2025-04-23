# opensbi-mle

项目名称：{面向智能操作系统的 RISC-V SBI 机器学习拓展}

项目链接：{https://github.com/xuyuanchao-cnu/opensbi-mle}

导师信息：{姓名：徐远超、Github ID：xuyuanchao-cnu、邮箱：xuyuanchao@cnu.edu.cn}

难度：{高}

分类：{未归类运行时支撑}

题目要求：{
描述题目的功能需求、性能需求、应用场景、约束等。描述尽量条目化，列举的功能尽
量从易到难，从简单到复杂，有一定的层次性。
随着人工智能与机器学习技术的广泛应用，传统操作系统在高效利用异构硬件（尤其是 AI 加速器）以及支持虚拟化环境下的 AI 任务方面面临严峻挑战。例如，在单机多操作系统场景中，各客户机操作系统维护独立机器学习库导致资源冗余。为应对这些挑战，本赛题基于开放指令集架构 RISC-V，尝试使用SBI机制解决操作系统内核智能化支持的难题。
}

特征：{}

预期目标：{

### 第一题 定义SBI机器学习拓展接口规范
设计并定义 SBI 机器学习拓展（MLE）接口规范，包括分配专属拓展 ID、确定涵盖矩阵乘法、卷积、激活函数等十余种基础机器学习算子的函数接口（FID），并规范基于物理地址传递的调用约定和关键数据结构（如 Tensor）。
### 第二题 基于OpenSBI实现机器学习拓展
基于开源固件 OpenSBI 实现了 SBI MLE 的原型系统。完成拓展注册、ecall 分发机制，并尝试实现在机器模式下配置 FPU/Vector 等硬件单元、自适应算法选择等高性能计算环境的构建方法。
### 第三题 设计一个智能操作系统Case
设计一个案例展示如何将内核内部机器学习运算函数调用替换为的 SBI MLE 调用，并处理跨特权级内存交互。展示本方案在解决内核智能化支持的优越性。
}

License：{Apache 2.0}

参考资料：{  
[1] RISC-V Software Group. OpenSBI：RISC-V Supervisor Binary Interface. Available at：https://github.com/riscv-software-src/opensbi. Accessed：2025-04-14.  
[2] RISC-V Non-ISA Group. RISC-V SBI Documentation. Available at：https://github.com/riscv-non-isa/riscv-sbi-doc. Accessed：2025-04-14.  
[3] 陈海波, 夏虞斌, 陈榕, 等. (2025). 模型原生操作系统：机遇、挑战与展望. 计算机科学学会通讯, 21(2), 38-45.  
[4] 唐楚哲, 王肇国, 陈海波. 机器学习方法赋能系统软件：挑战、实践与展望[J]. 计算机研究与发展, 2023, 60(5)：964-973.  
[5] Akgun I U, Aydin A S, Zadok E. KMLIB：Towards machine learning for operating systems[C]//Proceedings of the On-Device Intelligence Workshop, co-located with the MLSys Conference. 2020：1-6.  
[6] Fingler H, Tarte I, Yu H, et al. Towards a machine learning-assisted kernel with lake[C]//Proceedings of the 28th ACM International Conference on Architectural Support for Programming Languages and Operating Systems, Volume 2. 2023：846-861.  
}
