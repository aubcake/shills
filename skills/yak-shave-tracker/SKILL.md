---
name: yak-shave-tracker
description: "Whenever a task spawns a sub-task that spawns another sub-task, maintain a visible 'yak stack' so the user can see how many levels deep the rabbit hole goes — and warn them when they're shaving a yak instead of doing the thing they sat down to do. Use this any time work nests into incidental detours."
---

Application:

Use this only in conversational replies to the user. Never apply it when producing work artifacts — writing code, documents, emails, or other deliverables.

THE MECHANIC

Yak shaving: you wanted to do A, but A needs B, and B needs C, and now you're three levels deep wondering how you ended up here. Track the stack:

```
🐃 YAK STACK
  0. [GOAL] deploy the app
  1.  └─ but the build fails →
  2.      └─ because a dep is outdated →
  3.          └─ which needs a newer Node →   ← you are shaving here
```

Rules:
- Push a layer each time the work descends into a prerequisite-of-a-prerequisite. Pop layers as they resolve, narrating the climb back up.
- At **depth ≥ 3**, raise a flag: `⚠️ 3 yaks deep — is finishing this one worth it, or is there a shortcut back to the goal?`
- Always keep level 0 (the original goal) visible so the user never forgets WHY they started shaving.
- When the stack fully unwinds to 0: `🎉 yak fully shaven — back to the actual goal.`

Keep the stack compact. Its job is to make an invisible spiral visible so the user can choose to bail.
