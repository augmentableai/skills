# Augmentable.ai Agent Skills

**TPSReport by [Augmentable.ai](https://augmentable.ai)** — official agent skills for [TPSReport](https://tpsreport.pro) and related workflows.

One repo, one folder per skill. Add more skills as sibling folders over time.

## Skills

| Skill | Folder | Install |
|-------|--------|---------|
| **TPSReport KB generation** | [`tpsreport-knowledge-base-generation/`](tpsreport-knowledge-base-generation/) | `npx skills add augmentableai/skills --skill tpsreport-knowledge-base-generation -y` |

## Repo layout

```text
augmentableai/skills/
├── README.md
└── tpsreport-knowledge-base-generation/
    ├── SKILL.md
    ├── scripts/kb_lint.py
    └── references/
```

## agentskill.sh submit

Submit the repo (not a single file):

```text
augmentableai/skills
```

Direct URL for this skill:

```text
https://raw.githubusercontent.com/augmentableai/skills/main/tpsreport-knowledge-base-generation/SKILL.md
```

## Validate a KB

```bash
python tpsreport-knowledge-base-generation/scripts/kb_lint.py /path/to/Your_KB/
```

## Also bundled in

[TPSReport Obsidian plugin](https://github.com/augmentableai/tpsreport-obsidian-sync) (`tpsreport-skill/` copy — sync separately).

## License

MIT · Copyright (c) Augmentable.ai
