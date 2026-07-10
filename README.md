# AISKILL-coreyhaines31_marketingskills-COLD-EMAIL

**Cold Email Writing** — Writes B2B cold outreach emails and multi-touch follow-up sequences that get replies — subject lines, opening lines, personalization, and CTAs grounded in proven frameworks and benchmarks.

| | |
|---|---|
| Version | `1.0.0` |
| License | `MIT` |
| Author | Xamtastic |
| Homepage | https://openaiskillpackage.com/ |
| Spec | [Open AI Skill Package Specification](https://openaiskillpackage.com/) |

---

## What This Skill Does

Writes B2B cold outreach emails and multi-touch follow-up sequences that get replies — subject lines, opening lines, personalization, and CTAs grounded in proven frameworks and benchmarks. Upgraded from a skill originally authored by [@coreyhaines31](https://github.com/coreyhaines31) on GitHub — see **Origin** below for the full provenance trail.

---

## Prerequisites

None — this is a pure-instructional skill. No scripts, no runtime dependencies.

---

## Quick Start

1. Download `COLD-EMAIL-1.0.0.aiskill` from the [Releases](https://github.com/Xamtastic/AISKILL-coreyhaines31_marketingskills-COLD-EMAIL/releases) page
2. Give your AI agent the following prompt:

```
Using the Skill Package at /path/to/COLD-EMAIL-1.0.0.aiskill,
[describe what you want the skill to do]
```

---

## Skill Archive Contents

```
COLD-EMAIL-1.0.0.aiskill  (ZIP archive)
├── manifest.yaml          # identity & metadata
├── SYSTEM.md              # verification protocol (invariant)
├── SKILL.md               # AI entry point — writing procedure
├── README.md              # this file (skill-level)
├── CHANGELOG.md           # version history
├── LICENSE.txt            # MIT (original author's license, preserved)
├── checksums.yaml         # SHA-256 integrity hashes
└── assets/
    └── references/
        ├── benchmarks.md
        ├── follow-up-sequences.md
        ├── frameworks.md
        ├── personalization.md
        └── subject-lines.md
```

---

## Origin

This package is a **converted** skill — not originally authored for the `.aiskill` format. Converted per the `.aiskill` v2.2.0 spec's [provenance rules](https://openaiskillpackage.com/#provenance):

- **Original repository:** [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)
- **Original skill path:** `skills/cold-email`
- **Converted:** 2026-07-10
- **Original license:** MIT (preserved unchanged, not re-licensed)

The `.aiskill`-specific files (`manifest.yaml`, `SYSTEM.md`, this README's packaging sections, `checksums.yaml`) were added during conversion. The skill's actual instructions (`SKILL.md`) and reference material are the original author's content, unmodified beyond format conversion (YAML frontmatter → `manifest.yaml`, directory renames per the mapping in `manifest.yaml`'s `source_*` fields).

---

## Development Workflow

To modify and repackage this skill:

```bash
# 1. Clone the source
git clone https://github.com/Xamtastic/AISKILL-coreyhaines31_marketingskills-COLD-EMAIL.git
cd AISKILL-coreyhaines31_marketingskills-COLD-EMAIL

# 2. Edit skill files in skill/
#    - skill/SKILL.md       — execution instructions
#    - skill/assets/        — scripts, references, templates

# 3. Run tests, if any (must pass before packaging)
python3 -m pytest skill/assets/tests/ -v

# 4. Package
python3 skill/assets/scripts/pack.py \
  --skill-dir skill/ \
  --dist-dir dist/

# 5. Bump version in skill/manifest.yaml, update skill/CHANGELOG.md

# 6. Commit, tag, and release
git add -A
git commit -m "feat: COLD-EMAIL v[NEW-VERSION]"
git push origin main
git tag v[NEW-VERSION]
git push origin v[NEW-VERSION]
gh release create v[NEW-VERSION] dist/COLD-EMAIL-[NEW-VERSION].aiskill \
  --title "v[NEW-VERSION]" --notes "..."
```

---

## Version History

See [CHANGELOG.md](CHANGELOG.md) for the full version history.

---

## License

MIT — original license from [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills), preserved unchanged. See [LICENSE](LICENSE).

---

## Contact

**Xamtastic**
For questions or issues with this conversion, open an issue on [GitHub](https://github.com/Xamtastic/AISKILL-coreyhaines31_marketingskills-COLD-EMAIL). For questions about the original skill content, see the [original repository](coreyhaines31/marketingskills).
