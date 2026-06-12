---
name: branding-iron
description: "Whenever the user is struggling to name something — a project, a variable, a feature, a service, a team, a document — heat up the branding iron and stamp it: offer a few candidate names with the reasoning behind each, then a recommendation. Use this any time 'what should I call this' or 'I can't think of a good name' comes up."
---

Application:

Use this only in conversational replies to the user. Never apply it when producing work artifacts — writing code, documents, emails, or other deliverables.

THE MECHANIC

A name is a brand — it sticks to the thing forever and everyone reads it a hundred times. Heat the iron and offer a few stamps, each with its reasoning:

```
🔥🐄 BRANDING IRON — naming: "<the thing and what it does>"

   🅰️ <name>  — <style: literal / descriptive>
        why: <what it communicates instantly; who reads it and gets it>
        watch out: <collision, ambiguity, or how it ages>

   🅱️ <name>  — <style: metaphor / memorable>
        why: <…>     watch out: <…>

   🅲 <name>  — <style: short / neutral / boring-on-purpose>
        why: <…>     watch out: <…>

   🐄 Stamp this one: <recommendation + the single reason it wins>
```

Rules:
- Match the naming style to the CONTEXT. A variable wants clarity and convention; a product wants memorability; an internal tool can afford a little fun. Don't give a database column a brand-name.
- Always flag the practical hazards: name collisions, things that read badly when abbreviated, in-jokes that won't survive a new teammate, names that lie about what the thing does.
- Honor existing conventions in the user's codebase or org over cleverness. A consistent boring name beats a clever inconsistent one.
- Give a clear recommendation, not just a menu. The user came here because choosing is the hard part.
