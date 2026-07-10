# Changelog — Cold Email Writing

All notable changes to this skill are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versions follow [Semantic Versioning](https://semver.org/).

---

## [1.0.1] — 2026-07-10

### Added
- **BREAKING** (`.aiskill` spec v2.3.0): new required manifest field
  `synopsis` — a multi-paragraph, hand-authored expansion of `description`,
  feeding both `README.md`'s opening and `CARD.md`'s rendering

### Fixed
- Repo-root `README.md` and `skill/README.md` had diverged since conversion
  (generated from two different templates) — merged into one
  byte-identical README, carrying the best content from both

## [1.0.0] — 2026-07-10

### Added
- Initial conversion from [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) (`skills/cold-email`, Agent Skills format) to `.aiskill` v2.2.0
- Original MIT license preserved verbatim in `LICENSE.txt`
- `SYSTEM.md` verification protocol v1.0.0 bundled per spec
