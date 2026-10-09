# EAB — Multi-Element Approach (Bundle → Diagnose)

## Concept

Instead of isolating one element per clone from the start, bundle a small number of related changes into each clone, run the round, then diagnose which bundle(s) won. Faster and cheaper in clone count than pure isolation — at the cost of not knowing exactly which element inside a winning bundle did the work. That gap can be closed later with `eab-isolated.md`, if it's worth the follow-up.

## When to use

- Clone count or budget is tight and full isolation would take too many rounds to get through.
- A fast read across several candidate directions is wanted before committing to the slower isolated method.
- Both approaches are being kept available on purpose, and it hasn't been decided yet which one to commit to.

## Before bundling: read `read-results.md`

Apply whatever win-factor carryover exists before deciding what goes into each bundle — e.g. if the delivery is the confirmed win-factor, build bundles that vary hook/visual while keeping that delivery's structure intact.

## Building the bundles

- Keep each bundle small — 2–3 changes — and thematically coherent, not a random stack. A "big swing" bundle (new hook + new visual) and a "safe" bundle (same hook/visual, new CTA styling) are two different, readable bets. A bundle that changes five unrelated things isn't a bet, it's noise.
- Naturally linked elements (visual + design treatment) bundle well together, since they're rarely independent in practice anyway.
- Every clone runs against the same control: the literal Phase 2 winning ad, unmodified.

## Reading the results

- Compare each bundle's performance against the control and against each other.
- Note which elements co-occur in the winning bundle(s) — this is a lead, not proof.
- Decide what to do with the lead:
  - **Resources allow a follow-up** → hand the shortlisted elements to `eab-isolated.md` for a confirmation round that disentangles which one actually drove the result.
  - **Resources don't allow it, or the user has moved past this skill's scope** → adopt the winning bundle as the new control and stop there. Don't force a confirmation round that isn't going to happen.

## Structure

This round is one campaign (CBO), organized into ad sets per bundle concept if useful. If it's followed by an isolated confirmation round, that round is a separate, second campaign.

## Standalone use

This approach doesn't require ever running the isolated method afterward. A clear bundle winner, adopted as the new control, is a legitimate stopping point on its own.