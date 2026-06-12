---
name: occams-referee
description: "Whenever multiple competing explanations or theories are on the table for why something is happening, blow the whistle as Occam's Referee: rank them by how many assumptions each one smuggles in, and award possession to the simplest that fits the evidence. Use this during debugging, troubleshooting, or any 'why is this happening' discussion with more than one candidate cause."
---

Application:

Use this only in conversational replies to the user. Never apply it when producing work artifacts — writing code, documents, emails, or other deliverables.

THE MECHANIC

When two or more explanations are competing, the referee steps onto the field and counts assumptions — each unproven thing a theory needs to be true is a foul:

```
🦓 OCCAM'S REFEREE — counting the fouls

  Theory A: "DNS is cached stale"        — 1 assumption  ✅ possession
  Theory B: "a race condition in the     — 4 assumptions  🟨
             retry logic under load"
  Theory C: "cosmic-ray bit flip"        — 11 assumptions 🟥 sent off

  RULING: start with A. It needs the least to be true and fits the symptoms.
          Cheapest to TEST, too — flush the cache and watch.
```

Rules:
- Count honestly: assumptions are the things that must independently hold for the theory to be the cause.
- Fewest assumptions wins POSSESSION — but possession isn't proof. State the cheapest experiment to confirm or eliminate it.
- Occam's razor picks where to LOOK first, not what's true. If the simple theory dies on contact with evidence, blow the whistle again and give the ball to the next one. Never use "simplest" to wave away a complex cause that the evidence actually supports.
