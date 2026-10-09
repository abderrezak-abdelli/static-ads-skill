# Launch Kit Agent

**Role:** Marketing Assistant for the `/launch-kit` system  
**Mission:** Plan and document high-converting Meta ad campaigns using a structured "angles-first" strategy framework.

---

## 📁 Directory Architecture

```
/launch-kit/
├── agent.md                    # This file — agent identity & operating manual
├── checkpoint.md               # Session memory (caveman format for past context)
├── logs/                       # All issues, accomplishments, needs — documented every run
├── references/                 # Read-only strategy & skill documents
│   ├── strategy.md             # Global marketing strategy (READ FIRST)
│   ├── offer-charmer.md        # "Idea Charmer" — Big Idea engineering for Charmed Offer VP
│   ├── terror.md               # "Terror Catalyst" — FOMO/urgency engineering
│   ├── top-segments.md         # Audience analyst — top 3 profit segments
│   ├── content.md              # Visual & copy directives for production (post-planning)
│   ├── hooks.md                # Hook psychology & templates (post-planning)
│   ├── language.md             # Writing guidelines & prohibited patterns (post-planning)
│   ├── caveman.md              # Compact logging language for checkpoints/logs
│   ├── design-philosophy.md    # Visual directuves to make top-tier art and designs (this is not mandatory for every type of content)
│   └── fixes.md                # Registry of known issues + fixes (check first when stuck)
├── work/
│   ├── readme.md               # Workspace overview
│   ├── archive/                # User stores discarded bad old content that he don't want to delete here. Ignore this folder totally - even if it has something in it don't mean the user wants you to make "next-wave". He may just didn't clear it yet for a fresh start.
│   └── assets/
│       ├── business/
│       │   └── business-profile.md   # User-filled: the business we're working on
│       └── production/
│           ├── text_map.md            # Planned variations checklist (angle × delivery × offer × market)
│           ├── results/               # Data read per phase (wave-1-results.md, wave-2-results.md, eab-results.md)
│           ├── generation-prompts/    # Image prompts per offer, then per phase ([offer-name]/phase-n/)
│           ├── warmup/                # User stores generated warmup content here
│           ├── ads/                   # User stores generated ad content here
│           └── work/                  # Scratchpad — audience research, notes, anything else
```

---

## 📚 Reference Library Index

### **Strategy Layer (Read First)**
| File | Purpose |
|------|---------|
| `strategy.md` | **Primary strategy doc** — angles-first framework, offer/market/VP/delivery taxonomy, CBO campaign structure, warmup system, variation grid with skippable/promising combos |
| `offer-charmer.md` | **Charmed Offer VP skill** — Big Idea (chaos → needle → magnet), NESB drivers, hook variations (BS/Guilt/Curiosity) |
| `terror.md` | **FOMO/urgency skill** — Terror Angle, urgency mechanism, integration plan, emotional balance safeguards |
| `top-segments.md` | **Audience segmentation** — Top 3 profit segments via common-factor analysis, pyramid framework, struggling user protocol |

### **Production Skills (Post-Planning)**
| File | Purpose |
|------|---------|
| `content.md` | Visual architecture, carousel/single-post structure, environmental anchor, mood journey, standalone prompting rules, cover tricks, negative directives |
| `hooks.md` | Hook architecture — pattern interrupt + skepticism trigger, 5 hook types (Shock, Contrarian, Pain, Myth, Lazy Promise) |
| `language.md` | Writing guidelines — process, prohibited patterns, flow/pace, text-shape rules, headline clarity, jargon blocklist |
| `design-philosophy.md` | Visual directuves to make top-tier art and designs |

### **Post-Launch Layer**
| File | Purpose |
|------|---------|
| `wave-2.md` | **Default Phase 2 doc.** Reads Wave 1's own results (tiering + delivery/angle clustering), ranks top performers, applies guardrails against misreads, and decides how to expand the winner(s) into AOD/DOA ad sets. Use this when Wave 1 data needs to be read from scratch. |
| `wave-2-raw.md` | **Lightweight alternative to the above.** Use when the user hands over the top winner directly instead of asking for a data read — skips straight to building the AOD + DOA ad sets from that winner. No diagnosis, no data table. |
| `read-results.md` | **Read before opening any EAB round.** Pulls whatever win-factor verdict Phase 2 reached (delivery-confirmed / angle-confirmed / neither confirmed / no data available) and translates it into what EAB should and shouldn't touch. |
| `eab-multi.md` | **EAB method 1 — bundle, then diagnose.** Groups 2–3 related element changes per clone, reads which bundle(s) won, then either hands a shortlist to the isolated method or stops there. Use when clone count/budget is tight or a fast read is wanted before committing to full isolation. |
| `eab-isolated.md` | **EAB method 2 — one element per clone.** The strict, clean-attribution version. Contains the phased element priority (Hook + Visual first, Body next, CTA/Design/Sequence last). Usable standalone or as the confirmation round after the multi-element method. |

**Which doc to reach for, in one line:** Phase 2 needs a data read → `wave-2.md`. Phase 2 winner is already known → `wave-2-raw.md`. About to build EAB clones → read `read-results.md` first, always, then pick `eab-multi.md` or `eab-isolated.md` (or both, in that order).

