# 02 · Social Listening Playbook｜社群倾听手册

Read this when running **Step 1 · Query Finding**. It covers where to listen, how to search, how to read evidence, the friction taxonomy, full Query Map field definitions, and the clustering pass that closes the step.

## Contents

1. [Why Reddit (and what to use instead)](#1)
2. [Finding the right communities](#2)
3. [Search patterns that surface queries](#3)
4. [The friction taxonomy](#4)
5. [Query Map field definitions](#5)
6. [Evidence standards — what makes a query "sourced"](#6)
7. [Priority scoring](#7)
8. [Core Query Clustering, in detail](#8)
9. [Track 1A vs 1B execution detail](#9)
10. [Multi-line registry and dedupe](#10)
11. [Common failure modes](#11)

---

<a name="1"></a>
## 1. Why Reddit (and what to use instead)｜为什么用 Reddit

Reddit is the primary listening source for most Western categories because it uniquely concentrates:

- **Scenario-rich real problems** — people describe the whole situation, not just the product
- **Emotionally dense phrasing** — the exact words users would type into an AI
- **Natural-language question forms** — titles are already close to prompts
- **High volume of decision content** — comparisons, complaints, help-seeking, experience sharing
- **Long-tail scenarios** — the specific situations that generic keyword tools never surface

It is also, conveniently, a surface AI engines cite heavily.

**Substitutes and supplements by market/category.** Where Reddit is thin, listen in the equivalent decision venue and apply the identical method: Xiaohongshu (China consumer), Quora (broad EN), category-specific forums, Facebook Groups, Discord servers, TikTok and YouTube comment sections on high-view category videos, app-store and marketplace reviews (especially 2–3 star, which are the most diagnostic), and the brand's own customer-service transcripts and FAQ logs.

**Do not skip listening because the category "doesn't have a Reddit."** Every category has a place where people ask each other before they buy. Find it.

<a name="2"></a>
## 2. Finding the right communities｜找对社群

Work outward in three rings:

**Ring 1 · Category subs** — where the product itself is discussed. Usually obvious, often small, highest signal density. These give you comparison and worth-it queries.

**Ring 2 · Situation subs** — where the *user's life stage or condition* is discussed, not the product. Larger, more emotional, and the source of the best L2/L3 queries because people describe the problem before they know a product category exists. This ring is where intent-stage queries live.

**Ring 3 · Adjacent-role subs** — where the *other people in the situation* talk: partners, caregivers, professionals, hobbyist adjacents. Often the richest ground for shared-responsibility, gifting and "how do I get X to help" queries that the category subs never surface.

For each candidate community, record before you rely on it: subscriber count, weekly active posting volume, self-promotion rules (many communities ban brand mentions and links outright), and whether the moderators tolerate professional/expert participation. Rules determine what is publishable later in Step 3 — check them now, not after drafting.

<a name="3"></a>
## 3. Search patterns that surface queries｜有效的搜索模式

Search each community with patterns, not with your product name. Product-name searches return existing customers; pattern searches return prospects mid-decision.

| Pattern | Surfaces | Example shape |
|---|---|---|
| `worth it` / `worth the money` | Value and justification queries | "is {category} actually worth it" |
| `vs` / `or` / `instead of` | Comparison and decision queries | "{A} vs {B} for {situation}" |
| `anyone else` / `am I the only one` | Identity and emotional friction | "anyone else feel like {failure state}" |
| `how do you` / `how do I` | Workflow and routine queries | "how do you handle {task} when {constraint}" |
| `help` / `advice` / `desperate` | High-intent pain queries | "{symptom} — advice?" |
| `regret` / `wish I knew` / `don't buy` | Risk, caveat and myth-busting queries | "things I wish I knew before buying {category}" |
| `recommendations` / `budget` / `under $X` | Purchase-ready and gifting queries | "best {category} under {price}" |
| `back to work` / `travel` / `{season}` | Long-tail scenario queries | situational constraints |

Also mine **comment sections of high-upvote threads**, not just titles. The title gives you the Core Query; the comments give you the Sub-Queries, the objections, the caveat language and the competitor set — which is where most of the actual value is.

Sort by top-of-year and top-of-all-time as well as recent. Evergreen high-upvote threads are disproportionately likely to already be AI citation sources, which makes them both a query signal *and* a competitive intelligence signal.

<a name="4"></a>
## 4. The friction taxonomy｜摩擦类型

Tag every query with one friction type. This is what makes clustering possible later, and it determines which AU template fits.

| Friction type | What it is | Best AU template |
|---|---|---|
| **pain** | An acute problem the user wants stopped | Q&A Answer, Routine/How-to |
| **workflow** | The task is possible but exhausting or badly sequenced | Routine/How-to, Checklist |
| **comparison** | Two or more viable options, unclear tradeoff | Comparison |
| **identity** | "Am I doing this wrong / am I a bad {role}" | Scenario Proof |
| **emotional** | Anxiety, guilt, exhaustion, embarrassment | Scenario Proof, Q&A with reassurance |
| **recommendation** | Explicitly asking what to buy | Q&A Answer, Comparison |
| **edge-case** | Unusual constraint the mainstream answer ignores | Q&A Answer, Checklist |

A healthy monthly map spans at least four friction types. A map that is 80% `recommendation` means you searched with product terms and only found bottom-funnel — go back to Ring 2 communities.

<a name="5"></a>
## 5. Query Map field definitions｜字段定义

Full schema in `assets/query-map-template.csv`. The purpose of this table is **not** to log queries — it is to preserve the evidence, engagement intensity and comment insight alongside each one, so priority is decided on evidence rather than taste.

| Field | Definition |
|---|---|
| **Query ID** | `{PERIOD}-{LINE}-{THEME}-{NN}`, generated this round from listening |
| **Query Layer** | `Core` / `Sub-Query` / `Dimension Note` / `Merged` / `Deleted` |
| **Core Query** | Which decision entry point this belongs to. Core rows name themselves; Sub and Note rows hang back onto their Core. |
| **Discovered Query** | The natural-language question distilled from listening |
| **Source URL** | The thread or comment |
| **Source Post Title** | Verbatim — preserves the original tone and question framing |
| **Author ID** | To judge whether this is a real, active or high-karma user |
| **Community** | Which sub/forum/group |
| **Upvotes / Karma** | Engagement magnitude, especially high-upvote threads |
| **Comment Count** | Discussion heat and resonance strength |
| **Original User Language** | Verbatim quote, preserving emotion words and scenario words |
| **Comment Evidence Summary** | High-frequency opinions, recurring complaints, advice and purchase judgments from the comments |
| **Friction Insight Summary** | The key insight behind this friction — e.g. "wants freedom but worries about {tradeoff}" |
| **Friction Type** | From the taxonomy above |
| **Situation Cluster** | Named scenario grouping, e.g. "office use", "first 30 days", "travel", "shared responsibility" |
| **Intent Depth** | `L1 awareness` / `L2 research` / `L3 decision` / `L4 purchase-ready` |
| **Product Fit** | Which line or product this maps to |
| **North Star Proof Angle** | Which proof angle from Step 0 this query can demonstrate |
| **Priority** | A / B / C |
| **AU Readiness** | `Not ready` / `Ready with caveat` / `Ready` |
| **Risk / Caveat** | Medical, regulatory, overclaim, negative-review or platform-tone risk |

<a name="6"></a>
## 6. Evidence standards — what makes a query "sourced"｜证据标准

A query is only admissible to the map if it carries a **live source URL, the verbatim title, the community, engagement numbers and at least one verbatim user quote.** A query written from intuition and back-filled with a plausible-sounding source is worse than no query — it corrupts the priority ranking and it will not survive client review.

Where a query is genuinely synthesized across several threads (legitimate, and often correct), mark it explicitly as synthesized and cite **all** contributing threads. Do not present a synthesis as a single-source finding.

Verbatim quotes should be preserved with their original emotional register, including profanity and grammatical roughness, in the internal map. That register is what tells the AU crafter how the user actually talks — it gets cleaned up on the way to publication, never before.

<a name="7"></a>
## 7. Priority scoring｜优先级判断

Beyond raw relevance, four signals should drive the A/B/C call:

- **High karma / upvotes** → group resonance, not individual complaint. Strong candidate for a Core Query.
- **High comment count** → the question provokes discussion; supports a multi-angle AU and multiple platform cuts.
- **Comments converge** → a stable recommendation logic is available; good for a definitive Q&A or checklist AU.
- **Comments diverge sharply** → excellent for comparison, decision framework, or myth-busting. Divergence is an *asset*, not a problem — it means no brand currently owns the answer.

Weight against three more factors: does this query plausibly reach purchase intent (a fascinating query with no commercial path is a C); can we actually substantiate an answer (if the brand has no evidence and no expert access, it's `Not ready`); and is any competitor already the stable cited answer (if yes, you need either a better-evidenced answer or a different angle on the same situation).

<a name="8"></a>
## 8. Core Query Clustering, in detail｜核心 query 聚类

Never hand off a flat list. Run this pass at the end of every Step 1.

**Procedure:**

1. Group raw queries by friction cluster and situation cluster (not by product).
2. Within each cluster, ask: *what is the one entry-level decision question a user would actually put to an AI here?* That is the Core Query. Usually one per cluster; two only when genuinely distinct decisions live in the cluster. **Never split to hit a number.**
3. Everything else in the cluster is either a Sub-Query (an evaluation dimension the Core AU must cover) or a Dimension Note (supplementary detail for the crafter).
4. Keep **3–5 Sub-Queries** per Core. More than five means the Core is too broad — split it or demote the excess.
5. Log Merged and Deleted rows with a reason. Audit trail matters when a client asks "what happened to the query I mentioned."
6. Hand off **only Core + Sub** to Step 2.

**What belongs in each layer:**

| Layer | Test |
|---|---|
| Core Query | Would a user type this whole thing into an AI as their opening question? |
| Sub-Query | Is this something the answer to the Core Query *must address* to be complete? |
| Dimension Note | Is this a useful detail, example, caveat or edge condition — but not something the answer would be incomplete without? |
| Merged | Is this the same decision as another Core, phrased differently? |
| Deleted | Is this actually a brand tactical goal wearing a question mark? |

That last row catches the most common contamination: *"why is {brand} better than {competitor}"* is not a user query, it is a positioning wish. Real users ask *"{A} vs {B} for {situation}"*. Delete the first, keep the second.

**Client review order:** confirm Core Query *direction* first, then Sub-Query *coverage*. Clients who are shown a flat list will edit individual wording and miss the architecture; clients who are shown Core Queries will engage with what actually matters.

<a name="9"></a>
## 9. Track 1A vs 1B execution detail｜双轨执行

**Track 1A · Query Discovery** — client gives products, we find queries.

1. Client provides line / product / competitor set
2. Full listening sweep across all three community rings
3. Friction synthesis
4. Core Query clustering
5. Sub-Query expansion
6. Client summary in four sections: *listening evidence → Core Queries → Sub-Queries → AU generation logic*
7. Client confirms → Step 2

Use for: a line entering GEO for the first time, a new category, or any brief where there is no query direction yet. This is the full-weight version.

**Track 1B · Query Validation** — client gives queries, we find the insight.

1. Client provides query list + line attribution
2. Targeted listening against those queries only — no full sweep
3. Backfill: source post title, verbatim user language, friction dimensions, competitor mentions, scenario detail, proof angle
4. Light clustering — client queries are usually already near Core level, so this pass is mostly dedupe and dimension completion
5. Step 2

Use for: lines with an existing evergreen query list from SEO, customer-service FAQ logs, or an established content matrix. Roughly **30–40% of 1A's workload.** The value is enriching existing queries with real evidence, not rediscovering them.

**Choosing:** input is "product name + competitors" → 1A. Input is "query list + questions we want to cover" → 1B. A line typically runs 1A in month one and 1B for increments after.

<a name="10"></a>
## 10. Multi-line registry and dedupe｜跨品线去重

When multiple product lines run Step 1 in parallel, they share one index, distinguished by the line segment of the Query ID: `{PERIOD}-{LINE}-{THEME}-{NN}`.

Different lines will independently discover overlapping Core Queries — gifting queries, budget queries and season queries collide constantly. Run a **cross-line check after all lines finish clustering and before anyone starts Step 2**:

- Identical Core Query found by two lines → produce **one** AU, covering both lines' products inside it
- Similar Core Query at genuinely different angles → keep as separate AUs, but cross-reference them so the recommendation logic stays consistent
- A query that only makes sense as a multi-line answer → assign an owner line explicitly, or it will be produced twice or not at all

Skipping this check is the most reliable way to waste a month of AU production capacity.

<a name="11"></a>
## 11. Common failure modes｜常见失败模式

**Searching with product names.** Returns existing customers and brand-aware users. You need pre-awareness language. Search patterns and situations instead.

**Only listening in Ring 1.** Category subs give you bottom-funnel comparison queries and nothing else. The high-value intent queries live in Ring 2 situation communities.

**Collecting instead of distilling.** A 200-row flat query pool is a worse deliverable than 12 Core Queries with real evidence. Volume signals effort; architecture signals thinking.

**Treating divergent comments as noise.** Divergence means nobody owns the answer. That's the opening.

**Padding L3.** If long-tail listening surfaces nothing with genuine resonance this month, ship without an L3 section. A thin L3 dilutes the whole map.

**Fabricating sources under deadline.** This destroys the credibility of the entire program the first time a client clicks a link. If a query has no source, mark it `Not ready` and move on.

**Dropping the verbatim language.** Paraphrased user language loses the exact words the AI will be prompted with. Preserve the original wording — it is the single most valuable artifact listening produces.
