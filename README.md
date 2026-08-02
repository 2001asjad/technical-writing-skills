# Technical Writing Skills

Claude skills for developer-facing technical writing — reviewing drafts for authenticity and scaffolding documentation the right way.

## Skills

### deslop-reviewer

Reviews technical content — tutorials, how-to guides, API docs, READMEs, blog posts — for the writing patterns that make prose read as AI-generated rather than practitioner-written. Flags filler, contrast framing, narrated code, marketing language, manufactured stakes, and 25 other tells, then proposes a concrete rewrite for each. Groups findings by severity so you fix the loudest tells first.

```
deslop-reviewer/
├── SKILL.md
└── references/
    ├── warning-signs.md
    └── severity.md
```

### diataxis-scaffolder

Scaffolds a new documentation page in the correct Diátaxis mode. Classifies the intent first — tutorial, how-to, reference, or explanation — then generates a mode-appropriate skeleton with section headings, guidance notes, and the boundaries that keep the page from drifting into another mode. Built to catch the most common documentation mistake: mixing types on one page.

```
diataxis-scaffolder/
├── SKILL.md
└── references/
    └── modes.md
```

## Using these skills

Each skill is a self-contained folder with a `SKILL.md` at its root and a `references/` folder for supporting material. To use one, drop its folder into your Claude skills directory:

- **Claude Desktop / Claude.ai** — add the skill through the Skills settings, or place the folder in your skills directory.
- **Claude Code** — put the folder under `.claude/skills/` in your project (or your user-level skills directory).

Claude reads each skill's `description` to decide when to invoke it, and loads the `references/` files on demand as it works.

## License

MIT
