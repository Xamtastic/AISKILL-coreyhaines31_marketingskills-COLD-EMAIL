# AISKILL-coreyhaines31_marketingskills-COLD-EMAIL

**Cold Email Writing** — Writes B2B cold outreach emails and multi-touch follow-up sequences that get replies — subject lines, opening lines, personalization, and CTAs grounded in proven frameworks and benchmarks.

Writes B2B cold outreach emails and multi-touch follow-up sequences designed to get replies — subject lines, opening lines, personalization, and CTAs grounded in proven frameworks and benchmarks, not generic AI-written boilerplate. Reads optional business context automatically from a `product-marketing.md` file in the working directory, if one exists, before writing begins.

Reach for this whenever an SDR, founder, or marketer needs a cold email — or a full multi-touch sequence — written for a specific prospect and offer, and wants it grounded in tested framework and benchmark data rather than a generic pitch. Pure-instructional: no scripts run, nothing to install.

Converted from coreyhaines31/marketingskills with its original MIT license preserved unchanged, and carries the same SYSTEM.md external-registry verification as every other package in this ecosystem.

| | |
|---|---|
| Version | `1.0.1` |
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

1. Download `COLD-EMAIL-1.0.1.aiskill` from the [Releases](https://github.com/Xamtastic/AISKILL-coreyhaines31_marketingskills-COLD-EMAIL/releases) page
2. Give your AI agent the skill package and describe who you're writing to and what you're offering, e.g.:

```
Using the Skill Package at /path/to/COLD-EMAIL-1.0.1.aiskill,
write a cold email to VP Eng at a Series B startup about our observability tool.
```

---

## Inputs

No structured input file. If `.agents/product-marketing.md` (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md`) exists in the working directory, it's read automatically for business context before writing begins.

---

## Output

A cold email (or sequence) with subject line, opening, body, and CTA — plus, when requested, a multi-touch follow-up sequence.

---

## Skill Archive Contents

```
COLD-EMAIL-1.0.1.aiskill  (ZIP archive)
├── manifest.yaml          # identity & metadata
├── SYSTEM.md              # verification protocol (invariant)
├── SKILL.md               # AI entry point — writing procedure
├── README.md              # this file — byte-identical to the repo-root copy
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
