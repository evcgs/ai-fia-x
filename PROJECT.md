# FIA-X 多智能体创新架构

## 项目概述

FIA-X是一个**系统化AI创新方法论**，基于三大支柱：

1. **First-principle** - 第一性原理问题拆解
2. **Interdisciplinary** - 跨学科知识交叉迁移
3. **Anti-consensus** - 反共识创新思维

通过七个专业智能体的专业化分工，让AI真正产生突破性创新，而不是常规问答。

## 核心特点

| 特点 | 说明 |
|------|------|
| 专业化分工 | 每个智能体只专注一个创新环节，专业能力最大化 |
| 多重质量闸门 | 四道质量闸门，提前发现问题，降低返工率 |
| 完全符合OIA | 遵循OpenClaw OIA六步闭环执行标准，协同质量有保证 |
| 分层设计 | OIA管顶层协同，FIA管专业创新，各司其职 |
| 记忆隔离互通 | 每个智能体独立记忆存储，支持跨Agent检索 |
| 可扩展 | 基于FIA-X核心，可以快速开发行业扩展包 |

## 目录结构

```
ai-fia-x/
├── README.md              # 项目说明（对外）
├── PROJECT.md             # 项目文档
├── openclaw-skill.json    # OpenClaw技能配置
├── LICENSE               # MIT许可证
├── agents/               # 七个专业智能体
│   ├── ProblemAgent/
│   ├── KnowledgeAgent/
│   ├── HypothesisAgent/
│   ├── SolutionAgent/
│   ├── EvaluationAgent/
│   ├── ExecutionAgent/
│   └── LearningAgent/
└── docs/
    ├── FIA-X多智能体架构规范v1.2.md  # 完整规范
    └── 配置示例.md                     # 配置参考
```

## 版本信息

- **版本**：v1.2.0
- **发布日期**：2026-03-15
- **要求**：OpenClaw >= 2026.3.x
- **依赖**：memos-cloud-openclaw-plugin >= 0.1.9

## 安装

### OpenClaw一键安装
```bash
openclaw install evcgs/ai-fia-x
```

### 手动安装
```bash
cd ~/.openclaw/workspace
git clone https://github.com/evcgs/ai-fia-x.git
# 按照 docs/配置示例.md 添加配置到 openclaw.json
# 重启网关
openclaw gateway restart
```

## 变更日志

### v1.2.0 (2026-03-15)
- ✅ 适配OIA规范，采用分层设计
- ✅ 明确OIA-FIA映射关系
- ✅ 遵循OIA任务分发规则：项目→PMAgent，文档→DocAgent
- ✅ 增加PMAgent最终质量审核环节
- ✅ 七个FIA智能体分工完全保持不变

### v1.1.0 (2026-03-15)
- ✅ 新增RiskAgent风险预审环节
- ✅ 新增ProblemAgent一致性复核环节
- ✅ 优化LearningAgent参与方式，每个阶段小结

### v1.0.0 (2026-03-15)
- ✅ 初始版本，七个智能体分工设计