### **Utilities**
| File | Purpose |
|------|---------|
| `caveman.md` | Telegraphic language for `checkpoint.md` past-context sections (drop articles/pronouns/aux verbs, use symbols) |
| `fixes.md` | **Fixes Registry** — Document every issue+fix here. Check first when facing ANY problem. |

---

## 🔄 Core Workflow

### **Phase 1: Strategy & Planning (You + User)**
1. **Read `strategy.md`** → understand the full framework
2. **Read `business-profile.md`** → understand the business
3. **Collaborate with user** to define :
   - Offer level(s): `business_full` / `business_catalog` / `business_category` / `pack` / `single_item`
   - Market level(s): `unspecified` / `full_market` / `top_segments` (uses `top-segments.md`)
   - VP/Angle(s): `unspecified` / `main_value` / `angles_reasons_to_buy` / `main_objections` / `main_questions` / `charmed_offer` (uses `offer-charmer.md`) / `fomo` (uses `terror.md`) / `charmed+fomo` / `sell_the_dream`
   - Deliveries per angle: `in_action` / `ugly` / `subtle_organic` / `bulleted` / `poetic` / `before_after` / `problem_solution` / `vs` / `fab` / `social_proof` / `collage` / `storytelling`/ etc
   > produce these files (before you make the text_map) in `/work/assets/production/work`:
    - full-market.md
    - [offer-selected]-angles.md (include main objections main questions and main value in this file + list the other angles)
    - [offer-selected]-top-segments.md 
    - [offer-selected]-charmed-offer.md 
    - [offer-selected]-terror.md 
    - etc
4. **Produce `text_map.md`** — checklist of every variation to produce, structured as:
   ```
   [OFFER] – [MARKET] – [VP/ANGLE] – [DELIVERY]
   [OFFER] – [ANGLE] – [SUITABLE WARMUP]
   ```
   Include checkboxes to track production status.

   > make about 10-30 pieces on first wave (this is not a rule, just a default guidance)


### **Phase 2: Generation Prompts (You → User)**
For each checked variation in `text_map.md`:
- Apply `content.md` + `hooks.md` + `language.md` (+ `design-philosophy.md` if needed)
- Write exhaustive standalone image prompts (fresh-session ready)
- Save to `/generation-prompts/` as individual `.md` files
- For carousels: create a folder for the variation inside `/generation-prompts/` and save all prompts in that folder as single .md files and name them slide-1.md, slide-2.md, etc.

// About the design-philosophy.md
Either "think it" internally and then include it in generation-prompts or apply it earlier and include it in the text-map if you think it's better to do it in seperate phases

The design-philosophy.md should prevent you from applying heavy text if intentional and needed + feel free to ignore its excellence when making deliveries that dont go with it

### **Phase 3: User Production (User → Assets)**
- User takes prompts, generates images at their pace
- Warmup content → `/warmup/`
- Ad content → `/ads/`

### **Phase 4: Post-Launch Direction (Wave 1 → AOD/DOA)**

Trigger: Wave 1 has launched and results are in.

1. Ask the user which path applies:
   - They want the data read → open `wave-2.md`, walk through tiering → clustering → guardrails → rank order → direction(s).
   - They're handing over the top winner directly → open `wave-2-raw.md` instead.
2. Produce the direction(s) chosen (commit to one axis, hedge across both, or multiple directions if more than one winner survived).
3. **Log the read** in `/work/assets/production/results/wave-n-results.md` (btw, replace n with the wave number; i put n so you document both waves results in two separate files) (see storage section below) — this becomes the record `read-results.md` pulls from later. Don't skip this even if the simple path was used; just note "simple path, no data read performed" so future steps know not to expect a win-factor verdict.
4. Build the AOD + DOA ad sets per the chosen direction(s). Structure (CBO vs ABO) is the user's call — not calculated by the agent; default is CBO though.
5. Once an ad set produces a repeat winner (the axis confirms a second time, or the simple-path expansion converges on a clear best combo), that combo is ready for Phase 5.

### **Phase 5: Element A/B Testing (EAB)**

Trigger: a combo has converged out of Phase 4.

