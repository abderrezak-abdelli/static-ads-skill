# Meta Ads Launch Kit — Strategy Framework

## Purpose

This is a launch kit / starter system — a "put a table in the market" approach anyone can use to begin advertising, even with:
- a bad prior ads experience
- no structural ad strategy
- zero ad experience at all

It's also a **scout campaign**. The first launch isn't the end goal — it's how we gather real data (e.g. "Delivery X showed consistent wins," "Angle Y connects with people"). Once we have findings, we act on them (new formats/creative that lean into what worked).

**Overlaps between deliveries are allowed** if it helps the message land — but must be intentional (e.g. Story + Bulleted, Social Proof + VS, or any other combo).

---

## Strategy Overview

**Angles first, not element-testing.**

This is not A/B testing words/CTA/body copy. This is testing **combos/themes** to see what works with whom.

Why angles as the starting point: it brute-forces all probable variations and forces us to look at how to nail — and deliver — every variation well, so it can actually land.

⚠️ **Note:** Before/After framing is banned in Meta ads — execution needs to account for this. before-after delivery is Meta-restricted — it should get adapted (e.g. into a non-literal transformation framing) rather than executed literally.

**Flow:**
1. List angles worth hitting
2. Produce ads across multiple deliveries for each angle
3. Launch, gather data
4. Once winners are clear → run multiple executions of what worked, to squeeze the most out of the winning factors
5. Once the "why" behind what's working is clear → move to element-testing (one element to test per time - we clone that exact same winning ad a few times and change just one isolated element per clone—like testing new hooks, but keeping the background, script, and CTA completely identical to the winner. This way, if a variation spikes in performance, you know with 100% certainty that the new hook caused it. If you change multiple elements at once, you're just throwing blind shots and you'll never know what actually moved the needle)
6. This data also fuels other genres later (reels, organic content, etc.) — since by then we have an actual opinion about the market

**Anything past the first-wave launch is out of scope for this doc.** Once winners are spotted, next steps are decided from there.

---

## Format Focus: Statics First

We're focusing mainly on **static single-post or carousel ads**:
- Statics are the fastest/easiest to produce
- Producing a video for every variation would take forever
- A genre only counts as "tested" if it's executed at a 10/10 level — a bad UGC video from a bad creator doesn't mean UGC "doesn't work," it means that execution failed. Statics make it realistic to hit 10/10 across many variations.

Use **single post** vs **carousel** depending on the product:
- Simple/visually self-explanatory product → one image may be enough
- Complex product needing multiple points addressed → carousel, one point per slide

Recurring format (Story 9:16 / Post 3:4 / Reel / Static, etc.) is decided by the user. Reels are noted as a "future" genre — not part of this doc since they need separate video skills.

---

## Data Recording (Before Production)

Every variation must be logged before any image is produced — as an `.md` file (not a single file for every variation, but one file used to record all variations we going to make), a folder of `.md` files, or a free MongoDB table.

**Structure:**

[OFFER] – [MARKET] – [VP/ANGLE] – [DELIVERY] .
[OFFER] – [ANGLE] – [SUITABLE WARMUP].

---

## Campaign Structure: CBO Only (For Now)

Both the warmup campaign (if launched) and the first-wave ad campaign run as **CBO**, letting Meta decide budget distribution.

**Why not ABO for the first launch:**
- This is a first launch — no risk to be taken
- The user running this system is likely new to it, so it's fair for them to be doubtful; once CBO results prove theory matters in ads, they'll be more open
- ABO strategies exist and can be proposed later — either once the user trusts the system, or if they have a big enough budget to support solid testing


{"campaign_type":"CBO","ad_sets":[{"angle":"angle_1","ads":[{"id":"d1"},{"id":"d2"}]},{"angle":"angle_2","ads":[{"id":"d1"},{"id":"d2"}]},{"angle":"angle_3","ads":[{"id":"d1"},{"id":"d2"}]}]}

---

## Deliverables

### 1. Warmup

**Purpose:** Farm engagement from the right people; reach as much of the ideal avatar as possible. Warmup is **not** about nurturing/warming up the audience — it's about warming up the **ad account** (cheap, targeted interactions).

- Campaign goal: Post Engagement, optimized for **Comments** (trusted as the goal metric)
- Warmup content **never** mentions or sells the user's product/service — not once

