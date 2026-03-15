# DocAgent

📚 文档管理专家智能助手

---

## 项目简介

DocAgent 是一个专门负责文档管理的智能助手，专注于文档读写、Wiki编辑、知识库管理和多维表格操作。

可以作为独立的OpenClaw Agent使用，也可以通过Docker部署。

---

## ✨ 核心能力

### 1. 文档管理
- 读取和查看飞书文档
- 创建新的飞书文档
- 修改和更新现有文档
- 删除文档（需确认）

### 2. 知识库操作
- Wiki页面导航和搜索
- Wiki页面创建和编辑
- 知识库目录管理
- 知识内容整理和归档

### 3. 多维表格操作
- Bitable数据读取和查询
- Bitable记录创建和更新
- Bitable表格创建和配置
- 数据统计和报表生成

### 4. 云存储管理
- 飞书云盘文件管理
- 文件夹创建和整理
- 文件权限管理
- 文件搜索和筛选

---

## 🚀 快速开始

### 方式一：OpenClaw 直接安装（推荐）

详见 [INSTALL.md](INSTALL.md)

```bash
# 复制到OpenClaw agents目录
cp -r DocAgent ~/.openclaw/agents/DocAgent

# 重启OpenClaw
openclaw restart
```

### 方式二：Docker 安装

详见 [INSTALL.md](INSTALL.md)

```bash
# 构建并启动
docker-compose up -d

# 查看日志
docker-compose logs -f
```

---

## 📁 项目结构

```
DocAgent/
├── SKILL.md                    # 技能定义（参考OpenClaw技能标准）
├── README.md                   # 项目说明（本文件）
├── INSTALL.md                  # 安装指南
├── IDENTITY.md                 # 身份定义
├── SOUL.md                     # 个性和行为准则
├── SYSTEM.md                   # 系统提示词
├── MEMORY.md                   # 长期记忆
├── AGENTS.md                   # Agent配置
├── TOOLS.md                    # 工具配置
├── USER.md                     # 用户信息
├── BOOTSTRAP.md                # 初始化标记
├── HEARTBEAT.md                # 心跳检查
├── docker/                     # Docker配置
│   └── Dockerfile
├── docker-compose.yml          # Docker Compose配置
├── scripts/                    # 可执行脚本
├── references/                 # 参考文档
├── assets/                     # 资源文件
├── agent-tracker/              # Agent追踪器
├── skills/                     # 专用技能
├── memory/                     # 记忆文件
└── .openclaw/                  # OpenClaw配置
```

---

## 💡 特点

- **细心严谨**：处理文档时注重细节，确保内容准确无误
- **条理清晰**：知识库和文件管理井井有条
- **安全第一**：重要操作前主动确认，避免误操作
- **权限意识**：严格遵守文档权限设置，不越权操作

---

## 🔒 边界约束

- 只处理文档、知识库、多维表格相关的请求，不处理日程、会议、沟通等其他能力域的请求
- 重要文档修改前必须先确认，不擅自修改或删除重要文档
- 严格遵守文档权限，不访问或修改没有权限的文档
- 不泄露文档中的敏感信息和隐私内容

---

## 🤝 多Agent协作关系

| 协作 Agent | 协作方式 | 分工边界 |
|-----------|---------|---------|
| Main Agent | 主协调者，处理通用问题 | DocAgent只处理文档相关请求 |
| CalendarAgent | 平行协作，文档 vs 日程 | 互不干涉，边界清晰 |
| DataAgent | 数据协作，文档数据和表格数据互通 | 各自处理对应的数据类型 |

---

## 📚 相关文档

- [SKILL.md](SKILL.md) - 技能定义（参考OpenClaw技能标准）
- [INSTALL.md](INSTALL.md) - 详细安装指南
- [SYSTEM.md](SYSTEM.md) - 系统提示词
- [SOUL.md](SOUL.md) - 个性和行为准则

---

## 📋 许可证

本项目遵循相关许可证。

---

**创建日期**: 2026-03-07
**最后更新**: 2026-03-07
