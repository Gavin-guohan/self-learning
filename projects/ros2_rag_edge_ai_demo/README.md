# 🤖 ROS2 + RAG + TensorRT YOLO 边缘AI Demo

> 闭环项目：实时视觉检测 + 自然语言指令理解 + Agent决策控制

## 项目概述

用户通过自然语言下达指令（如"检测桌上的红色物体"），系统通过 LangChain Agent 解析意图，调用 YOLO 视觉检测节点进行目标识别，并将结果通过 ROS2 通信反馈给用户或下游控制模块。

## 系统架构

```
用户指令（文本）
    │
    ▼
LangChain Agent（意图解析 + 工具调用）
    │
    ├──► RAG检索（知识库查询）
    │
    ├──► ROS2 Service 调用
    │       │
    │       ▼
    │   YOLO检测节点（TensorRT加速）
    │       │
    │       ▼
    │   相机图像 → 检测结果
    │
    ▼
结果汇总 + 自然语言回复
```

## 技术栈

| 组件 | 技术选型 |
|------|----------|
| LLM推理 | Ollama (Qwen2.5/Llama3) |
| Agent框架 | LangChain ReAct Agent |
| 向量检索 | Chroma / FAISS |
| 目标检测 | YOLOv8 + TensorRT |
| 机器人通信 | ROS2 Humble |
| 部署平台 | Jetson Orin Nano / RK3588 |

## 目录结构

```
ros2_rag_edge_ai_demo/
├── README.md
├── agent/                 # LangChain Agent + RAG
│   ├── agent_node.py      # Agent主逻辑
│   ├── tools/             # 自定义工具（ROS2调用等）
│   └── knowledge_base/    # 知识库文档
├── detection/             # YOLO检测模块
│   ├── yolo_ros_node.py   # ROS2检测节点
│   ├── engine/            # TensorRT引擎文件
│   └── utils/             # 前后处理
├── launch/                # ROS2 Launch文件
├── config/                # 配置文件
├── docker/                # Docker部署（可选）
└── docs/                  # 项目文档 + 性能报告
```

## 开发计划

- [ ] Phase 1：YOLO检测节点（ROS2 + TensorRT）
- [ ] Phase 2：LangChain Agent + RAG模块
- [ ] Phase 3：Agent ↔ ROS2 桥接
- [ ] Phase 4：端侧部署 + 性能优化
- [ ] Phase 5：文档 + Demo视频 + 性能报告

## 性能目标

| 指标 | 目标值 |
|------|--------|
| 检测FPS (Jetson) | ≥ 25 |
| Agent响应延迟 | < 3s |
| 端到端延迟 | < 5s |
| 显存占用 | < 4GB |