**Warmup is mandatory for every angle**, even if the user doesn't plan to launch it as a paid ad (e.g. low budget). Reasons:
- can be used as organic content
- may change his mind

#### Warmup Content Types

**A. Education / Informative**

- **Struggles** — addressing observable struggles/issues the audience faces, in 3 possible depths:
  1. **No solution (Unaware Stage — Striking a Nerve):** Expose hidden pains, make invisible struggles feel urgent/tangible. Focus on *why it's a problem*, not how to fix it. Hooks: Pain / Controversy / Contrarian. CTA: open-ended question that drives real comments (personal experience/opinion — not lazy "comment 'yes'" bait).
  2. **Theoretical fix (Problem-Aware Stage — Giving Hope):** Prove the problem is solvable by breaking down a theoretical framework/principle. No specific product pitch, no actionable steps. Hooks: Benefit / Curiosity / Logic.
  3. **Practical fix:** Observable (1–3 lines max) + Diagnosis (bullets) + Payoff (content promise / micro action / quick win). Payoff = snackable, easy-to-pull, achievable advice. Match awareness stage to relevance.

- **Questions** — real audience questions (1–3 lines max each) + Answer (content promise / payoff / quick win).
- **Basics** — concepts/prerequisites/tips/"did you know" the audience should know + Lesson (details).
- **Misconceptions** — common industry misconceptions.
- **Ball-Knowledge** — content that shows deep, authentic niche/domain expertise (Gen Z term: knowing the obscure inner mechanics of a subject, not just surface-level trends).
- **Polemic** — content designed to get the comment section alive/talking.
- **News + comment CTA** — even absurd comment-bait framing works (e.g. "who's at fault here?").
- **Trend** — riding a current trend.
- **Probers / Scouters / Data-farmers** — content used to collect informal market data (favorite brands, style A vs style B, etc.). Getting data is a bonus — the real goal is comments from the right people (functions as a virtual/informal survey, not literal research).
- **Satire / Memes**
- **Ragebait**
- **Lead Magnets (comment-to-DM)** — requires explicit user approval before producing.
- Anything else that fits the same underlying concept.

---

## Reference: Ad Structure Skills

**Flow:** Offer → Market → VP/Angle → Delivery → produce for every probable variation worth trying → launch CBO → find winners → everything after is outside this doc's scope.

The approach is intentionally a brute-force sweep across probable variations — e.g. taking one product with no specific market defined, choosing "charmed offer" as the VP, and producing ads across every angle × every delivery.

### Offer Level — *what* to advertise
- **business_full** — the whole business, including free stuff (lessons, freebies, products, services) as one unit. CTA usually points to page/site/relevant destination; can include multiple CTAs if things live in different places.
- **business_catalog** — the whole catalog/menu. CTA: explore catalog.
- **business_category** — a category (e.g. drinks only), niche (e.g. feminine clothes), or vibe (e.g. medieval games, dark clothing). Usually covers multiple items at once (not sold at once like a pack, but advertised together).
- **pack** — a single offer bundling multiple products together.
- **single item** — any one service/product.

### Market Level — *who* we're speaking to
- **Not specified** — no targeting direction stated; model reasons it out.
- **Full Market** — treat all possible markets as one vague, inclusive audience snapshot.
- **Top Segments** — target the top 3 segments (separate research skill covers this, see: '/launch-kit/references/top-segments.md').

