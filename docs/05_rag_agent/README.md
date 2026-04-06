# RAG + Agent (LangChain) · 学习笔记

## 学习资源
- LangChain 官方文档：python.langchain.com/docs
- B站：搜"LangChain RAG 实战"
- GitHub：langchain-ai/langchain 官方examples

## 学习阶段

### 阶段1：基础概念（2-3天）
- [ ] LangChain核心抽象：LLM、Chain、Prompt Template、Output Parser
- [ ] 跑通最简单的 LLM 调用 + Prompt模板

### 阶段2：RAG Pipeline（4-5天）
- [ ] Document Loader → Text Splitter → Embedding → Vector Store → Retriever → Chain
- [ ] 用 Chroma 或 FAISS 做向量存储
- [ ] 实现本地文档问答系统（PDF/Markdown）
- [ ] 理解 chunk_size、overlap、top_k 对效果的影响

### 阶段3：本地LLM接入（2-3天）
- [ ] 用 Ollama 跑本地模型（Qwen2.5、Llama3等）
- [ ] LangChain 对接 Ollama

### 阶段4：Agent基础（3-4天）
- [ ] ReAct Agent 原理（思考→行动→观察）
- [ ] LangChain Agent + 自定义Tool
- [ ] 实现能调用搜索+计算工具的简单Agent

### 阶段5：RAG + Agent整合（3-4天）
- [ ] RAG检索作为Agent的Tool
- [ ] 用户提问 → Agent判断是否检索 → 检索后回答
- [ ] 加入对话记忆（ConversationBufferMemory）

### 阶段6：和ROS2结合（项目阶段）
- [ ] Agent接收自然语言指令 → 解析意图 → 调用ROS2 Service/Action
- [ ] 示例："去检测桌子上的红色物体" → YOLO检测 + 导航指令

## 面试要点
- 能说清RAG完整数据流
- 能解释chunk_size/embedding模型的选择理由
- 理解ReAct循环原理
- 知道框架帮你做了什么，不用框架需要自己处理什么
