# clawhub-setup-cn

面向中文用户的 ClawHub 安装与使用技能（Skill），覆盖安装、镜像配置、**找技能**（发现/推荐）以及技能管理。**完全覆盖 skill-finder-cn 的能力**，安装本技能即可替代 skill-finder-cn。

## 技能结构（标准 Skill 布局）

```
clawhub_install_use/
├── SKILL.md    # 技能说明与触发条件（必选）
├── README.md   # 本文件
└── .gitignore
```

## 功能

- ClawHub 安装与初始化
- 镜像配置（支持阿里云镜像）
- **找技能**：根据需求发现、推荐并安装技能（覆盖 skill-finder-cn）
- 技能的安装、更新、启用/禁用

## 安装

```bash
clawhub install clawhub-setup-cn
```

## 触发场景

当在 Claude Code / Cursor 中提到以下关键词时，该技能会被自动激活：

- `clawhub`、`安装 clawhub`、`clawhub 怎么用`
- `找技能`、`有什么技能可以`、`找一个技能`、`搜索技能`
- `安装技能`、`更新技能`、`管理技能`
- `clawhub init`、`clawhub install`、`clawhub search`、`clawhub update`
- `openclaw skills`

## 许可证

MIT
