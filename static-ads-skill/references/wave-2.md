# Meta Ads — Phase 2: Post-Launch Direction (Wave 1 → EAB)

## Scope

This covers the moment right after Wave 1 reports results, through to a combo earning Element A/B testing (EAB). It does not cover future phases beyond EAB, budget math, or result logging — logging may be handled by the parent agent skill this doc lives inside.

**What counts as a win:** whatever gets most profits. Absent connected sales data, Meta on-platform results (cost-per-result, CTR) are the working proxy. If a winner later turns out different by actual sales, the user will flag it — don't try to resolve that mismatch automatically, just surface it before planning the next wave.

---

## Step 1 — Tier every ad

Rank all Wave 1 ads by cost-per-result (or the equivalent efficiency metric available). Split into three bands:

- **Top** — the most efficient third
- **Mid** — the middle third
- **Low** — the least efficient third

Use relative bands, not fixed dollar thresholds — Wave 1 spend levels vary. If the split isn't clean into thirds, use judgment on where the natural breaks fall.

---

## Step 2 — Cluster by delivery, then separately by angle

Every ad gets counted twice: once under its delivery, once under its angle. For each delivery value and each angle value that appears **2 or more times**, tally how many of its appearances landed Top / Mid / Low, and note whether the appearances were paired with genuinely different partners (different angle *types* — value-led vs objection-led vs FOMO-led — not just different segment labels on the same idea).

Classify each cluster:

| Pattern | Label |
|---|---|
| Majority Top, across diverse partners | **Strong** |
| Consistently Mid, never Top or Low | **Stable** (safe, unremarkable) |
| Consistently Low, across diverse partners | **Weak** (real negative signal) |
| Split roughly evenly between tiers, or repeats are really the same partner type in disguise | **Mixed** (no signal) |
| Appears only once | **N=1** (can't cluster — not a red flag, just no data) |

---

## Step 3 — Guardrails

Apply these before drawing any conclusion from the clusters:

1. **Never discard a Top-tier individual result for lacking repeat siblings.** Raw performance is judged before clustering, not gated by it.
2. **Never let a Mixed or absent cluster water down an ad's own Top-tier score.** Isolated excellence stays top priority — it gets hedged treatment instead of committed treatment (see Step 5), never no treatment.
3. **When an ad sits at the intersection of two clusters, credit the stronger, more consistent one.** Don't average two axes into a vague "both mattered."
4. **Stable and Weak are not the same as Mixed.** Consistently Mid is a safe filler signal. Consistently Low is a real negative — deprioritize it. Mixed means no usable signal either way. Don't collapse all three into "ignore."
5. **Tiers are directional, not exact**, especially at low spend. Don't over-read a one-result gap between two ads in the same tier.

---

## Step 4 — Rank order

Priority runs in this order — top performers first, clusters second, everything else last.

**Rank 1 — Top individual performers. Lean hard.**
Every ad in the Top tier carries forward into Phase 2, regardless of whether it has cluster backing. Nothing gets dropped here for lacking company.

**Rank 2 — Strong, diverse clusters. Lean mid.**
Used to decide *how* a Rank 1 result gets expanded (see Step 5) — it doesn't introduce new candidates on its own unless a cluster is loud enough to be worth a small independent look even without a Top-tier individual result.

**Rank 3 — Everything else. Lean soft.**
Mixed clusters, one-off Mid performers, confidently Weak clusters. Logged, deprioritized, not actively pursued unless nothing else is available.

---

## Step 5 — Decide the expansion type for each Rank 1 result

For each Top-tier ad, check its delivery cluster and its angle cluster independently, then pick one:

- **Both axes weak/mixed/N=1 → Hedge.** Run a small AOD and a small DOA on this pairing in parallel, to find out whether either axis actually travels, or whether the pairing itself is the reason it worked.
- **One axis Strong, the other weak/mixed/N=1 → Commit to the backed axis.** Run a full round on that axis (DOA if the delivery is backed, AOD if the angle is backed). Treat the unbacked axis as exploratory only, if at all.
- **Multiple Rank 1 results share the same Strong cluster → Treat as one direction, not several.** The repeated top scores reinforce each other; commit to that axis with the largest share of the round's budget.

---

## Step 6 — Structure the ad sets

- **Tight budget:** one CBO, bulk-created, let it run. Diagnosis (Steps 1–5) is free either way and should always be done — it's just reading data already paid for. (assume user has tight budget by default, unless he says otherwise)
- **Flexible budget:** ABO, sized per creative to guarantee roughly 8% reach into the targeted market segment, instead of leaving allocation to CBO's early-result bias.

Budget amounts themselves aren't calculated here — that's on the user.

---

## Step 7 — Multiple directions

If more than one direction survives Step 5:

- Directions backed by the same Strong cluster merge into one (see Step 5).
- Standalone directions (hedged pairings, angle-only or delivery-only leads) are cascaded: pursue the top 1–2 with paid testing, log the rest as pattern data for future creative generation. Logging mechanics live in the parent agent skill.

---

## Step 8 — Graduate to EAB

Once a direction's AOD or DOA round itself produces a repeat winner — the axis confirms a second time — that specific combo graduates to Element A/B testing. EAB is not a parallel branch chosen up front; it's the destination every direction is working toward, and it only starts once there's a combo worth refining at the element level.

Wave 1 already proves a combo can win in the real market. What Steps 1–7 exist to answer is *why* it won, so that EAB spends its precision on the ingredient that actually earned the result — not on whichever one happened to be sitting next to it.

---

## Appendix — Worked reference

A short illustration of the reading process, using placeholder results on a 20-ad wave:

- Ad `X` (delivery `problem_solution`, angle `main_value`) — **Top**. Delivery `problem_solution` also appears in 3 other ads across genuinely different angle types, Top in 2 of them → **Strong** cluster → **Commit**: full DOA on `problem_solution`.
- Ad `Y` (delivery `poetic`, angle `sell_the_dream`) — **Top**, the best single result in the wave. Neither its delivery cluster nor its angle cluster is Strong → **Hedge**: small AOD + small DOA on this pairing.
- Ad `Z` (delivery `collage`, angle `main_value`) — **Top**, delivery is N=1 but angle `main_value` is independently Strong (2 Top results across 3 appearances, different deliveries each time) → **Commit to the angle**: full AOD on `main_value`, including more of the delivery style that produced Ad Z.
- Deliveries `vs` and `ugly` — both ran twice, both Low both times, across different angles → **Weak**, deprioritized going forward.

---

## Next Steps

After you diagnosed data, planned your next moves; go ahead and make a /[offer]-wave-2 folder inside /[offer] folder that is inside /generation-prompts (just like you did with wave-1) > make wave-2-text_map.md inside it and start generating the prompts inside the /[offer]-wave-2.
