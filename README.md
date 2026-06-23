# Augmentable.ai Agent Skills

**TPSReport by [Augmentable.ai](https://augmentable.ai)** — official agent skills for [TPSReport](https://tpsreport.pro) and related workflows.

## Skills

| Skill | Path | Install |
|-------|------|---------|
| **TPSReport KB generation** | [`skills/tpsreport-knowledge-base-generation/`](skills/tpsreport-knowledge-base-generation/) | `npx skills add augmentableai/skills --skill tpsreport-knowledge-base-generation -y` |

## Repo layout

agentskill.sh indexes **`skills/{name}/SKILL.md`** (same pattern as [affaan-m/seo](https://agentskill.sh/@affaan-m/seo) and elophanto/studio-operations):

```text
augmentableai/skills/
├── README.md
└── skills/
    └── tpsreport-knowledge-base-generation/
        ├── SKILL.md
        ├── scripts/kb_lint.py
        └── references/
    └── (future-skill-here/)
```

## agentskill.sh submit

**Repo:** `augmentableai/skills`

**Direct URL:**
`https://raw.githubusercontent.com/augmentableai/skills/main/skills/tpsreport-knowledge-base-generation/SKILL.md`

## Validate a KB

```bash
python skills/tpsreport-knowledge-base-generation/scripts/kb_lint.py /path/to/Your_KB/
```

## License

MIT · Copyright (c) Augmentable.ai