### VP / Angle Level — *what* we say, *which nerve* we hit
- **No specified value** — model picks.
- **Main value** — Rule of One: identify the main single core value proposition, discard all other angles. Every element reinforces this one idea.
- **Angles / reasons to buy** — list all possible reasons before selecting; then target all of them (e.g. gifting, seasonality, taste vs weight-loss, motive, etc.). Honorable mentions: seasons/holidays, gift, motive, argument, vibe, style, culture. etc
- **Main objections** — Result-effectiveness / Price / Trust, etc. — and counter them.
- **Main questions** — common questions people have about the product (may need the user's raw-dump of real questions they've received).
- **Charmed Offer** *(uses "Idea Charmer" skill see: '/launch-kit/references/offer-charmer.md')* — reframes a commoditized product into an exclusive, necessary solution to a hidden market opportunity. Presents a "Big Idea" contrasting market chaos (the haystack) with a hidden opportunity most people miss (the needle), positioning the offer as the unique mechanism (the magnet) to capitalize on it. Triggers core emotions: Newness, Easiness, Safeness, Bigness. "New" here means new-to-them, not literally recently launched. Addresses objections through proof, not just claims.
- **FOMO** *(separate skill see: '/launch-kit/references/terror.md', can top Charmed Offer)* — the "terror aspect": elicits fear of missing out by visualizing the cost of inaction — what the audience loses by ignoring the offer/opportunity. Not fear-mongering about safety/health — it's intrigue + regret over a missed advantage. Used *before* revealing the mechanism, as a catalyst to make the audience lean in before they even know the solution.
- **Charmed + FOMO** — both combined.
- **Sell the Dream / Future-You** — emotional selling; proof matters less here than emotional investment in fantasizing the target audience's future.

### Delivery Level — *how* it's visually/structurally delivered
- **Usecases / In-action** — offer + angle shown in real action, communicated visually.
- **Ugly ads** — e.g. dirty setting, black bg + plain to-the-point on-screen text, etc.
- **Subtle / Organic** — must fight ad-blindness, feel native to scroll behavior (e.g. UI/chat screenshots, real POV usage (if you make this preferably the user add native IG-story fonts manually, the ad image must first made with no text on screen, the users add what to type)). 
- **Bulleted benefits/values** — the standard "list the benefits/features" ad style, no comparison.
- **Poetic (symbolic/feel)** — visually symbolic messaging, like big-brand promotional style.
- **Before/After / Transformation Contrast** — sell the dream / future-you framing. *(⚠️ Meta restriction — handle carefully.)*
- **Problem–Solution**
- **VS (comparison)**
- **FAB** — Feature → Advantage over the alternative → Benefit.
- **Social Proof** — when available.
- **Collage** — e.g. 4x4 grid: one square text-only on empty bg, one square product with no text, one square benefits, one square 5-star review, etc. Bonus: doubles as a multi-test of multiple elements at once.
- **Storytelling**, **Behind the Scenes**, etc. 

You are never limited to the delivery examples included here, if you got a better idea i'm all in for creative freedom

---
## Anti Monotony
On the first wave don't make them all look the same or have the vibe/feel (eg: same vertically-centered text on black bg, etc) , try to vary the overall feel between variations, test multiple compositions, layouts, graphic-elements, the overall style, etc try some realistic, others dark/light theme, others light, different text placements, other setups, perhaps with 3d elements (perhaps even with depth of field / perspective lense applied on that 3d object - btw never make a human in your ads, i leave humans on real videos, if you make a human in your ad it will with no doubt flop), depth of field applied on text, maybe vary between overloaded graphics posts and minimal posts, or try to vary between basic-template-like design and brand-loyal design, or maybe something completly different like a known-app ui, trendy formats (eg: breaking-news, tier list, irl Whiteboard+marker, irl poster on wall, etc \\ irl means "in real life" here), leading object-outlining lines text or anything cool, maybe something cool with the text like text behind object makes the object feels 3d (not to cover all text that it wont be readable), etc. 

in short, just don't make them all the same

The point of this strategy is to stress-test, to do that we may also need to execute contradictory concepts (so results can make sense).
---

## Production Workflow (Post-Planning, Out of Scope for This Doc but Noted for Context)

1. text_map of variations to produce first, ideally recorded in MongoDB (or `.md` files as noted above). use '/launch-kit/work/assets/production/text_map.md' to log what you plan to produce or what you produced (after your discussion with the user, have a back and forth convo with him, guide him, ask questions and etc, eventually land on a text_map (also structure the text_map in a way you can use to keep track of what you produced so far, like a checklist).)
2. A separate downstream workflow takes each logged variation + the user's [writing guidelines / design taste / image-prompt guides / business info] and writes an image prompt for each image/carousel slide.
3. User takes the prompt and generates images one by one, at their own pace.
4. Test-launch the ads.
5. Anything beyond this point is out of scope — results dictate next steps.

===\
angles-reasons-to-buy and main-objections/main-questions aren't single VPs — they're lists that need to be expanded per-product first (gift/seasonality/motive/etc., each product's actual objections, each product's actual questions). Once expanded, each of those sub-items gets its own × N deliveries row. 


