# EAB — Isolated Approach (One Element Per Clone)

## Concept

The strict version of element A/B testing — each clone changes exactly one thing versus the control, so any performance difference is cleanly attributable. Slower and more clone-hungry than the multi-element approach, but the only version that actually proves which element moved the needle.

## Usable two ways

- **Standalone** — skip the multi-element round entirely, start straight from the Phase 2 winning combo, test elements in the priority order below.
- **As a continuation** — after `eab-multi.md` narrows a shortlist of promising elements, run those specific elements in isolation here to confirm which one actually drove the bundled win.

## Before testing: read `read-results.md`

Same carryover logic applies — keep variants inside whatever axis (delivery or angle) Phase 2 confirmed as the win-factor, if it confirmed one.

## The control

The literal Phase 2 (or Phase 2 – Simple Path) winning ad, unmodified. Every clone in this round is measured against it.

## Element priority — phased, not all at once

**Phase A — non-negotiable, test first**
- **Hook** — the on-screen headline text, and its placement/composition where relevant. Highest leverage, always tested.
- **Dominant visual** — the main visual element the delivery is built around. Swap the subject, add or remove contrast against the background, reangle to a forced perspective or close-up — whichever fits the specific piece. It's dominant for a reason; it earns a test.

**Phase B — test once Phase A has a read, or alongside it if volume allows**
- **Body copy** — the supporting text beneath the hook.

**Phase C — light touch, test last or only once there's more data/budget**
- **CTA** — the action itself stays fixed (a DM CTA stays a DM CTA). Vary length (brief vs. elaborated vs. symbol-based), placement, or styling only.
- **Design/color treatment** — mostly inherited from the user's design guidelines and the proven delivery already. Only test this in isolation if it's clearly tied to another element under test, or obviously applicable on its own.
- **Slide sequence (carousel only)** — test with intent, never by blind reshuffling. Reordering point 2 before the hook for no reason is just noise. A legitimate sequence test has a hypothesis behind it — e.g. moving a light CTA into slide 2–3 to catch people who don't scroll to the end tests a real behavior; shuffling for the sake of shuffling doesn't.

## Volume

Aim for roughly 10–30 pieces across the whole EAB phase — same default guidance as Wave 1, not a hard rule.

## Structure

One campaign (CBO) for this whole phase, organized into ad sets per element or per phase as useful. This only becomes two campaigns if it's running as the confirmation round after a separate multi-element diagnostic campaign.

## Multiple surviving directions

If more than one combo survived Phase 2, this whole isolated process runs on the one chosen as primary (see `read-results.md`). Don't split full isolated rounds across multiple directions unless budget genuinely supports it.

## Out of scope here

- Stopping point for the whole EAB phase — on the user. They may move beyond this skill's scope entirely (video, organic content, bigger ABO tests) once they have enough data and confidence.
- Creative fatigue / refresh cycles for the eventual scaled winner — not this doc's concern.