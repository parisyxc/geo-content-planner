# GEO Content Planner — Tool Spec

> 把完整版 `social-geo-content-planner` skill 框成一个 **input → output 的工具**，公开呈现为 **GEO Content Planner**。
> 引擎不变（`SKILL.md` 月度四步闭环 + 5 份 references + 3 个 assets 模板）。改的是外壳、命名、I/O 契约。
> 定位：tool-led · "帮你做"（直接产出可发布的 GEO 内容计划），不是卖咨询过程。

---

## 1 · 是什么（一句话）

**GEO Content Planner** —— 输入品牌 / 目标人群 / 平台定位三件事，输出一套让 AI 搜索（ChatGPT / Perplexity / Gemini）愿意推荐你的月度内容计划：值得赢的 Query、可被 AI 直接引用的 Answer Unit、以及每条内容放到哪个平台。把社媒产出从一次性 campaign 流量，转成可被 AI 长期识别、引用、推荐的**证据型资产**。

## 2 · Input → Output 契约

**INPUT（品牌需提供的三项）**

| # | 输入 | 含义 | 缺失时 |
|---|------|------|--------|
| 1 | **Brand** | 品牌名、品类、当月主推产品 | Blocker，必问 |
| 2 | **Consumer target** | 目标人群 + 真实处境（是场景不是人口标签） | Blocker，只给「25-40 女性」不够，要追问处境 |
| 3 | **Platform positioning** | 哪些平台、各自在矩阵里的角色 | 非 blocker，可用默认角色库提案后确认 |

可选升级项：上月漏斗数据、营销日历/campaign 节点、竞品集、已有 SEO 关键词、可引用的专家/临床来源。

**OUTPUT（交付的三项产出，各有模板）**

| # | 产出 | 内容 | 模板 |
|---|------|------|------|
| 1 | **Query Map** | Core × Sub 分层 query，每条带真实 listening 证据、优先级、就绪度 | `assets/query-map-template.csv` |
| 2 | **Answer Units** | AI 可整段抽取的答案模块 | `assets/answer-unit-template.md` |
| 3 | **Platform Distribution** | 每平台月度计划：数量 · 帖级 angle · 格式 · 漏斗角色 · 引用面 | `assets/platform-monthly-plan-template.md` |

## 3 · 月度四步闭环（引擎）

```
Step 0 Intake（语义北极星）→ Step 1 Query Finding → Step 2 Answer Unit → Step 3 Distribution → Step 4 Monthly Track ↻
```

- **Step 0 · 语义北极星**：一句话「让 AI 理解：{品牌} 是 {品类} 里 {某属性} 的选择」，再拆成 5–8 个 proof angle。**最重要、最常被跳过**——下游每个判断都对着这一句话解析。
- **Query ID 是全链路脊柱**：`{PERIOD}-{LINE}-{THEME}-NN` → 一个 Query → 多个 AU → 多平台分发；月末每个引用/漏斗数据都挂回这个 ID。
- **Heavy / Medium / Light 耦合分级**：不是每条内容都塞完整 AU；Light（TVC/KV/趋势/强制 campaign）只做卫生优化，且**只进平台漏斗 KPI，不背引用指标**——保护叙事内容不被误判。

## 4 · 这个工具的性质（和另外两个对比）

| | **GEO Content Planner** | Cultural Brand Analyzer | Product Video Studio |
|---|---|---|---|
| 帮你 | **做**（内容计划） | **想**（文化分析） | **做**（创意生产） |
| 输出 | Query Map / AU / 分发计划 | 6 段文化分析 | 场景→冲突→脚本→分镜 |
| 有无运营层 | **有**（Step 4 月度双 KPI 追踪，recurring） | 无（一次性） | Step 4 手动触发 |

它是"帮你做"里最"运营化"的一个——不只出一次计划，而是一套可每月复跑的操作系统。

## 5 · 纪律必须保留（这是它的价值，不能稀释）

- **意图研究，不是关键词研究**——Step 1 找的是真实用户的决策问题，且每条保留证据。
- **答案优先，品牌其次**——AU 先帮用户判断，推荐逻辑只在答案自立之后出现。
- **每个 AU 只贡献一条证据**——不是每个 AU 重复北极星，而是各证一个不同的 proof angle。
- **GEO 是滞后信号**——月读 leading 指标（语料密度、引用面、早期 mention），季读真实语义位移；第一个月看不到位移是正常的。
- **首月要轻**——L1 单条最高优先品线、聚成 8–15 个 Core Query、证据强于数量。

## 6 · 命名与结构

- **公开工具名**：`GEO Content Planner`（按成果命名）。skill 内部 `name: social-geo-content-planner` 保持不变（引擎的规范名）。
- **引擎**：`geo-content-planner-skill/`（`SKILL.md` + `references/01–05` + `assets/` 三个模板）——完整自包含，无外部依赖。
- **已取代**：旧的 GEO 草稿工作流与旧的 Steps 1-2 query 引擎已被本完整版完全吸收，标记废弃、待删除；更早的 PDCA 版本亦已 superseded。（旧版含客户校准的 worked-example，仅内部保留、不发布。）
- **公开 demo**：用**虚构品牌 Aria**（敏感肌护肤）跑一遍 Step 0 → 三项产出（见 `geo-content-planner-demo.html`）——不涉及任何客户产品。
- **隐私**：客户 worked-example 仅内部参考，不进公开仓库、不显示客户名。

## 7 · 与轻量化目标的关系

- 公开呈现为 **"工具名 → input（3 件事）→ output（3 份产出）→ demo case → 用它"**。
- registry：`geo-content-planner`（general/tool，覆盖 S6/S7/S8），指向本 spec + skill + demo；旧 id 全部 superseded。
- 与 Cultural（帮你想）、Video Studio（帮你做·创意）构成三个成熟 tool+demo；结构一致、可复制。
