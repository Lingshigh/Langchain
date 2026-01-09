# Langchain
## 1.Langchain核心概念

### 图结构（Graph struct）
LangGraph将应用逻辑变为一个有向图，其中：
结点（Nodes）代表具体操作或计算步骤，可以是调用语言模型、执行函数或与外部工具交互等
边（Edges）：定义节点之间的连接和执行顺序，支持普通边（直接连接）和条件边（基于条件动态选择下一步）
### 状态管理（State Management）
LangGraph的核心特点是自动维护和管理状态
状态是一个贯穿整个图的共享数据结构，记录了应用运行过程的上下文信息
每个节点可以根据当前执行任务并更新状态，确保系统在多步骤或多主题交互中保持一致
### 循环能力（Cyclical Working）
与传统的线性工作流不同，LangGraph支持循环逻辑这使其非常适合需要反复推理、决策或与用户交互的代理应用
<img width="512" height="278" alt="image" src="https://github.com/user-attachments/assets/fa7850ef-886c-4629-a394-83fe4fec94e9" />

