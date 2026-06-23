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
        ├── references/kb_lint.py
        └── evals/evals.json
    └── (future-skill-here/)
```

## agentskill.sh submit

**Repo:** `augmentableai/skills`

**Direct URL (try this if repo import fails silently):**
`https://raw.githubusercontent.com/augmentableai/skills/main/skills/tpsreport-knowledge-base-generation/SKILL.md`

**Important:** [Connect GitHub](https://agentskill.sh) in your account settings before importing org repos (`augmentableai/*`). The UI often shows "failed" with no error when GitHub is not linked.

## Validate a KB

```bash
python skills/tpsreport-knowledge-base-generation/references/kb_lint.py /path/to/Your_KB/
```

## License

MIT · Copyright (c) Augmentable.ai
