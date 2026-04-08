# AI Agent 代码

Week 9-14 的AI应用开发代码。

## 目录结构

```
ai_agent/
├── 01_llm_basic/          # LLM API调用 + Prompt Engineering
├── 02_rag_pipeline/       # LangChain RAG Pipeline
├── 03_agent/              # Agent + Tool Calling
└── 04_spring_ai/          # Spring AI（Java版RAG/Agent）
```

## 环境准备

### Python端
```bash
pip install langchain langchain-community chromadb faiss-cpu sentence-transformers
pip install ollama
```

### Java端（Spring AI）
```xml
<dependency>
    <groupId>org.springframework.ai</groupId>
    <artifactId>spring-ai-openai-spring-boot-starter</artifactId>
</dependency>
```
