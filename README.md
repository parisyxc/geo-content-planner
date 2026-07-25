# GEO Content Planner

> Get recommended by AI search. A monthly operating system that turns a brand's social output into long‑lived, **AI‑citable evidence assets** — instead of one‑off campaign traffic.

Shopping is moving from Google/Amazon/feeds to questions asked of AI: *"I sleep badly, help me pick a pillow."* The AI understands the need, then names a brand. The competitive question is no longer only "does the user know me" but **"is the AI willing to recommend me."** This tool builds the evidence that earns the recommendation.

## Input → Output

**Input — 3 things**
- `brand` — name · category · core product
- `consumer_target` — who, and the real *situation* they're in (not a demographic)
- `platform_positioning` — which platforms and each one's role

**Output — 3 deliverables** (templates in `assets/`)
- **Query Map** — tiered Core × Sub queries, each with real listening evidence, priority, and readiness
- **Answer Units** — structured answer modules an AI engine can lift wholesale
- **Platform Distribution** — a per‑platform monthly plan: quantity, post‑level angle, format, funnel role, citation surface

## The monthly loop

```
Step 0 Intake → Query Finding → Answer Unit → Distribution → Monthly Track  ↻
```

**Step 0 · the Semantic North Star** is the most important step: one sentence — *"AI should understand {brand} is the {attribute} choice in {category}"* — decomposed into 5–8 proof angles. Every Answer Unit then carries one angle, so the AI generalizes a pattern instead of hearing a slogan.

The **Query ID** (`{PERIOD}-{LINE}-{THEME}-NN`) is the spine: one query → one or more Answer Units → many platform posts → every month‑end citation and funnel datapoint hangs back onto it. **Heavy / Medium / Light** coupling keeps narrative content (TVC, KV, trend) from being wrongly scored as a failed citation.

## What's in this repo

| Path | What it is |
|------|-----------|
| `SKILL.md` | The full skill — Step 0–4, bilingual (EN / 中文). Load into Claude / any LLM |
| `TOOL-SPEC.md` | The input → output contract and how it's framed as a tool |
| `references/01–05` | Deep playbooks: GEO thesis · Reddit listening · Answer Unit craft · platform roles · tracking & KPI |
| `assets/` | Copy‑and‑fill templates: Query Map (CSV) · Answer Unit (MD) · platform monthly plan (MD) |
| `demo/geo-content-planner-demo.html` | A fully worked sample on a **fictional** brand ("Aria") |

## Use it

Load `SKILL.md` as a skill, confirm the three inputs, then run the monthly loop — pulling in `references/` when a step needs depth and copying the `assets/` templates instead of reinventing the schema. Open `demo/` first to see the shape of the output.

---

*Part of theAgenticMarketing — a marketing toolkit for founders, solo operators, and agency owners. Demos use fictional or public brands only; no client work is included.*