===\

# Claude Taste Comments : the following section is wrote by claude (may be a good model in this) as comments (they are in no way strict rules)
## How to Use the Offer × Message × VP × Delivery Variation Grid (Read Before Producing Anything)

The variation grid (offer × message level × VP/angle × delivery, run separately per offer) is a **library, not a checklist**. It represents every theoretically possible combo — it is NOT a production requirement. Exercise judgment and select combos based on what actually fits the specific offer/business being worked on. Treat low-fit combos as available-but-skippable, and treat "promising routes" as a starting shortlist, not a limit — selection can go outside the shortlist if the offer calls for it.

Two structural notes already handled elsewhere in this doc, don't re-flag them:
- `angles-reasons-to-buy`, `main-objections`, and `main-questions` are lists to be expanded per-product before combining with deliveries.
- top segments too, they produce multiple segments to target separately.
- `before-after` delivery is Meta-restricted and must be adapted, not executed literally.

### Skippable / Low-Fit Combos (Default: Deprioritize)

These combos tend to fight themselves — tonal, structural, or format mismatches that usually produce a weak or incoherent ad. Skip by default unless the specific offer has an unusual reason to force the combo:

- **`ugly` × `poetic`** — ugly/raw aesthetic directly conflicts with poetic/symbolic polish.
- **`ugly` × `collage`** — collage relies on structured visual composition; ugly-ads relies on deliberate rawness. Rarely coexist cleanly.
- **`poetic` × `vs`** — comparison delivery needs clarity/directness; poetic needs ambiguity/feel. Usually cancels itself out.
- **`poetic` × `fab`** — FAB is a logical/structured breakdown; poetic is emotional/abstract. Mismatched cognitive modes.
- **`social-proof` × `sell-the-dream`** — sell-the-dream leans on emotional fantasy over proof; pairing with social-proof (a credibility/logic lever) usually dilutes the emotional pull.
- **`bulleted` × `storytelling`** — storytelling needs narrative flow; bulleted format breaks that flow into fragments. Usually better as two separate executions than one.
- **`subtle-organic` × `main-objections`** — objection-handling needs to be legible/direct; subtle/organic delivery is built to hide the sales intent, which works against clearly addressing an objection.
- **`main-questions` × `poetic`** — Q&A-style content wants clarity and directness; poetic delivery obscures the direct answer.

### Promising Routes (Default Shortlist — Not Exhaustive)

These pairings are structurally coherent and tend to produce strong first-wave candidates. Use as a starting point, adjust per offer:

- **`main-value` × `in-action`** — clean, direct proof of the core value being used/working.
- **`main-value` × `problem-solution`** — pairs a single strong value prop with the clearest persuasion structure there is.
- **`charmed-offer` × `poetic`** — the Idea Charmer's "Big Idea"/needle-in-haystack narrative benefits from symbolic, feel-driven visual treatment (not to make a literal image of a needle+haystack, but to inspire you the underlying subtext that should be communicated based on the offer selected).
- **`charmed+fomo` × `storytelling`** — both mechanisms are narrative-driven (haystack/needle + cost-of-inaction); storytelling delivery is the natural carrier.
- **`fomo` × `ugly`** — urgency/terror-aspect messaging often lands harder in a raw, low-polish, "this is real" format than in a polished one.
- **`sell-the-dream` × `poetic`** — emotional-selling angle paired with the delivery built for feel over proof — natural fit.
- **`angles-reasons-to-buy` (per expanded angle) × `subtle-organic`** — native, scroll-blending delivery is a strong low-risk default for testing multiple reason-to-buy angles cheaply.
- **`main-objections` (per expanded objection) × `fab`** — FAB's feature→advantage→benefit structure is well-suited to directly dismantling a named objection.
- **`social-proof` × `bulleted`** — when proof assets exist, pairing them with a clean benefits list is a reliable, low-risk combo for warmup-to-ad crossover content.
- **`unspecified-value` × `usecases/in-action`** — a safe, low-assumption default when angle direction is genuinely unclear and needs the model to reason freely.

You should still weigh offer type, market, and available creative assets before finalizing selections — this list narrows the search space, it doesn't replace judgment.