# RAG + Agent + Spring AI · 学习笔记

## 学习资源
- LangChain官方文档：python.langchain.com/docs
- Spring AI官方文档：docs.spring.io/spring-ai
- B站：搜"LangChain RAG 实战"
- B站：搜"Spring AI 入门"

## 学习阶段

### Week 9：Python + LLM基础
- [ ] Python基础补强（如已会可跳过）
- [ ] LLM API调用（OpenAI / 通义千问 / Ollama本地）
- [ ] Prompt Engineering基础

### Week 10：LangChain RAG Pipeline
- [ ] LangChain核心抽象（LLM、Chain、Prompt Template、Output Parser）
- [ ] Document Loader → Text Splitter → Embedding → Vector Store → Retriever
- [ ] 用Chroma/FAISS实现本地文档问答
- [ ] 理解chunk_size、overlap、top_k对效果的影响

### Week 11：Agent + Tool Calling
- [ ] ReAct Agent原理（思考→行动→观察）
- [ ] LangChain Agent + 自定义Tool
- [ ] RAG作为Agent Tool
- [ ] 对话记忆（ConversationBufferMemory）

### Week 12：Spring AI（核心差异化）
- [ ] Spring AI框架概述
- [ ] Java调用LLM API
- [ ] Java实现Embedding + 向量检索
- [ ] 用Java实现RAG Pipeline
- [ ] 对比Python版和Java版的差异

### Week 13-14：AI应用闭环项目
- [ ] 项目选型与架构设计
- [ ] 后端开发（Spring Boot + Spring AI）
- [ ] RAG + Agent集成
- [ ] 前端页面（简单Vue/React或纯接口）
- [ ] 部署与测试

## 面试要点
- 能说清RAG完整数据流
- 能解释chunk_size/embedding模型的选择理由
- 理解ReAct循环原理
- Spring AI和LangChain的区别与各自优势
- 为什么用Java做AI应用（企业级、生态、性能）
