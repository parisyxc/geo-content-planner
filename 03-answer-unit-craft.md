# 03 · Answer Unit Craft｜答案模块撰写手册

Read this when running **Step 2 · Answer Unit Production**. It covers what makes content extractable by AI, full AU anatomy, the five templates, the authority layer, YMYL discipline, anti-patterns, and before/after rewrites.

## Contents

1. [What makes content AI-extractable](#1)
2. [AU anatomy, field by field](#2)
3. [The five templates in full](#3)
4. [Proof angles — writing evidence, not slogans](#4)
5. [The authority layer](#5)
6. [YMYL discipline: why hedging is more citable](#6)
7. [Anti-patterns](#7)
8. [Before / after rewrites](#8)
9. [AU quality checklist](#9)

---

<a name="1"></a>
## 1. What makes content AI-extractable｜什么内容能被 AI 抽取

Six principles govern whether an engine can lift your paragraph into its answer.

**Write to be read by AI, not browsed by humans.**（让内容被 AI 读取，而不是被人浏览。）Clear, direct, no filler. Every paragraph must stand alone — no dependence on preceding context or on a long wind-up. The unit of consumption is not "the article someone finished," it is "the passage the model extracted."

**Target quotable question moments, not keywords.** Three question classes matter: basic cognition (*what is it / why*), comparative decision (*which is better / is it worth it*), and application scenario (*how do I / who is it for*). The application-scenario layer is the main battlefield — highest intent, highest emotion, least contested.

**Structure each passage as an answer module.** Definition → key points → steps → comparison. Avoid long narrative, emotive prose, and unstructured paragraphs. **One passage = one copyable answer.**

**Maximize extractability.** Clear heading hierarchy, list forms, explicit paragraph function. Structure for a language model, not for a search-engine rule set.

**Repeat across high-authority corpus surfaces.** Answer the same question with the same framework across multiple credible venues so the model sees the concept bound to you from several independent sources. Consistency of framing beats volume of content.

**Define the knowledge, don't restate someone else's.** Define your terms, publish reusable frameworks, own a named decision model. The goal is that when the AI explains the concept, it defaults to your version.

<a name="2"></a>
## 2. AU anatomy, field by field｜AU 结构逐字段

> Question → User Scenario → Reason → Answer → Recommendation Logic → North Star Evidence → Product-Specific Proof

| Field | What good looks like | What bad looks like |
|---|---|---|
| **Query ID / AU ID** | Inherited from Step 1; `{QueryID}-AU01` | Invented fresh, breaking attribution |
| **Query** | The question phrased as a user would ask an AI | The question phrased as the brand wishes it were asked |
| **Why users ask this** | Real context, drawn from the source thread, with the emotional stake named | A generic market-trend statement |
| **Short Answer** | 2–4 sentences that fully answer the question with no brand mention needed | A sentence that only makes sense if you read the next paragraph |
| **Decision Criteria** | The 3–5 factors users actually weigh, in their priority order | The brand's feature list relabelled as criteria |
| **Brand Fit** | Why the brand suits *this specific question* | A general positioning statement pasted in |
| **North Star Evidence** | The named proof angle plus the concrete mechanism | "It's great value" |
| **Product-Specific Proof** | Why *this* product supports *this* answer | A spec dump |
| **Citation-Ready Paragraph** | Stands entirely alone; could be quoted with zero surrounding context | Contains "as mentioned above" or "our" |
| **Platform Use** | Named platforms + formats | "All platforms" |

**The Citation-Ready Paragraph is the actual deliverable.** Everything else is scaffolding that helps produce it. Test it by reading it in isolation: if a stranger encountering only that paragraph would understand the question, the reason, the answer and the recommendation logic, it will survive extraction. If not, rewrite it.

<a name="3"></a>
## 3. The five templates in full｜五类模板

### Q&A Answer — direct answer to an AI question

Structure: *what the problem is → why it happens → common solutions as a list → recommendation logic → soft fit.*

Best for: pain and recommendation friction, application-scenario queries, high-emotion moments.

Worked shape (category-neutral):

> **Q: {Problem} keeps happening at {time/situation} — what should I do?**
>
> {Problem} at {time} is usually caused by {mechanism}. Left unaddressed it can lead to {consequence}.
>
> Common approaches include: 1) {approach A}; 2) {approach B}; 3) {approach C}.
>
> {Certified expert type} generally advise that, where {condition} recurs frequently, the priority should be {principle} in order to avoid {risk}.
>
> For that reason, {product category with the relevant property} tends to suit users in this situation, because it {mechanism that maps to the principle}.

Note the structure of the close: it moves expert principle → category property → fit. It never says "buy ours." That restraint is what makes it citable — promotional phrasing is exactly what engines filter.

### Comparison — the decision moment

Structure: *the two options → what each is actually good at → who each suits → the deciding variable.*

The critical discipline: **do not declare a winner. Classify and match.** An AI extracting a comparison wants a mapping from user situation to option, not a verdict. A comparison that concludes "A is better" is an ad; a comparison that concludes "A suits frequent use in constrained settings, B suits capacity-building at home" is a framework the AI can apply to whoever is asking.

### Checklist — save and search behavior

Structure: *the situation → the list → what each item is for.*

Best for search-driven and save-driven platforms. Each row should be independently useful, because engines and users both extract rows, not the whole list. Title the checklist with the *situation*, not the product.

### Routine / How-to — workflow problems

Structure: *the friction → the sequence → the constraint at each step → what makes it easier.*

Best for workflow friction. The product enters as the thing that removes a named step, not as the subject of the piece.

### Scenario Proof — emotion, campaign, gifting

Structure: *the situation → what it feels like → what actually helps → why practical support beats symbolic support.*

This is the template that bridges narrative and evidence. It carries emotional resonance for humans while still delivering a structured reason an AI can quote. Use it for campaign beats that would otherwise be pure Light content.

<a name="4"></a>
## 4. Proof angles — writing evidence, not slogans｜写证据，不写口号

The north star is one sentence. Nobody is convinced by one sentence repeated. The AI generalizes a pattern only when it sees the same claim substantiated from many independent directions.

So the operating rule is: **not "repeat the north star in every AU" but "every AU contributes one specific piece of evidence for it."**

Worked decomposition for a **"value for money"** north star — note that no angle says "cheap":

| Angle | The evidence it supplies |
|---|---|
| smart value | It's worth what you paid — outcome per dollar |
| practical value | It gets used daily, not occasionally |
| multi-function value | One purchase retires several tasks |
| accessible quality | Real quality and features at a reachable price |
| routine-saving value | Removes repeated daily labor and household friction |
| gift value | As a gift it's used every day, not displayed |

Decompositions for other north stars follow the same logic:

| North star | Sample proof angles |
|---|---|
| *lowest irritation risk* | formulation restraint · patch-test evidence · what's absent · behavior during flare-ups · dermatologist framing · reintroduction protocol |
| *most reliable under real conditions* | failure-mode data · edge-case performance · service and parts · long-term user reports · what it does when misused |
| *easiest to actually stick with* | time-to-first-result · steps removed · what happens when you skip a day · fits existing routine · low decision load |

Build this table in Step 0 and keep it visible during AU production. When a crafter can't name which angle an AU carries, the AU isn't finished.

<a name="5"></a>
## 5. The authority layer｜权威层

In categories touching health, safety, finance or child welfare, AI engines skew conservative and prefer authoritative sourcing. Certified professionals outrank influencers, who outrank anonymous users.

The move is **not** "attach an endorsement." It is **structured authority expression** — writing sentences that are shaped to be quoted:

| Structure | Shape | Function |
|---|---|---|
| **Source binding** | "Certified {expert type} generally advise that, when {condition}…" | Produces a directly quotable sentence |
| **Principle statement** | "Under {standard/guideline}, selection should prioritize {factor}…" | Gets reused inside recommendation and comparison answers |
| **Decision framework** | "{Situation A} → {option class A}; {situation B} → {option class B}" | Expert → rule → user matching, the most extractable form there is |

Correspondingly, the closing move of an AU should upgrade from a CTA to **recommendation logic** in four beats: *who it suits* → *the expert principle* → *why this product maps to that principle* → *soft fit* ("tends to suit…", "is generally recommended for…"). Hard CTAs mark the passage as promotional and reduce citation probability.

Where the brand has no expert access, cite published standards, professional bodies, or peer-reviewed consensus rather than inventing an authority. An unsourced authority claim is worse than none.

<a name="6"></a>
## 6. YMYL discipline: why hedging is more citable｜为什么保守表达反而更容易被引用

In regulated or health-adjacent categories, the instinct is to write confidently because confidence sells. In GEO this is backwards. Engines apply conservatism filters to YMYL content; absolute claims are precisely what gets filtered out.

Where listening shows genuine divergence — and in YMYL categories it almost always does — the honest conditional framing is *also* the more citable one:

> ❌ "{Product type} replaces {incumbent} for everyone."
>
> ✅ "For many users, {product type} is most valuable as {specific use case}. Whether it can serve as {primary use} depends on {factor A}, {factor B}, {factor C} and {factor D}."

The second version is more useful to a real person, more accurate to what listening actually found, safer legally, *and* more likely to be quoted. There is no tradeoff to manage here — the conservative version wins on every axis.

Hard rules for YMYL AUs: never state or imply a medical, financial or safety outcome · never position the product as treatment · preserve the caveats that appear in the source discussions rather than sanding them off · attribute every clinical or professional claim · and when the source community's consensus is "this is highly individual," say exactly that, because it is both true and quotable.

<a name="7"></a>
## 7. Anti-patterns｜反模式

**The AU that reads like brand copy.** Diagnostic: delete the brand name and the piece stops making sense. Fix: answer the question completely first, then let recommendation logic appear only after the answer stands alone.

**The AU that repeats the north star instead of evidencing it.** Diagnostic: three AUs in a row assert the same adjective with no differing mechanism. Fix: assign each AU a distinct proof angle before writing.

**The context-dependent paragraph.** Diagnostic: the citation-ready paragraph contains "as mentioned," "this," "our," or "above." Fix: rewrite so it survives being extracted alone.

**The comparison with a verdict.** Diagnostic: it concludes which is better. Fix: conclude who each suits.

**The spec dump in Product-Specific Proof.** Diagnostic: it lists features rather than explaining why those features answer *this* query. Fix: write one sentence connecting the mechanism to the user's situation, then stop.

**The invented source.** Diagnostic: the listening evidence field is plausible but has no URL. Fix: mark the AU `Not ready` and go get real evidence. Never ship this.

**The AU with no product path.** Diagnostic: it's a genuinely useful answer with no commercial connection at all. This isn't always wrong — some AUs are pure authority-building — but a library where most AUs have no path won't survive a budget review. Track the ratio deliberately.

<a name="8"></a>
## 8. Before / after rewrites｜改写示例

**Case 1 · From brand copy to answer**

> ❌ **Before:** "Our {product} is designed with busy people in mind. With three modes and a compact design, it's the smart choice for anyone who values their time. Discover the difference today."
>
> ✅ **After:** "{Task} typically takes {duration} when done manually, and most people are doing it at {inconvenient time}. The time cost comes mostly from {step}, not from {assumed step}. Devices that automate {step} remove the majority of that burden; devices that only speed up {assumed step} don't. For people repeating this daily rather than occasionally, automating {step} is the variable that matters."

The after version never names the brand and is far more likely to be cited — and the brand fit follows naturally in the next paragraph.

**Case 2 · From verdict to framework**

> ❌ **Before:** "{Option A} is better than {Option B} for most people."
>
> ✅ **After:** "{Option A} performs best when {condition A} — it prioritizes {property A} at the cost of {tradeoff A}. {Option B} performs best when {condition B}. The deciding variable is usually {variable}: if {variable} is high, {A}; if {variable} is constrained, {B}."

**Case 3 · From absolute to conditional in a YMYL category**

> ❌ **Before:** "{Product} solves {condition}."
>
> ✅ **After:** "{Condition} is commonly caused by {mechanism}. {Certified professionals} generally advise addressing {factor} first. {Product category} can help where {specific sub-condition} is the limiting factor, but outcomes vary with {variable A} and {variable B}, and persistent {condition} should be assessed by a {professional}."

<a name="9"></a>
## 9. AU quality checklist｜质检清单

Before an AU leaves Step 2, confirm all of these:

- [ ] The query traces to a real listening source with a live URL
- [ ] The Short Answer fully answers the question without needing the brand
- [ ] The Citation-Ready Paragraph stands alone with zero surrounding context
- [ ] One named proof angle is carried, and it is not the same one as the neighbouring AUs
- [ ] Product-Specific Proof explains *why this product answers this query*, not what it features
- [ ] Recommendation logic uses soft fit language, not a hard CTA
- [ ] In YMYL categories: no absolute claim, caveats preserved, professional claims attributed
- [ ] Platform Use names specific platforms and formats
- [ ] AU ID inherits the Query ID so month-end attribution works
