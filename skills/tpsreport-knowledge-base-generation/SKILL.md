---
name: tpsreport-knowledge-base-generation
description: Builds, enriches, lints, and syncs TPSReport Obsidian knowledge bases with Graph RAG frontmatter. Use when authoring KB folders, YAML metadata, kb_lint validation, or TPSReport plugin push workflows.
---

# TPSReport KB Skill

**TPSReport by Augmentable.ai** — workflow skill for Obsidian knowledge bases synced to TPSReport.

## When to Use

Use this skill when:
- seeding or expanding a TPSReport knowledge base in Obsidian
- enriching YAML frontmatter (`summary`, `keywords`, `hyde_questions`, `retrieval_hint`, `description`, `seo_title`, `og_image`)
- validating metadata before push
- mapping folders and syncing via the TPSReport Obsidian plugin
- assessing KB coverage, duplicates, or retrieval quality after push

## Instructions

When activated, manage the full KB lifecycle: scope, seed, generate, enrich, validate, push, iterate.

1. Read `00_CONTEXT.md` for topic, audience, voice, and glossary.
2. Fill RAG + **web SEO** frontmatter using exact TPSReport plugin key names. See `references/METADATA.md`.
3. Validate with `python references/kb_lint.py YOUR_KB_FOLDER/` until exit 0 (includes `description` and RAG core).
4. User maps folder and syncs via the Obsidian plugin. Never push without explicit approval.
5. Test agent questions after push; fix under-retrieval and re-validate.

## Guardrails

- Never invent facts — derive from body or cited sources
- Never hand-edit plugin-managed keys (`node_id`, `sync_status`, `last_synced`, `tps_content_hash`)
- Never rewrite a finished doc's voice
- Never push without explicit user approval

## Resources

- `references/LIFECYCLE.md` — full workflow
- `references/METADATA.md` — key reference
- `references/kb_lint.py` — deterministic linter
- `references/metadata-contract.yaml` — validation contract

## Anti-patterns

- Synonym keys TPSReport ignores (`questions` instead of `hyde_questions`)
- Generic keywords that match everything
- Missing negative clause in `retrieval_hint`
- Missing `description` on content docs (web SEO)
- Using `summary` instead of a dedicated meta `description`
- Pushing before lint exits 0
