# 🖥️ Java后端实战项目

> Week 7 实战项目：完整的Spring Boot后端应用

## 项目概述

一个完整的后端项目，涵盖Java后端开发的核心技能点，可作为面试作品展示。

## 候选方案（三选一）

### 方案A：用户管理系统
- 用户注册/登录（JWT认证）
- 角色权限管理（RBAC）
- 用户CRUD + 分页查询

### 方案B：博客系统
- 用户注册/登录
- 文章发布/编辑/删除
- 分类/标签管理
- 评论系统

### 方案C：API开放平台
- 用户注册/登录 + API密钥管理
- API接口调用与计费
- 接口文档自动生成

## 技术栈

| 组件 | 技术选型 |
|------|----------|
| 框架 | Spring Boot 3.x |
| ORM | MyBatis-Plus |
| 数据库 | MySQL 8.x |
| 缓存 | Redis |
| 认证 | JWT + Spring Security |
| 接口文档 | Knife4j |
| 部署 | Docker + 云服务器 |

## 项目结构（规划）

```
java_backend_project/
├── src/main/java/
│   └── com/gavin/project/
│       ├── controller/        # 接口层
│       ├── service/           # 业务层
│       ├── mapper/            # 数据访问层
│       ├── model/             # 实体类
│       │   ├── entity/
│       │   ├── dto/
│       │   └── vo/
│       ├── config/            # 配置类
│       ├── common/            # 通用工具（Result、异常处理）
│       └── utils/             # 工具类
├── src/main/resources/
│   ├── application.yml
│   └── mapper/
├── Dockerfile
├── docker-compose.yml
├── pom.xml
└── README.md
```

## 核心功能清单

- [ ] 项目初始化（Spring Boot + Maven）
- [ ] 统一返回格式（Result封装）
- [ ] 全局异常处理
- [ ] 用户注册/登录（JWT）
- [ ] 权限控制（Spring Security）
- [ ] CRUD接口 + 分页查询
- [ ] Redis缓存集成
- [ ] Knife4j接口文档
- [ ] Docker打包
- [ ] 云服务器部署

## 性能目标

| 指标 | 目标值 |
|------|--------|
| 接口响应时间 | < 100ms |
| 并发支持 | > 500 QPS |
| 测试覆盖率 | > 60% |
