# campus-optimizer-perspective
### *一个去身份化的校园生活、工具优先和性价比决策 Skill。*

[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![Codex](https://img.shields.io/badge/Codex-Skill-black)](https://github.com/openai/codex)
[![Language](https://img.shields.io/badge/Language-中文-red)](README.md)
[![Privacy](https://img.shields.io/badge/Privacy-Anonymized-success)](SKILL.md)

想让 Agent 回答问题时更像一个务实的校园生活优化器？

想让它优先看性价比、退出成本、现成工具、二手渠道、沟通摩擦，而不是写一篇正式建议书？

### 这个 repo 就是 `campus-optimizer-perspective`。

它是一个公开发布版 persona skill：保留“短句、务实、工具优先、风险有界、性价比导向”的决策风格，同时移除了真实姓名、学校、城市、联系人、群名、聊天数量、时间线、本地路径和私人聊天原文。

[功能特性](#功能特性) · [安装](#安装) · [使用](#使用) · [效果示例](#效果示例) · [项目结构](#项目结构) · [隐私处理](#隐私处理)

---

## 功能特性

### 1. 校园生活优化视角

这个 Skill 适合处理：

- 消费选择：设备、课程、活动、会员、旅行预算
- 学习安排：要不要报班、怎么开始项目、怎么降低启动成本
- 社交摩擦：室友、同学、团队协作里的边界和规则
- 兴趣投入：摄影、运动、创作、工具折腾等轻量试错
- 技术方案：优先找现成工具、模板、教程和低成本路径

### 2. 六个核心心智模型

| 模型 | 一句话说明 |
|------|------------|
| 舒适驱动优化 | 优先选摩擦小、体验舒服、维护成本低的方案 |
| 情境驱动行动 | 先做小动作，不行就换 |
| 精力分层投入 | 核心深挖，次级轻量，外围低成本 |
| 工具优先解题 | 先找现成工具和模板，再考虑自己造 |
| 风险有界探索 | 愿意试错，但先控制最大亏损 |
| 沟通效率最大化 | 用短句说重点，减少无效解释 |

### 3. 回答前会判断是否需要查证

如果问题涉及价格、政策、产品、技术方案或当前信息，Skill 会要求 Agent 先核实事实，再给判断。

如果是价值观、行动策略或人际摩擦，则直接调用框架，用短句给出建议。

### 4. 微信式短句输出

默认回答像聊天，不像报告：

```text
可以
先别冲
看看二手
亏损封顶
能出掉就行
感觉风险不大[旺柴]
```

---

## 安装

你可以直接让 Agent 自己装：

```text
帮我安装这个 skill：https://github.com/ninjaz0/campus-optimizer-perspective
```

### 手动安装

```bash
git clone https://github.com/ninjaz0/campus-optimizer-perspective ~/.claude/skills/campus-optimizer-perspective
```

不同宿主的推荐路径：

| 宿主 | 路径 |
|------|------|
| Claude Code | `~/.claude/skills/campus-optimizer-perspective` |
| Codex | `~/.codex/skills/campus-optimizer-perspective` |
| OpenClaw | `~/.openclaw/workspace/skills/campus-optimizer-perspective` |

---

## 使用

安装后，可以这样触发：

```text
用校园优化者视角看看
性价比角度想想
短句务实一点
campus optimizer
工具优先想想
```

退出角色：

```text
退出
切回正常
不用这个视角了
```

---

## 效果示例

### 买设备

```text
用户 ❯ 我想买个相机学摄影，预算3000，怎么选？

campus optimizer ❯ 可以
                   先看二手
                   别买太新
                   亏损要低
                   能出掉就行
                   要不先租一次
                   感觉更稳[旺柴]
```

### 学习规划

```text
用户 ❯ 我想学一个新技术，但不知道能不能坚持。

campus optimizer ❯ 先别报班
                   找个教程
                   做三天
                   能做再说
                   不行就算了
                   成本别拉满[旺柴]
```

### 宿舍沟通

```text
用户 ❯ 室友总是不打扫卫生，我该怎么办？

campus optimizer ❯ 直接说
                   别阴阳
                   定个表
                   一人一天
                   不行就拍照
                   规则比吵架好[旺柴]
```

---

## 项目结构

```text
campus-optimizer-perspective/
├── SKILL.md                         # skill 入口和核心规则
├── README.md                        # GitHub 展示和安装说明
├── test-prompts.json                # 公开测试提示
└── references/
    └── research/
        ├── 01-writings.md           # 匿名兴趣与投入模式
        ├── 02-conversations.md      # 匿名价值观与沟通模式
        ├── 03-expression-dna.md     # 公开表达 DNA
        ├── 04-external-views.md     # 匿名社交协作模式
        ├── 05-decisions.md          # 公开决策启发式
        └── 06-timeline.md           # 脱敏边界与非时间线说明
```

---

## 隐私处理

这个仓库是公开版，不包含原始私人资料。

已移除或泛化：

- 真实姓名、昵称和可识别身份
- 学校、城市、班级、社团、群名
- 联系人、家人、朋友、关系推测
- 精确日期、行程、账户、投资和设备细节
- 聊天数量、群聊排名、活跃天数等可反推身份的数据
- 本地文件路径和原始数据来源位置
- 私人聊天原文

公开版只保留抽象后的行为模式、表达规则和决策框架。

---

## License

MIT
