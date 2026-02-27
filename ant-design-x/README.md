# Ant Design X Skill

[English](#english) | [中文](#中文)

---

## English

### Overview

**Ant Design X Skill** is a specialized development guide for building AI conversation interfaces using the [Ant Design X](https://x.ant.design) component library.

This skill provides comprehensive knowledge and best practices for creating Language User Interfaces (LUI) for AI-powered applications.

### Core Capabilities

1. **Conversation Components** - Bubble (message bubbles), Sender (input box), Conversations (session management)
2. **Expression Components** - Prompts (quick suggestions), Suggestions (input suggestions), Attachments (file uploads)
3. **Feedback Components** - Actions (action lists), ThoughtChain (thinking chains), Sources (citations)
4. **Rendering Components** - XMarkdown (streaming Markdown), CodeHighlighter (code highlighting), Mermaid (diagrams)
5. **State Components** - Think (thinking process), Welcome (welcome page), Notification (system notifications)

### When to Use

- ✅ Building AI chat interfaces
- ✅ Rendering streaming Markdown content (formulas, code, diagrams)
- ✅ Displaying AI thinking processes or reasoning chains
- ✅ Managing multi-session/historical conversations
- ✅ Providing quick prompts and command inputs
- ✅ Handling file uploads and previews
- ✅ Displaying citations and references
- ✅ Creating welcome onboarding pages

### Trigger Scenarios

This skill activates when users mention:

| Category | Keywords |
|----------|----------|
| **Conversation UI** | "chat interface", "message bubble", "input box", "send message" |
| **AI Components** | "AI conversation", "agent", "bot", "chatbot", "LUI" |
| **Markdown** | "Markdown rendering", "streaming output", "formula rendering", "code highlighting" |
| **Session Management** | "switch conversation", "history", "multi-session", "conversation list" |
| **Interaction Feedback** | "like/dislike", "copy button", "action menu", "thought chain" |
| **File Handling** | "upload file", "attachment", "file preview", "paste image" |
| **Quick Input** | "quick prompt", "slash command", "input suggestion" |

### Documentation Structure

```
ant-design-x/
├── SKILL.md                 # Main skill guide
├── README.md                # This file
└── reference/
    ├── bubble/              # Message bubble component
    ├── sender/              # Input box component
    ├── conversations/       # Session management
    ├── x-markdown/          # Streaming Markdown
    ├── prompts/             # Quick prompts
    ├── suggestion/          # Input suggestions
    ├── attachments/         # File attachments
    ├── file-card/           # File card display
    ├── actions/             # Action lists
    ├── thought-chain/       # Thinking chains
    ├── think/               # Thinking process
    ├── sources/             # Citations
    ├── code-highlighter/    # Code highlighting
    ├── mermaid/             # Mermaid diagrams
    ├── welcome/             # Welcome pages
    ├── notification/        # System notifications
    └── x-provider/          # Global configuration
```

### Quick Start

```bash
npm install @ant-design/x @ant-design/x-markdown
```

```tsx
import { Bubble, Sender } from '@ant-design/x';
import XMarkdown from '@ant-design/x-markdown';

// Basic chat interface
<Bubble.List items={messages} />
<Sender onSubmit={sendMessage} />

// Streaming Markdown
<XMarkdown content={streamingContent} streaming={{ hasNextChunk: isStreaming }} />
```

### Key Features

- 🎨 **Complete LUI Components** - All components needed for AI conversation interfaces
- 🌊 **Streaming Support** - Built-in support for streaming Markdown and typing animations
- 🧠 **Thinking Process Display** - Show AI reasoning and thought chains
- 📁 **File Handling** - Upload, preview, and manage attachments
- 🎯 **Quick Commands** - Slash commands and suggestion prompts
- 🎨 **Theme Customization** - Full theme support via XProvider

---

## 中文

### 概述

**Ant Design X Skill** 是使用 [Ant Design X](https://x.ant.design) 组件库构建 AI 对话界面的专业开发指南。

本技能提供构建 AI 应用语言用户界面（LUI）的完整知识和最佳实践。

### 核心能力

1. **对话组件** - Bubble（消息气泡）、Sender（输入框）、Conversations（会话管理）
2. **表达组件** - Prompts（快捷提示）、Suggestions（建议）、Attachments（附件）
3. **反馈组件** - Actions（操作列表）、ThoughtChain（思维链）、Sources（来源引用）
4. **渲染组件** - XMarkdown（流式 Markdown）、CodeHighlighter（代码高亮）、Mermaid（图表）
5. **状态组件** - Think（思考过程）、Welcome（欢迎页）、Notification（系统通知）

### 使用场景

- ✅ 构建 AI 聊天界面
- ✅ 渲染流式 Markdown 内容（公式、代码、图表）
- ✅ 展示 AI 思考过程或推理链
- ✅ 管理多会话/历史对话
- ✅ 提供快捷提示和命令输入
- ✅ 处理文件上传和预览
- ✅ 展示引用来源和参考链接
- ✅ 创建欢迎引导页面

### 触发场景

当用户提到以下内容时触发此技能：

| 类别 | 关键词 |
|------|--------|
| **对话界面** | "聊天界面"、"对话气泡"、"消息列表"、"输入框"、"发送消息" |
| **AI 组件** | "AI 对话"、"智能体"、"Bot"、"聊天机器人"、"LUI" |
| **Markdown** | "Markdown 渲染"、"流式输出"、"公式渲染"、"代码高亮"、"Mermaid 图表" |
| **会话管理** | "切换会话"、"历史对话"、"多会话"、"会话列表" |
| **交互反馈** | "点赞点踩"、"复制按钮"、"操作菜单"、"思维链"、"思考过程" |
| **文件处理** | "上传文件"、"附件"、"文件预览"、"粘贴图片" |
| **快捷输入** | "快捷提示"、"快捷命令"、"/命令"、"输入建议" |

### 文档结构

```
ant-design-x/
├── SKILL.md                 # 主技能指南
├── README.md                # 本文件
└── reference/
    ├── bubble/              # 消息气泡组件
    ├── sender/              # 输入框组件
    ├── conversations/       # 会话管理
    ├── x-markdown/          # 流式 Markdown
    ├── prompts/             # 快捷提示
    ├── suggestion/          # 快捷命令
    ├── attachments/         # 文件附件
    ├── file-card/           # 文件卡片
    ├── actions/             # 操作列表
    ├── thought-chain/       # 思维链
    ├── think/               # 思考过程
    ├── sources/             # 来源引用
    ├── code-highlighter/    # 代码高亮
    ├── mermaid/             # Mermaid 图表
    ├── welcome/             # 欢迎页
    ├── notification/        # 系统通知
    └── x-provider/          # 全局配置
```

### 快速开始

```bash
npm install @ant-design/x @ant-design/x-markdown
```

```tsx
import { Bubble, Sender } from '@ant-design/x';
import XMarkdown from '@ant-design/x-markdown';

// 基础对话界面
<Bubble.List items={messages} />
<Sender onSubmit={sendMessage} />

// 流式 Markdown
<XMarkdown content={streamingContent} streaming={{ hasNextChunk: isStreaming }} />
```

### 主要特性

- 🎨 **完整 LUI 组件** - AI 对话界面所需的所有组件
- 🌊 **流式支持** - 内置流式 Markdown 和打字动画支持
- 🧠 **思考过程展示** - 展示 AI 推理和思维链
- 📁 **文件处理** - 上传、预览和管理附件
- 🎯 **快捷命令** - 斜杠命令和提示建议
- 🎨 **主题定制** - 通过 XProvider 支持完整主题配置

---

## License

MIT