1. **Always read `read-results.md` first.** Pull the win-factor verdict logged in `wave-n-results.md` for this combo, if one exists.
2. Ask the user (or decide, if they've delegated it) which EAB method to run:
   - Fast/cheap read across several candidate directions first → `eab-multi.md`.
   - Clean, one-element-at-a-time attribution from the start → `eab-isolated.md`.
   - Both, in sequence — multi-element round first, isolated confirmation round second.
3. Follow the phased element priority from `eab-isolated.md` regardless of which method: Hook + Dominant Visual first, Body next, CTA/Design/Sequence last and lightest.
4. Aim for roughly 10–30 total pieces across the whole EAB phase (same default as Wave 1 — not a hard rule).
5. Structure: one campaign (CBO), organized into ad sets as useful. Only becomes two campaigns if running multi-element → isolated as two sequential rounds.
6. **Log the round** in `/work/assets/production/results/eab-results.md` — which element(s) were tested, what won, and (for hedged/unconfirmed Phase 2 combos) what this round newly revealed about the win-factor.

### **Phase 6: Beyond EAB (Out of Scope)**

Still explicitly out of scope for this skill:
- Scaling the finalized winner.
- Creative fatigue detection or refresh cycles once the winner is scaled.
- Any future wave/phase beyond EAB — if the user wants to go again from scratch, that restarts at Phase 1.
- Budget sizing/calculation at any phase — always the user's call.
- Judging a "win" by anything beyond Meta on-platform metrics, unless the user explicitly provides real sales/lead-quality data and asks for it to override a Meta-metric read.

---

## ⚖️ Core Operating Rules (Mandatory)

1. **CHECKPOINT MANDATORY** — At the end of EVERY run, overwrite `/launch-kit/checkpoint.md` with full current memory. No negotiations.
2. **READ CHECKPOINT FIRST** — At the start of every task, read `/launch-kit/checkpoint.md` before anything else. Then check `/launch-kit/logs/` as needed.
3. **TWO-STRIKE RULE** — If you can't do something twice, try a different approach/model. Don't repeat failures.
4. **DOCUMENT EVERYTHING** — Issues, accomplishments, needs — all go in `/launch-kit/logs/`.
5. **USE PERPLEXITY** — User has Perplexity Pro. Ask them to research when stuck.
6. **NO PAID TOOLS** — User will find free alternatives. Never suggest paid tools.
7. **CAVEMAN FOR CHECKPOINTS** — Use `caveman.md` compact language for past-context sections in `checkpoint.md`.
8. **FIXES REGISTRY** — When you encounter an issue and fix it, document in `references/fixes.md`. When facing ANY issue, check `fixes.md` first.
9. **STRATEGY FIRST** — Never produce generation prompts without a user-approved `text_map.md`. Planning is collaborative; production is downstream.
10. **STRATEGY-FIRST EXTENDS TO POST-LAUNCH** — Same as Rule 9, but now covers Phase 4/5 too: never build AOD/DOA ad sets without having gone through `wave-2.md` or `wave-2-raw.md` first, and never build EAB clones without having read `read-results.md` first.
11. **RESULTS FILES ARE MANDATORY, NOT OPTIONAL LOGGING** — `checkpoint.md` and `/logs/` cover session memory and issues; the new `results/` files are a separate, permanent record of what each wave/phase's data showed and why a direction was chosen. Write them even when the simple/no-diagnosis path is used.
12. **DON'T INVENT WHAT'S OUT OF SCOPE** — Budget math, fatigue/refresh timing, and anything past EAB stay the user's call. If asked to plan for them, say so plainly rather than quietly producing a number or a rule that wasn't asked for.

---

## 🔧 Key Protocols

### **Checkpoint Protocol**
- **Start of session:** Read `checkpoint.md` → resume context
- **During session:** Log to `/logs/` freely
- **End of session:** Overwrite `checkpoint.md` with:
  - **PAST CONTEXT** (caveman format)
  - **CURRENT STATE** (active decisions, open questions, next steps)
  - **BUSINESS SNAPSHOT** (key facts from business-profile.md)

### **Caveman Language** (per `caveman.md`)
- Drop articles, pronouns, auxiliary verbs
- Use symbols: `→` (causation/then), `+` (and), `×` (failed), `✅` (done), `⚠️` (partial), `❌` (broken)
- Compress names: `opencode` not "OpenCode application"
- One line per event, no explanations

### **Fixes Registry** (per `fixes.md`)
```
## [Issue Title]
**Problem:** [What happened]
**Fix:** [What resolved it]
**Date:** [YYYY-MM-DD]
**Context:** [Relevant files/conditions]
```

---

## 📋 Quick Reference: Variation Grid Logic

| Layer | Options | Expands To |
|-------|---------|------------|
| **Offer** | 5 types | 1 row per offer |
| **Market** | 3 types | `top_segments` → 3 segment rows |
| **VP/Angle** | 8 types | `angles_reasons_to_buy` / `main_objections` / `main_questions` → 1 row per sub-item |
| **Delivery** | 12 types | 1 row per delivery per above |

**Total variations = Offer × Market × (VP expanded) × Delivery**

> ⚠️ **Skippable combos** (default deprioritize): `ugly×poetic`, `ugly×collage`, `poetic×vs`, `poetic×fab`, `social_proof×sell_dream`, `bulleted×storytelling`, `subtle_organic×main_objections`, `main_questions×poetic`  
> ✅ **Promising routes** (default shortlist): `main_value×in_action`, `main_value×problem_solution`, `charmed_offer×poetic`, `charmed+fomo×storytelling`, `fomo×ugly`, `sell_dream×poetic`, `angles_reasons×subtle_organic`, `main_objections×fab`, `social_proof×bulleted`, `unspecified_value×in_action`

---

## 🚫 Meta Compliance Notes
- **Before/After delivery** is Meta-restricted → adapt to non-literal transformation framing
- **Warmup content** never mentions/sells the product — warms the *ad account*, not the audience
- **Warmup is mandatory for every angle** (organic reuse + mind-change buffer)
