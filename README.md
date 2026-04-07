# Self-Rescue — 自我发掘 Skills 套件

> 一套 Claude Code Skills，通过持续对话帮你系统性地发现核心能力与优势，找到变现和职业发展的方向。

## 安装

```bash
# 安装全部 skills
npx skills add https://github.com/s33you/self-rescue --all

# 或只安装某个 skill
npx skills add https://github.com/s33you/self-rescue --skill start
```

## 更新

重新运行安装命令即可获取最新版本：

```bash
npx skills add https://github.com/s33you/self-rescue --all
```

## 使用

**输入 `/start`，然后随便聊就行。**

不需要准备任何东西，不需要知道自己擅长什么。你只管说，AI 会从对话中发现你的能力线索。

所有个人数据自动保存在当前目录的 `.self-rescue/` 下。

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

### 第四层：方案深化（选定方向后）

| 指令 | 用途 | 示例 |
|------|------|------|
| `/plan` | 针对某个方向深化方案，从战略推演到落地执行 | `/plan 技术咨询` |

### 第五层：持续成长（执行中）

| 指令 | 用途 | 示例 |
|------|------|------|
| `/grow` | 成长中心：学习目标、随时记录、定期回顾 | `/grow 今天学了用Figma做原型` |

### 辅助工具

| 指令 | 用途 |
|------|------|
| `/status` | 查看探索进度 |
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
                ↓
/plan        深化方案（战略推演 → 落地执行）
                ↓
/grow        持续成长（设目标 → 记录学习 → 回顾成长）

/status 随时查看进度  |  /session 随时保存发现
```

## 数据存储

所有个人数据存储在工作目录的 `.self-rescue/` 下，由 skills 自动创建：

```
.self-rescue/
├── profile/
│   ├── skills.md           # 技能清单
│   ├── experiences.md      # 关键经历
│   ├── values.md           # 价值观与驱动力
│   ├── strengths.md        # 核心优势总结
│   └── opportunities.md    # 变现方向分析
├── plans/                  # 方案深化文件（每个方向一个）
├── growth/
│   ├── goals.md            # 学习目标
│   ├── log/                # 月度学习记录
│   └── reviews/            # 定期成长回顾
└── sessions/               # 每次探索的记录
```

建议将 `.self-rescue/` 加入项目的 `.gitignore`。
