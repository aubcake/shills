# shills

A curated collection of useless agent skills.

## Skills

| Skill | What it does |
|-------|--------------|
| [**emerils-revenge**](skills/emerils-revenge/) | Get unsolicited advice from celebrity chef Emeril Lagasse. |
| [**farmer-wisdom**](skills/farmer-wisdom/) | Puts a tiny farmer in your command line. |
| [**kobayashi-special**](skills/kobayashi-special/) | Everything is relative to hot dogs. |
| [**lizard-people**](skills/lizard-people/) | They live. |
| [**permanent-pedometer**](skills/permanent-pedometer/) | Update with your shoe size to get all distances in steps.|
| [**sail-away**](skills/sail-away/) | Dates and time spans are expressed relative to the sinking of the Titanic. |
| [**token-saver-9000**](skills/token-saver-9000/) | One word answers for yes/no questions.|

### Skill interactions

- **kobayashi-special** handles short lengths; **permanent-pedometer** handles long distances. They cross-reference each other.
- **farmer-wisdom** does not apply when **token-saver-9000** is invoked — you cannot reckon in one word.

All skills apply only to conversational replies, not to work artifacts (code, docs, emails, etc.).

These are markdown instructions that tell the AI how to behave in specific situations. They work exactly as designed (which is to say they are _not_ designed to help you get work done).

## Install

### Option 1: npx (all platforms)

Install shills with a single command:

```bash
npx skills add aubcake/shills
```

This works across **Cursor**, **Claude Code**, **Codex**, **Gemini CLI**, **Google Antigravity**, **OpenClaw**, **Pi**, and any other agent that supports the open [Agent Skills](https://agentskills.io/) standard.

### Option 2: GitHub CLI (`gh skill`)

If you use the [GitHub CLI](https://cli.github.com/) (v2.90.0+), you can install skills with [`gh skill`](https://github.blog/changelog/2026-04-16-manage-agent-skills-with-github-cli/):

```bash
# Browse and install interactively
gh skill install aubcake/shills

# Install a specific skill directly
gh skill install aubcake/shills emerils-revenge

# Target a specific agent host
gh skill install aubcake/shills --agent cursor
gh skill install aubcake/shills --agent claude-code
gh skill install aubcake/shills --agent codex
gh skill install aubcake/shills --agent gemini
```

`gh skill` automatically installs to the correct directory for your agent host and records provenance metadata for supply chain integrity.

#### Version pinning

Pin to a specific release tag or commit SHA for reproducible installs:

```bash
# Pin to a release tag
gh skill install aubcake/shills --pin v1.0.0

# Pin to a commit SHA
gh skill install aubcake/shills --pin abc123def
```

#### Keeping skills up to date

```bash
# Check for updates interactively
gh skill update

# Update all installed skills
gh skill update --all
```

### Other Agent Skills hosts (OpenClaw, Pi, Hermes, …)

`npx skills add` (Option 1) installs into the shared `~/.agents/skills/` convention, and any compliant client that scans that directory discovers the skills automatically. Project-scoped installs land in `.agents/skills/`. To install without the CLI, clone straight into either location:

```bash
git clone https://github.com/aubcake/shills.git ~/.agents/skills/shills   # user-level
git clone https://github.com/aubcake/shills.git .agents/skills/shills    # project-level
```

**Hermes** uses its own registry instead of the shared directory, so add the repo as a tap:

```bash
hermes skills tap add aubcake/shills
```

**That's it!** Your agent will automatically discover the skills and use them when relevant. You can also invoke any skill manually by mentioning the skill name in your prompt. 

## Add your own

Each skill follows the standard layout:

```
skills/your-skill-name/
└── SKILL.md
```

The `SKILL.md` needs YAML frontmatter with `name` and `description`, plus instructions in the body. See Cursor's [skill docs](https://cursor.com/docs/agent/skills) for the full format.

New to this and don't write code? No problem — [CONTRIBUTING.md](CONTRIBUTING.md) walks you through adding a skill entirely in your browser, step by step.

The bar is low. The bar is also on the floor. That's the point.

## Contributing

Anyone can add a skill — no coding required. See [CONTRIBUTING.md](CONTRIBUTING.md) for a step-by-step, browser-only guide that walks you through it from start to finish.

## License

MIT — see [LICENSE](LICENSE).
