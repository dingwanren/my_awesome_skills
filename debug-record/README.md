# Bug Fix Doc Skill

自动记录 Bug 修复文档的技能。

## 安装

### 方式 1：本地安装（推荐）

将 `skills/bug-fix-doc` 目录复制到 Qwen 技能目录：

```powershell
# PowerShell
Copy-Item -Recurse ".\skills\bug-fix-doc" "$env:USERPROFILE\.qwen\skills\bug-fix-doc"
```

或在 Qwen 设置中添加技能路径指向 `skills/bug-fix-doc`。

### 方式 2：直接使用

在 Qwen 配置中引用此目录的绝对路径。

## 使用

安装后，当你说以下内容时会自动触发：
- "有 bug"、"报错了"、"出错了"
- "有问题"、"帮我修复"
- 粘贴错误日志

技能会自动在项目的 `docs/bugfixes/` 目录下创建修复记录。

## 目录结构

```
debug_skill/
├── skills/
│   └── bug-fix-doc/     ← 安装这个目录到 Qwen
│       └── SKILL.md
├── templates/            ← 开发用模板参考（可选）
├── docs/
│   └── bugfixes/        ← 技能输出目录示例
├── evals/               ← 开发测试用（不需要安装）
└── README.md            ← 本文件
```

## 记录格式

生成的文档包含：
- 📅 日期时间
- 🏷️ 问题类型（bug/性能/安全/重构/...）
- 📦 涉及模块
- 📝 问题描述 + 复现步骤
- 🔍 根因分析
- 🔧 修复方案 + 代码变更
- ✅ 验证方式
- 🛡️ 预防措施
