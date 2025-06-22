# GourmetGenius - 美食推荐系统 -- 更多在微信 ： jackSinWu --在咸鱼：不知名选手java小鑫 --B站：不知名选手java小鑫 关注可打9折

## 项目介绍
**GourmetGenius** 是一个基于个性化推荐算法的美食推荐系统，旨在为用户提供个性化的美食推荐、菜谱分享、餐厅查找等功能。该项目是 **个人毕业设计**，结合前端 Vue.js、后端 Spring Boot 和机器学习算法，打造智能化美食推荐体验。
![image](https://github.com/user-attachments/assets/baca4894-ce8b-4153-912f-fa4f005e6d02)

## 技术栈
- **前端**：Vue.js + Vuex
- **后端**：Spring Boot + MyBatis + Shiro + Netty
- **数据库**：MySQL
- **存储**：MinIO（对象存储服务）
- **推荐算法**：基于用户行为的协同过滤（CF）、内容推荐（CB）

## 核心功能
### 1. 美食推荐
- 个性化美食推荐（基于用户喜好、浏览记录、评分等）
- 热门菜品、热门餐厅推荐
- 评分与评论系统

### 2. 菜谱管理
- 用户上传菜谱（名称、图片、配料、做法等）
- 菜谱分类管理（中餐、西餐、甜点等）
- 收藏、点赞、评论菜谱

### 3. 餐厅查找
- 按照位置推荐附近的餐厅
- 餐厅详情查看（菜单、评分、地址等）
- 用户点评、打分

### 4. 用户管理
- 账号注册、登录、权限管理（Shiro）
- 用户信息管理
- 实名认证（可选）

### 5. 在线交流（Netty 实现）
- 用户与美食达人在线聊天
- 讨论美食、交流烹饪技巧

### 6. 存储管理（MinIO）
- 上传美食图片、用户头像等
- 文件管理

## 项目部署
### 1. 环境要求
- **JDK 11+**
- **Node.js 16+**
- **MySQL 8+**
- **MinIO 服务器**

### 2. 后端启动
```bash
# 进入后端项目目录
cd backend

# 编译打包
mvn clean package

# 运行 Spring Boot
java -jar target/gourmet-genius.jar
```

### 3. 前端启动
```bash
# 进入前端项目目录
cd frontend

# 安装依赖
npm install

# 启动前端项目
npm run serve
```

### 4. MinIO 配置
- 启动 MinIO 服务器：
```bash
minio server /data --console-address ":9001"
```
- 访问 MinIO 控制台：[http://localhost:9001](http://localhost:9001)
- 配置 **Access Key** 和 **Secret Key**，并在后端 `application.yml` 配置 MinIO 连接信息。

## 目录结构
```bash
gourmet-genius/
├── backend/        # 后端 Spring Boot
│   ├── src/main/   # Java 代码
│   ├── resources/  # 配置文件
│   ├── pom.xml     # Maven 配置
│   └── ...
├── frontend/       # 前端 Vue 项目
│   ├── src/        # Vue 代码
│   ├── public/     # 静态资源
│   ├── package.json# 依赖管理
│   └── ...
├── docs/           # 项目文档
├── README.md       # 项目说明
└── ...
```

## 贡献指南
如果你想参与贡献代码，请遵循以下步骤：

1. **Fork 本仓库**
2. **创建新分支** (`git checkout -b feature-xxx`)
3. **提交代码** (`git commit -m '添加新功能 xxx'`)
4. **推送分支** (`git push origin feature-xxx`)
5. **提交 Pull Request**

## 许可证
本项目基于 **MIT License** 进行开源。

---
如需更多信息或合作，请联系微信：jackSinWu

