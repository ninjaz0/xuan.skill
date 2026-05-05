# xuan.skill
### *把 xuan 装进你的 AI 里。问事、砍价、劝退、先看二手。*

[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![Codex](https://img.shields.io/badge/Codex-Skill-black)](https://github.com/openai/codex)
[![Language](https://img.shields.io/badge/Language-中文-red)](README.md)
[![Persona](https://img.shields.io/badge/Persona-xuan.skill-4B5563)](SKILL.md)

朋友问：

> 这东西能买吗？

xuan.skill：

```text
先别冲
看二手
能出掉吗
亏多少
感觉可以试[旺柴]
```

朋友又问：

> 要不要报这个课？

xuan.skill：

```text
先别报
找免费教程
做三天
还想学再说
不想学就省钱[旺柴]
```

懂了吧。

这不是一个“人生导师型”Skill。

这是一个“先把你从冲动消费边上拉回来，然后顺手帮你找个更便宜方案”的 Skill。

---

## 这是什么

`xuan.skill` 是一个给朋友玩的 persona skill。

主要功能：

- 朋友上头时：`先别冲`
- 朋友纠结时：`要不试小版`
- 朋友想买贵东西时：`看看二手`
- 朋友要写长篇大论时：`太正式了`
- 朋友问技术方案时：`有没有现成的`
- 朋友内耗半天时：`算了 先做`

高情商说法：

> 工具优先、风险有界、舒适驱动、性价比导向。

低情商说法：

> 别一上来拉满预算。

---

## 适合问什么

### 适合

- 这个设备值不值得买
- 这个课要不要报
- 学一个新东西怎么开始
- 室友不干活怎么办
- 一个活动要不要去
- 这个方案有没有更省事的做法
- 我现在很纠结，能不能骂醒我一下，但别太正式

### 不太适合

- 需要专业医生、律师、财务顾问的问题
- 需要官方确认的流程
- 想听 3000 字人生大道理
- 想被无条件鼓励“冲就完事了”

最后一个尤其不适合。

它大概率会说：

```text
别冲
先查
不急[旺柴]
```

---

## 安装

你可以直接让 Agent 自己装：

```text
帮我安装这个 skill：https://github.com/ninjaz0/xuan.skill
```

手动安装也行：

```bash
git clone https://github.com/ninjaz0/xuan.skill ~/.claude/skills/xuan.skill
```

不同宿主放这里：

| 宿主 | 路径 |
|------|------|
| Claude Code | `~/.claude/skills/xuan.skill` |
| Codex | `~/.codex/skills/xuan.skill` |
| OpenClaw | `~/.openclaw/workspace/skills/xuan.skill` |

装完以后，重启一下对应的 Agent。

不行就再装一遍。

还是不行就先别急。

怎么说，可能路径放错了[旺柴]

---

## 怎么玩

触发方式随便挑：

```text
用 xuan 的视角看看
xuan 会怎么看？
xuan.skill
性价比角度想想
工具优先想想
短句一点
别写小作文
```

退出角色：

```text
退出
切回正常
不用这个视角了
```

---

## 实战样例

### 买相机

```text
用户 ❯ 我想买个相机学摄影，预算3000，怎么选？

xuan ❯ 可以
       先看二手
       别买太新
       亏损要低
       能出掉就行
       要不先租一次
       感觉更稳[旺柴]
```

### 报课

```text
用户 ❯ 我想学一个新技术，但不知道能不能坚持，要不要报课？

xuan ❯ 先别报
       找个教程
       做三天
       能做再说
       不行就算了
       成本别拉满[旺柴]
```

### 宿舍卫生

```text
用户 ❯ 室友总是不打扫卫生，我该怎么办？

xuan ❯ 直接说
       别阴阳
       定个表
       一人一天
       不行就拍照
       规则比吵架好[旺柴]
```

### 冲动消费

```text
用户 ❯ 我现在很想买一个贵东西。

xuan ❯ 先放购物车
       明天再看
       查下二手价
       能不能退
       先别上头
       你不急[旺柴]
```

---

## 技能点

| 技能 | 表现 |
|------|------|
| 性价比雷达 | 贵了就会皱眉 |
| 二手优先 | 新的不是不能买，先看亏多少 |
| 工具优先 | 能用现成的就不手搓 |
| 小额试错 | 先试小版，别开局梭哈 |
| 短句输出 | 拒绝小作文，从我做起 |
| 舒适驱动 | 不舒服就换，不硬熬 |

---

## 项目结构

```text
xuan.skill/
├── SKILL.md                         # skill 入口和核心规则
├── README.md                        # 你正在看的这个东西
├── test-prompts.json                # 测试提示
└── references/
    └── research/
        ├── 01-writings.md           # 兴趣与投入模式
        ├── 02-conversations.md      # 价值观与沟通模式
        ├── 03-expression-dna.md     # 表达 DNA
        ├── 04-external-views.md     # 社交协作模式
        ├── 05-decisions.md          # 决策启发式
        └── 06-scope.md              # 适用范围
```

---

## 友情提示

这玩意儿主要给朋友玩。

真要做重大人生决策，还是多查资料，多问真人，多睡一觉。

但如果你只是想问：

```text
这个东西值不值得买
```

那它可能真的挺有用。

毕竟第一反应不是“买”，而是：

```text
先看二手[旺柴]
```

---

## License

MIT
