---
name: holy-cow-alarm
description: "Whenever a number, result, or claim in the conversation is genuinely surprising — an outlier, a too-good-to-be-true figure, a result that contradicts what came before, an order-of-magnitude that doesn't add up — pull the Holy Cow Alarm, flag the anomaly, and sanity-check it before anyone trusts it. Use this any time something deserves a double-take."
---

Application:

Use this only in conversational replies to the user. Never apply it when producing work artifacts — writing code, documents, emails, or other deliverables.

THE MECHANIC

Most numbers slide by unexamined. The Holy Cow Alarm only rings for the ones that genuinely shouldn't — the outlier, the figure that's too clean, the result that quietly contradicts an earlier one:

```
🐄🔔 HOLY COW —

   "<the surprising figure or claim>"

   Why the alarm rang:
     <what makes it anomalous — wrong order of magnitude / contradicts
      <earlier fact> / improbably perfect / implies something absurd if true>

   🧮 Before anyone trusts it, check:
     • Units right? (a 1000× error loves to hide in a unit slip)
     • Same denominator as what it's compared to?
     • If it IS real, what would have to be true? Is that plausible?

   Verdict: <probably a glitch, verify before acting / genuinely surprising
            and apparently real — worth understanding why>
```

Rules:
- Ring ONLY for genuine anomalies. An alarm that goes off for ordinary numbers gets ignored — protect its signal value ruthlessly.
- A surprising result isn't automatically wrong. The job is to flag-and-check, then let it stand if it survives. Sometimes "holy cow, that's real" is the answer.
- Always name WHY it's surprising and the specific check that would confirm or kill it. A double-take with no follow-through is useless.
- Most often the culprit is units, a denominator mismatch, or a typo'd zero — check those first.
