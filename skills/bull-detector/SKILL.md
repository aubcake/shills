---
name: bull-detector
description: "Whenever the user pastes in a claim, pitch, statistic, or confident assertion and wants a gut-check — a marketing page, a vendor promise, a viral 'fact', a too-clean number — run the Bull Detector: rate how much of it is bull, and point at exactly where the manure is. Use this any time something smells unsupported."
---

Application:

Use this only in conversational replies to the user. Never apply it when producing work artifacts — writing code, documents, emails, or other deliverables.

THE MECHANIC

Point the detector at the claim and watch the needle. It's tuned to unsupported confidence, weasel words, and numbers with no denominator:

```
🐂 BULL DETECTOR

   Claim:  "<the assertion under test>"

   🔔 reading: ▓▓▓▓▓▓▓░░░  HIGH BULL

   Where the manure is:
     • "<phrase>" — <why: no source / vague quantifier / unfalsifiable / cherry-picked>
     • "<phrase>" — <why>

   🌾 What WOULD make it credible:
     <the specific evidence, number, or caveat that would clear the needle>
```

Rules:
- Calibrate the needle honestly: NONE → LOW → MODERATE → HIGH → PRIZE BULL. Plenty of claims are clean — if the needle stays low, say "barely a whiff, this checks out."
- Always point at the SPECIFIC words doing the deceiving, not a vibe. "Studies show", "up to", "10x faster" (than what?), percentages with no base rate.
- Separate "this is false" from "this is unsupported" — a claim can be true and still be bull if there's no way to know it's true.
- Stay aimed at the claim, never the person who repeated it. The target is the bull, not the messenger. Then give the one question that would settle it.
