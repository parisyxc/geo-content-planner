# 05 · Tracking & KPI｜追踪与衡量

Read this when running **Step 4 · Monthly Track & Optimization**. It covers the dual-KPI architecture, metric definitions, citation attribution classes, the bridge between the two KPI families, leading vs lagging discipline, double/drop rules, and dashboard structure.

## Contents

1. [Why two KPI families, and only two](#1)
2. [KPI 1 · GEO layers](#2)
3. [KPI 2 · Platform funnel](#3)
4. [Citation attribution classes](#4)
5. [The bridge: Citation Source × Funnel](#5)
6. [Leading vs lagging discipline](#6)
7. [Double / drop decision rules](#7)
8. [Dashboard structure](#8)
9. [Feeding results back into next month](#9)

---

<a name="1"></a>
## 1. Why two KPI families, and only two｜为什么只有两个 KPI

Multi-metric sprawl is the most reliable way to lose executive attention. Two KPI families, each with its own closed loop:

- **KPI 1 · GEO coverage** — is the AI recommending us, for the right reason, with real evidence behind it?
- **KPI 2 · Platform conversion** — is each platform moving people down its funnel?

Everything else — individual save rates, share rates, referral sessions, ROI ratios — becomes a **process metric**: tracked internally, used for diagnosis, kept out of the executive view. This is a discipline, not a preference. The moment a third headline KPI appears, the first two stop being decision-grade.

**Never report the two as one number.** They lag differently, they attribute differently, and combining them hides exactly the failure the program exists to catch: strong platform numbers with nothing citable.

<a name="2"></a>
## 2. KPI 1 · GEO layers｜GEO 三层

| Layer | The question | Metrics |
|---|---|---|
| **Brand Presence**｜品牌是否出现 | When AI makes category recommendations, are we named? | Category prompt hit rate — % of a standing prompt set where the brand appears |
| **Semantic Reason**｜推荐理由是否对 | Is the reason it gives our north star attribute? | North-star semantic match rate — % of mentions where the stated reason maps to a defined proof angle |
| **Citation Support**｜引用来源是否支撑 | Do the cited sources actually substantiate that reason? | Citation source count · citation quality (authority class) · citation content fit |

**Building the prompt set.** Standing prompts should mirror the Core Queries from Step 1 plus a layer of pure category prompts ("best {category} for {situation}", "what should I look for in {category}"). Freeze the wording — changing prompts between months destroys comparability. Run each prompt across the engines that matter for the market, on a fixed schedule, and log the full answer text, not just whether the brand appeared. The answer text is what lets you score Layer 2 and identify Layer 3 sources.

**Scoring Layer 2 honestly.** A mention with a generic reason ("popular option", "widely available") is a Layer 1 hit and a Layer 2 miss. Only count Layer 2 when the stated reason maps to a proof angle you actually defined in Step 0. This distinction is what turns the dashboard into a content brief — every Layer 2 miss names a specific angle that needs more evidence.

<a name="3"></a>
## 3. KPI 2 · Platform funnel｜平台四层漏斗

| Layer | Meaning | Metrics |
|---|---|---|
| **L1 Awareness** | Is content reaching the target audience? | Reach, views, impressions, organic share |
| **L2 Engagement** | Are users interacting, saving, sharing? | Save rate, share rate, comments, completion rate |
| **L3 Consideration** | Are users entering a decision state? | Profile visits, link clicks, product page visits, subscribes, follows, comparison engagement |
| **L4 Conversion** | Is business outcome moving? | Traffic, conversion rate, assisted conversion, ROI |

**L3 is the diagnostic layer.** "I'll come back to this" signals — save, subscribe, follow — predict purchase intent better than "I agree with this" signals like like and share. Where a save-to-share ratio is available, it is a useful single indicator of whether content is producing utility or just agreement; rising ratio means the content is being treated as a resource.

**Diagnose to a specific transition, never to an aggregate.** "Conversion is down" is not a finding. "L2→L3 transition rate fell while L1 and L2 held" is a finding, and it names the fix: the content is resonating but not producing utility, so ship savable decision content. Every platform verdict should name the weakest *transition*, not the weakest *number*.

<a name="4"></a>
## 4. Citation attribution classes｜引用来源归因

When an AI cites a source, classify it. This is what lets you say what your work actually caused.

| Class | What it is | Whose credit | How to use it |
|---|---|---|---|
| **External authority** | Independent standards bodies, professional associations, encyclopedic references, peer-reviewed sources | Nobody's — it's the field's | Cite it in your own AUs to raise their authority signal |
| **Brand owned** | The brand's own site — blog, FAQ, product pages, structured data | The brand's SEO/content team | Cite it and link to it; it strengthens both surfaces |
| **Brand earned** | Third-party placements the brand secured — PR, sponsored reviews, partner content, creator video | The brand's PR/partnership team | Reference it where genuinely relevant; don't over-lean, engines discount promotional density |
| **Social / community** | Forum answers, community discussion, platform content produced by this workstream | **This workstream's, directly** | This is the self-evidencing metric — track it as its own line |

**`Social citations ÷ total citations`** is the single clearest measure of what a social GEO workstream contributes. Report it separately from overall GEO movement, because overall movement is confounded by the brand's SEO, PR and paid work.

The corollary is a useful piece of realism: when the AI cites brand-owned or brand-earned sources for the right reason, that is still a win for the brand's north star — just not one this workstream should claim. Distinguishing them builds credibility faster than claiming everything.

<a name="5"></a>
## 5. The bridge: Citation Source × Funnel｜两个 KPI 的桥

Read separately, the two KPI families produce one of two useless states: *"great platform numbers but nothing citable"* or *"GEO is rising and we can't say which platform earned it."* Cross them on Query ID.

At month end, answer both questions per platform simultaneously:

| Platform | Query ID / AU ID | Coupling | GEO contribution (KPI 1) | Funnel health (KPI 2) | Verdict |
|---|---|---|---|---|---|
| *search platform* | `{ID}` | Heavy | Became a citation source for this query? | Did click rate patch the L1–L2 weakness? | Both good → double. Funnel good, no citation → structure is not extractable; re-frame the AU. |
| *discovery platform* | N/A or campaign-tagged | Light | **Not in scope for KPI 1** | Views / engagement / completion on target? | Judge on KPI 2 alone. Absence of citation is not failure. |

**Attribution must respect coupling level.** Heavy and Medium content enters both KPI families. **Light content enters KPI 2 only** and carries no citation target. Without this rule, brand films, key visuals, trend participation, street interviews and mandatory campaign shipping all get scored as failures for not producing something they were never designed to produce — and the in-house team correctly stops trusting the dashboard.

**The most valuable cell in this table** is "funnel good, no citation." It means the content performs but has no extractable structure. That is a framing problem in the AU, and it is fixable next month without changing the topic, the platform or the budget.

<a name="6"></a>
## 6. Leading vs lagging discipline｜领先与滞后指标

AI citation moves on a **weeks-to-months lag.** Content published in month one may not appear in an engine's answers until month three, and semantic reason shifts lag further than presence.

**Read monthly:** leading indicators only — proof-angle corpus density (how many pieces of evidence exist per angle), citation surfaces shipped (how many Heavy assets went live), early mentions, and platform funnel metrics.

**Read quarterly:** the real Layer 1 and Layer 2 movement — presence rate and semantic match rate trends.

**Say this before month one, not after.** Setting the lag expectation up front is what prevents the program being judged a failure on its first report. A month-one report showing no semantic shift is a *correct* report, and the leading indicators are what demonstrate the work happened.

<a name="7"></a>
## 7. Double / drop decision rules｜加倍与放弃

Run these at month end and write the verdict into the dashboard. A dashboard that reports numbers without verdicts gets skimmed; a dashboard that ends each view with a decision gets read.

| Observation | Decision |
|---|---|
| AI mentions us, but the reason is generic or wrong | Strengthen evidence on that query — more proof-angle density, more authority structure, more surfaces |
| AI recommends a competitor for our target query | Analyze which sources it cites and why; match the scenario with better evidence, or take a different angle on the same situation |
| No brand is stably recommended for a query | Keep reinforcing — it's an open field and the cheapest win available |
| A query shows weak resonance and low citation potential | Demote or drop next month. Sunk listening cost is not a reason to keep it. |
| An AU type is consistently adopted by AI or performs on platforms | Double down cross-platform |
| Heavy content performs on platform but never gets cited | Re-frame the AU structure — the topic is right, the extractability isn't |
| Light content underperforms on platform metrics | Judge and adjust on platform terms only |
| Platform L2→L3 transition is the weakest link | Ship savable decision content — this is what proof angles do best |
| A single format repeatedly produces hit content | Capture it in a format library and replicate it deliberately rather than hoping it recurs |

**Escalation rule.** A single failed action is a monthly drop — it does not touch strategy. But when multiple actions against the *same* proof angle or the *same* pillar fail repeatedly, that is a signal the strategic assumption is wrong, and it should be escalated to a quarterly strategy review rather than absorbed silently as another monthly drop.

<a name="8"></a>
## 8. Dashboard structure｜仪表盘结构

Two dashboards, read in sequence, each ending in a verdict.

**Dashboard 1 · GEO health**

| View | Contents |
|---|---|
| Presence | Prompt hit rate by query cluster, trend line, competitor comparison |
| Reason | Semantic match rate; breakdown of which proof angles are landing and which aren't |
| Sources | Citation counts by attribution class; social share of total |
| Gaps | Queries with no coverage, queries where a competitor owns the answer, angles with thin evidence |

**Dashboard 2 · Platform conversion funnel**

| View | Contents |
|---|---|
| Per-platform L1→L4 | Stage values and stage-to-stage transition rates |
| Weakest link | The named weakest transition per platform |
| Contribution | Which content types drove which layer |
| Verdict | Double / drop per format and per platform |

**Every view ends with a plain-language "what this means" line.** Not a number restated — a sentence a non-specialist executive can act on. This single formatting rule does more for whether a dashboard gets used than any amount of chart work.

**Keep strategic vocabulary out of the executive view.** Pillars, personas, coupling levels, encoding layers and AU taxonomy all belong in the underlying trace, not on the top-level dashboard. The executive layer sees goal, action, data, decision. Everything else is available on request.

<a name="9"></a>
## 9. Feeding results back into next month｜反哺下月

The loop only closes if month four's Query Finding is shaped by month three's results. Four feedback paths:

**High-comment questions → next month's queries.** Comments on your own content are free listening, and they're pre-qualified by the fact that these people already engaged with your framing. Harvest them monthly and feed them into Step 1.

**Gap analysis → next month's priorities.** Sort every tracked query into four states: *covered and winning* (maintain), *covered but losing* (optimize the evidence), *uncovered and open* (build), *winning without effort* (understand why and replicate). The second and third categories set next month's production priorities.

**Hit-format capture → next month's formats.** Collect the month's highest-performing content across platforms and identify the *format* pattern, not the topic. Replicate the format deliberately. This is algorithm-driven rather than taste-driven, and it is far more reliable than subjective judgment about what looks good.

**Failed angles → the north star decomposition.** If a proof angle repeatedly fails to land — no citations, no engagement, no resonance — the problem may be the angle rather than the execution. Revisit the Step 0 decomposition quarterly with this evidence in hand.

**Cold start.** In month one there is no feedback loop yet. Skip these steps rather than inventing inputs for them. Fabricating a gap analysis from no data produces confident, wrong priorities — and month two will have real data anyway.
