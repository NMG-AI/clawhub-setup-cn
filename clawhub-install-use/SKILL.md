---
name: clawhub-install-use
description: "ClawHub 安装和使用指南。帮助用户安装 ClawHub、配置镜像、安装/更新/管理技能（Skills）。当用户提到 'clawhub'、'安装 clawhub'、'clawhub 怎么用'、'安装技能'、'更新技能'、'管理技能'、'clawhub init'、'clawhub install'、'clawhub update'、'openclaw skills' 时使用此技能。"
---

# ClawHub 安装和使用

## 安装 ClawHub

```bash
# npm 安装
npm install -g clawhub

# 或 pnpm 安装
pnpm add -g clawhub
```

初始化：

```bash
clawhub init
```

配置阿里云镜像（推荐国内用户）：

```bash
clawhub config set clawhub.mirror "https://mirror.aliyun.com/clawhub/"
```

## 安装核心技能

批量安装新手必备技能（等待 5-10 分钟）：

```bash
clawhub install tavily-search find-skills proactive-agent-1-2-4 pdf-chat file-organizer
```

验证安装状态：

```bash
openclaw skills list
```

## 技能管理

### 搜索与安装

```bash
# 搜索技能
clawhub search "<关键词>"

# 查看技能详情
clawhub inspect <技能名称>

# 安装技能
clawhub install <技能名称>

# 安装指定版本
clawhub install <技能名称>@<版本号>
```

### 更新

```bash
# 更新单个技能
clawhub update <技能名称>

# 更新所有技能（推荐定期执行）
clawhub update --all
```

### 启用与禁用

```bash
# 查看技能状态
openclaw skills list --status

# 禁用技能
openclaw skills disable <技能名称>

# 启用技能
openclaw skills enable <技能名称>
```
