# SadBoard

每块板子都有问题，找到原因是你的任务。

SadBoard 是一个面向嵌入式 Linux 的故障定位与分析练习项目，计划在 QEMU 和实体开发板上提供不同难度的故障现场，练习从症状观察、证据收集、根因定位到修复验证的完整过程。

## 关注方向

- 内核 Oops、panic 与崩溃转储分析。
- 内存泄漏、内存压力与 OOM。
- CPU、调度、锁竞争、缓存与 I/O 性能分析。
- 网络吞吐、延迟、丢包和重传分析。

计划围绕 GDB、strace、perf、ftrace、trace-cmd、KernelShark、eBPF、iperf3 和火焰图设计实验，并逐步支持指定场景、分级提示和随机盲测。

## 当前状态

项目处于规划阶段，当前仓库包含学习资料，尚未实现故障场景或命令行工具。

## 文档

- [Bootlin Linux 调试课程详解与实验学习指南](docs/bootlin-linux-debugging-guide.md)：课程主题、官方实验、资料链接，以及与 SadBoard 目标的对应关系。

## 仓库

项目名称为 **SadBoard**，当前远程仓库地址为 [linux-bsp/BadBoard](https://github.com/linux-bsp/BadBoard)。

## 资料署名

课程文档中对 Bootlin 实验手册的归纳和改编沿用 CC BY-SA 3.0，具体署名与来源见文档末尾。项目代码许可将在开始实现时另行确定。
