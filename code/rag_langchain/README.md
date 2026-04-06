# RAG + Agent (LangChain) 项目代码

## 环境准备

```bash
pip install langchain langchain-community chromadb faiss-cpu sentence-transformers
pip install ollama  # 本地LLM
```

## 目录结构

```
rag_langchain/
├── 01_basic_chain/        # LLM调用 + Prompt模板
├── 02_rag_pipeline/       # 完整RAG流程
├── 03_local_llm/          # Ollama本地模型接入
├── 04_agent_basic/        # ReAct Agent + 自定义Tool
├── 05_rag_agent/          # RAG + Agent整合
└── 06_ros2_integration/   # 与ROS2结合
```
