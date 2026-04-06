### self learning

## 📊 学习进度看板

| 模块 | 进度 | 状态 |
|------|------|------|
| 数据结构与算法 | □□□□□□□□□□ 0% | 🔜 待开始 |
| 计算机组成原理 | □□□□□□□□□□ 0% | 🔜 待开始 |
| 操作系统 | □□□□□□□□□□ 0% | 🔜 待开始 |
| 计算机网络 | □□□□□□□□□□ 0% | 🔜 待开始 |
| 数字/模拟电路 | □□□□□□□□□□ 0% | 🔜 待开始 |
| ROS2 Humble | □□□□□□□□□□ 0% | 🔜 待开始 |
| RAG + Agent (LangChain) | □□□□□□□□□□ 0% | 🔜 待开始 |
| TensorRT 端侧部署 | □□□□□□□□□□ 0% | 🔜 待开始 |
| 嵌入式 Linux | □□□□□□□□□□ 0% | 🔜 待开始 |

## 🎯 当前目标

Week 01：算法（数组+链表）+ 计算机组成原理（系统概述+数据表示）

## 🚀 核心项目

**ROS2 + RAG + TensorRT YOLO 边缘AI Demo**（规划中）
- 实时视觉检测 + 自然语言指令理解 + Agent决策控制
- 目标平台：Jetson Orin Nano / RK3588

---

## 🗂️ 仓库结构

```
.
├── docs/                        # 学习笔记
│   ├── 01_algo/                 # 数据结构与算法
│   ├── 02_cs_fundamentals/      # 计算机基础（组原/OS/网络）
│   ├── 03_ee_fundamentals/      # 电路基础（数电/模电）
│   ├── 04_ros2/                 # ROS2 Humble
│   ├── 05_rag_agent/            # RAG + Agent (LangChain)
│   ├── 06_deployment/           # TensorRT + 嵌入式部署
│   └── weekly_review/           # 每周复盘
├── code/                        # 手写代码
│   ├── algo_solutions/          # LeetCode题解
│   ├── rag_langchain/           # RAG + Agent 项目代码
│   ├── ros2_ws/                 # ROS2 工作空间
│   ├── tensorrt_deploy/         # TensorRT 部署代码
│   └── embedded_linux/          # 嵌入式Linux实验
├── projects/                    # 核心项目
│   └── ros2_rag_edge_ai_demo/   # 闭环项目
├── assets/                      # 截图、GIF、性能对比图
├── scripts/                     # 构建、部署脚本
└── .github/workflows/           # CI（可选）
```

## 📅 16周节奏

| 阶段 | 周次 | 内容 |
|------|------|------|
| 基础夯实 | 1-5 | 算法 + 计算机基础 + 电路 |
| 核心技能 | 6-10 | ROS2 + RAG/Agent + 嵌入式Linux |
| 工程部署 | 11-14 | TensorRT部署 + 模块整合 |
| 项目冲刺 | 15-16 | 闭环项目 + 文档美化 + 复盘 |

## 🛠️ 技术栈

- **语言**：Python / C++
- **机器人**：ROS2 Humble / Gazebo
- **AI框架**：PyTorch / ONNX / TensorRT
- **RAG/Agent**：LangChain / Chroma / FAISS / Ollama
- **嵌入式**：Jetson Orin Nano / RK3588 / ARM Linux
- **工具**：Docker / Git / VS Code / Rviz2

## 📝 提交规范

```
week[05]-day[03]: [ROS2] 完成图像发布订阅节点 + CvBridge测试
week[06]-day[01]: [RAG] LangChain RAG Pipeline + Chroma检索
```

## 📜 License

MIT
