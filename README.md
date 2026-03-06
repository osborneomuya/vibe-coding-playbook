# Vibe Coding Playbook

**用 AI 写代码很快，但写出能维护的代码很难。**

这个仓库解决的问题是：当你用 Cursor / Windsurf 等 AI IDE 开发时，如何**不让项目在高速迭代中失控**——代码越写越乱、AI 越改越偏、Bug 修了又来。

这里沉淀了一套经过实战验证的**提示词、工作流和协作规范**，帮你：

- **约束 AI 行为**：让它遵守你的代码风格、不擅自重构、不乱删代码
- **控制代码质量**：组件结构、状态管理、五态处理等前端核心问题有章可循
- **高效交付 UI**：有设计稿用工具转码 + AI 重构，没设计稿用组件库 + AI 设计工具
- **管理复杂度**：从项目启动到维护修复，每个阶段都有明确的过程规范

> 所有内容持续迭代中，欢迎提 Issue 或 PR 分享你的 Vibe Coding 经验。

---

## 快速开始

- **第一步**：先把 [AI IDE 全局规则](prompts/global-rules.md) 放进你的 Windsurf / Cursor 全局提示词里
- **第二步**：按场景选择工作流
  - 前端任务看 [前端 Vibe 工作流](prompts/frontend-vibe-workflow.md)
  - 后端任务看 [后端 Vibe 工作流](prompts/backend-vibe-workflow.md)
- **第三步**：按交付场景补上下文
  - 有设计稿 / 无设计稿，看 [AI 高质量交付前端 UI](experiences/design-to-code.md)
  - 需要过程规范和复杂度控制，看 [复杂度管理与人机协作 SOP](experiences/vibe-coding-sop.md)
- **第四步**：需要实时文档、搜索、代码索引能力时，按 [MCP 服务配置](tools/mcp-servers.json) 和 [MCP 服务说明](tools/mcp-servers.md) 配置工具

---

## 内容索引

### 提示词

| 文件 | 说明 |
|------|------|
| [AI IDE 全局规则](prompts/global-rules.md) | 贴入 AI IDE 的全局提示词，控制 AI 行为边界（适用于 Windsurf / Cursor） |
| [前端 Vibe 工作流](prompts/frontend-vibe-workflow.md) | 核心原则、组件结构、状态管理、Prompt 写法、审计清单 |
| [后端 Vibe 工作流](prompts/backend-vibe-workflow.md) | 不变量、DoD、LLM 集成、慢 SQL 定位 |

### 实战经验

| 文件 | 说明 |
|------|------|
| [复杂度管理与人机协作 SOP](experiences/vibe-coding-sop.md) | 四阶段 SOP：前置基建 → 过程控制 → 质量闸口 → 维护修复 |
| [AI 高质量交付前端 UI](experiences/design-to-code.md) | 有设计稿 / 无设计稿两种场景的完整方案 |

### 工具配置

| 文件 | 说明 |
|------|------|
| [MCP 服务配置](tools/mcp-servers.json) | Context7 / Exa / Tavily / AWSLabs Document Loader / Ace Tool 配置模板 |
| [MCP 服务说明](tools/mcp-servers.md) | 每个 MCP Server 的用途、核心能力与配置方式 |

---

## 目录结构

```
vibe-coding-playbook/
├── prompts/        # 提示词（全局规则、前端/后端工作流）
├── experiences/    # 实战经验（SOP、设计稿还原等）
└── tools/          # 工具配置（MCP Server 等）
```
