# 🤖 AI Agent 智能应用项目

> Week 13-14 闭环项目：Spring Boot + LangChain RAG + Agent

## 项目概述

一个完整的AI应用项目，展示Java后端 + AI能力的贯通。用户通过自然语言与系统交互，系统通过RAG检索知识库、Agent调用工具，返回智能回答。

## 候选方案（二选一）

### 方案A：智能知识库问答系统
- 上传文档（PDF/Markdown）→ 自动分块 → 向量化存储
- 用户提问 → RAG检索 → LLM生成回答
- Agent判断是否需要检索、调用工具

### 方案B：AI驱动的数据查询平台
- 自然语言 → 生成SQL → 查询数据库 → 返回结果
- Agent调用数据库工具 + 计算工具
- 支持多轮对话

## 系统架构

```
用户（前端页面/API）
    │
    ▼
Spring Boot 后端
    │
    ├──► Spring AI / LangChain Agent
    │       │
    │       ├──► RAG检索（Chroma/FAISS）
    │       ├──► 工具调用（数据库查询/计算/搜索）
    │       └──► LLM推理（Ollama本地 / 云端API）
    │
    ├──► MySQL（业务数据）
    └──► Redis（缓存/会话）
```

## 技术栈

| 组件 | 技术选型 |
|------|----------|
| 后端框架 | Spring Boot 3.x |
| AI框架 | Spring AI + LangChain（Python） |
| LLM | Ollama（Qwen2.5/Llama3）/ 通义千问API |
| 向量数据库 | Chroma / FAISS |
| Embedding | sentence-transformers / 通义Embedding |
| 业务数据库 | MySQL |
| 缓存 | Redis |
| 前端 | Vue3（简单页面）或纯API |

## 项目结构（规划）

```
ai_agent_project/
├── backend/                   # Spring Boot后端
│   ├── src/main/java/
│   │   └── com/gavin/ai/
│   │       ├── controller/    # API接口
│   │       ├── service/       # 业务逻辑
│   │       ├── agent/         # Agent + Tool定义
│   │       ├── rag/           # RAG Pipeline
│   │       ├── config/        # 配置
│   │       └── model/         # 实体类
│   └── pom.xml
├── agent-python/              # Python端Agent（可选）
│   ├── agent.py
│   ├── rag_pipeline.py
│   └── requirements.txt
├── frontend/                  # 前端页面（简单）
├── docker-compose.yml
└── README.md
```

## 开发计划

- [ ] Phase 1：后端基础框架搭建
- [ ] Phase 2：RAG Pipeline（文档上传 → 分块 → 向量化 → 检索）
- [ ] Phase 3：Agent + Tool Calling
- [ ] Phase 4：Spring AI集成（Java原生AI能力）
- [ ] Phase 5：前端页面 + 联调
- [ ] Phase 6：部署 + Demo录制

## 核心亮点（面试展示）
- Java后端 + AI能力贯通（Spring AI）
- 不仅会用Python LangChain，还能用Java实现同等功能
- 完整的工程化：Docker部署、接口文档、错误处理
- 支持本地LLM，不依赖云端API
