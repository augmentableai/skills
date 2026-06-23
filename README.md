# Augmentable.ai Agent Skills

**TPSReport by [Augmentable.ai](https://augmentable.ai)** — official agent skills for [TPSReport](https://tpsreport.pro) and related workflows.

## Skills

| Skill | Path | Install |
|-------|------|---------|
| **TPSReport KB generation** | [`skills/tpsreport-knowledge-base-generation/`](skills/tpsreport-knowledge-base-generation/) | `npx skills add augmentableai/skills --skill tpsreport-knowledge-base-generation -y` |

## Repo layout

```text
augmentableai/skills/
├── README.md
└── skills/
    └── tpsreport-knowledge-base-generation/
        ├── SKILL.md
        ├── references/kb_lint.py
        └── evals/evals.json
    └── (future-skill-here/)
```

## Validate a KB

```bash
python skills/tpsreport-knowledge-base-generation/references/kb_lint.py /path/to/Your_KB/
```

## Related repos

| Repo | Purpose |
|------|---------|
| [tpsreport-obsidian-sync](https://github.com/augmentableai/tpsreport-obsidian-sync) | Obsidian plugin + install guides / examples |
| [tpsreport.pro](https://tpsreport.pro) | Product home |

## License

MIT · Copyright (c) Augmentable.ai
