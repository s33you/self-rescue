# Self-Rescue —— 自我发掘 Skills 套件

> 一套 Claude Code Skills，通过持续对话帮你系统性地发现核心能力与优势，找到变现和职业发展的方向。

## 安装

Clone 本仓库到任意目录，用 Claude Code 打开即可使用。所有个人数据由 skills 动态创建，不会入 git。

```bash
git clone <repo-url> self-rescue
cd self-rescue
# 启动 Claude Code，输入 /start 开始
```

## 怎么开始？

**输入 `/start`，然后随便聊就行。**

不需要准备任何东西，不需要知道自己擅长什么。你只管说，AI 会从对话中发现你的能力线索。

## 可用指令

### 第一层：自然对话（零门槛）

| 指令 | 用途 |
|------|------|
| `/start` | **从这里开始。** 随便聊，AI 自动捕捉技能线索 |

### 第二层：定向探索（有方向后）

| 指令 | 用途 | 示例 |
|------|------|------|
| `/explore` | 针对某个方向深入挖掘 | `/explore 技术能力` |
| `/reflect` | 从一段具体经历中提炼能力 | `/reflect 上次做的项目` |

### 第三层：分析输出（积累够了）

| 指令 | 用途 |
|------|------|
| `/assess` | 综合评估核心优势和独特组合 |
| `/opportunity` | 将能力映射到变现/职业方向 |

### 辅助工具

| 指令 | 用途 |
|------|------|
| `/status` | 查看探索进度，看看聊到哪了 |
| `/session` | 保存本次对话的发现 |

## 工作流程

```
/start       随便聊 → 发现线索
                ↓
/explore     深入某个方向 ← /reflect 从经历中提炼
                ↓
/assess      综合分析核心优势
                ↓
/opportunity 探索变现方向

/status 随时查看进度  |  /session 随时保存发现
```

## 项目结构

```
self-rescue/
├── .claude/skills/         # Skills 定义（入 git）
│   ├── start/              # 零门槛自然对话入口
│   ├── explore/            # 按维度深入探索
│   ├── reflect/            # 经历反思提炼
│   ├── session/            # 会话记录
│   ├── assess/             # 综合评估
│   ├── opportunity/        # 变现方向映射
│   └── status/             # 进度总览
├── insights/
│   └── skill-map.md        # 技能探索框架（入 git）
├── profile/                # 个人数据（自动创建，不入 git）
├── exploration/            # 探索记录（自动创建，不入 git）
├── .gitignore
└── README.md
```

## 阶段目标

- **Phase 1：广泛探索** — 用 `/start` 打开话匣子，发现尽可能多的技能线索
- **Phase 2：深度挖掘** — 用 `/explore` 和 `/reflect` 深入，找到反复出现的模式
- **Phase 3：方向聚焦** — 用 `/assess` 确定核心优势，用 `/opportunity` 锁定 2-3 个方向
- **Phase 4：行动计划** — 为选定方向制定具体的变现/发展路径
