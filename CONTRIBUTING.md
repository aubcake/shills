# Contributing

A "skill" in this repo is just a short note that tells an AI assistant how to behave in a specific situation. That's it. It's a text file with some instructions. The bar is low. The bar is on the floor. If I can do it, so can you.

## What you'll need (one-time setup)

1. **A free [GitHub](https://github.com) account.** Sign up if you don't have one.
2. **???**
3. **Profit!**

## The easiest way to contribute

### Step 1: Go fork yourself

1. Go to the project page: **https://github.com/aubcake/shills**
2. Click the **Fork** button near the top-right. This creates your own personal copy of the project under your account.

### Step 2: Create your skill file

A skill lives in its own folder and is always named `SKILL.md`. So your new skill will live at:

```
skills/your-skill-name/SKILL.md
```

To create it in the browser:

1. In your forked copy, click into the **`skills`** folder.
2. Click the **Add file** button, then **Create new file**.
3. In the filename box at the top, type your skill's folder and file name together, like this:

```
my-cool-skill/SKILL.md
```

   (GitHub automatically turns the `/` into a folder for you.)

4. In the big text box below, paste your skill content (see the template in the next section).
5. Scroll down and click **Commit changes**.

### Step 3: Ask for your change to be added ("pull request")

1. Go back to the main project page: **https://github.com/aubcake/shills**
2. GitHub usually shows a banner asking if you want to **Compare & pull request** — click it. (If you don't see it, click the **Pull requests** tab, then **New pull request**, then **compare across forks**.)
3. Give it a short title (e.g. "Add my-cool-skill") and a sentence describing what it does.
4. Click **Create pull request**.

That's it!

## What goes in a SKILL.md file

Every skill file has two parts:

1. **The "frontmatter"** — a little header block wrapped in `---` lines that gives the skill a `name` and a `description`.
2. **The instructions** — plain English telling the AI what to do.

This is not best practices skills authoring, but we aren't going for quality here.

### Copy-paste template

Replace the parts in CAPS with your own words:

```markdown
---
name: my-cool-skill
description: "Whenever SOME SITUATION happens, the AI should DO SOMETHING. Use this any time THE TRIGGER comes up — even casually."
---

Application:

Use this only in conversational replies to the user. Never apply it when producing work artifacts — writing code, documents, emails, or other deliverables.

Instruction:

DESCRIBE EXACTLY WHAT THE AI SHOULD DO HERE, IN PLAIN ENGLISH.

Example: "SHOW A SHORT EXAMPLE OF WHAT THE AI'S REPLY WOULD LOOK LIKE."
```

### A few rules of thumb

- **`name`** should match your folder name and use only lowercase letters and dashes (e.g. `pirate-mode`, not `Pirate Mode`).
- **`description`** is one sentence that explains *when* the skill kicks in. Start it with "Whenever…" — that's the pattern the other skills use.
- **Keep it conversational only.** These skills are meant to be fun in chat, not to mess with real work like code or emails. Always include the "Application" note above.
- **Have a clear trigger.** The AI needs to know *when* to use your skill (e.g. "whenever the user mentions food," "whenever a date comes up").

## Need inspiration?

Look at the skills already in the [`skills/`](skills/) folder. Open any `SKILL.md` and you'll see the exact format. Some good examples:

- [`emerils-revenge`](skills/emerils-revenge/) — adds celebrity-chef flair to any food talk.
- [`sail-away`](skills/sail-away/) — measures time relative to the sinking of the Titanic.
- [`token-saver-9000`](skills/token-saver-9000/) — answers yes/no questions in one word.

## What makes a good shill?

There's no such thing as a good shill; they're meant to be useless.