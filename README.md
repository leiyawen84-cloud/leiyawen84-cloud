## Hi there 👋

# Ti60 二维图形渲染加速工程学习记录

这里记录我与队友对 **Ti60_FIN2_HUD2** 工程的理解，对应竞赛赛题二：基于 RISC-V 与 FPGA 异构架构的 2D 图形渲染加速引擎。

RISC-V 负责游戏逻辑、场景组织和绘图任务提交，FPGA 负责图像搬运、填充、透明处理与显示输出。我们通过源码阅读，逐步理解各模块怎样协同工作。

## 阅读入口

👉 **[项目设计思路、底层流程与源码阅读笔记](docs/project-understanding.md)**

文档包括：

- 赛题要求与工程实现的对应关系。
- 软硬件分工与一帧的执行过程。
- 绘图命令、APB 控制、AXI 访存和 DMA。
- 拷贝、填充、Color Key、Alpha 与 Add 混合。
- DDR 带宽优化、三缓冲及 HDMI 显示。
- 专用弹幕路径、测试模式和历史验收数据的边界。
- 源码阅读入口及后续学习计划。

## 一起完善

欢迎队友补充理解、提出问题或纠正文档。可以通过 Issue 讨论，也可以提交修改；已获得协作者权限的成员可以按团队约定提交更新。

笔记中的源码实现、个人推断和历史测试记录应分别注明。本文档仓库用于学习交流，目前不包含完整工程源码或固件。

<!--
**leiyawen84-cloud/leiyawen84-cloud** is a ✨ _special_ ✨ repository because its README.md appears on your GitHub profile.
-->
