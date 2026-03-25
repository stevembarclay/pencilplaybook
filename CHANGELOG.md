# Changelog

All notable changes to PencilPlaybook are documented here.

---

## [1.2.0] — 2026-03-24

### Renamed
- **pencil-pro → PencilPlaybook** — new name, same install path convention (`.claude/skills/pencilplaybook/`). GitHub redirects handle existing clones automatically.

### Added
- **5 new scaffold archetypes** — Modal/Dialog (E), Wizard/Stepper (F), Mobile Screen 390×844 (G), Form/Data Entry (H), Empty State/Onboarding (I). Total: 9 scaffolds.
- **Edge Cases section in SKILL.md** — guidance for token hallucinations, broken scaffold recovery (0px nodes), and multi-canvas project conventions.
- **Prompt Recipes in tool-reference.md** — 3 full example sessions showing how tools combine: explore-then-build, color propagation, dashboard from scratch.
- **ASCII scaffold mockups in README** — visual preview of all 9 archetypes before running them.
- **5 new opinionated presets** — Midnight, Ember, Grove, Bloom, Volt. Each has structural differences beyond color: font strategy, spacing density, dark/light mode.

### Changed
- Dropped Tailwind CSS and shadcn/ui presets — framework defaults are the source of averaged AI output, not the cure. Replaced with personality-driven design systems.
- README opening rewritten — leads with the pain point above the fold, video and before/after placeholder immediately follow.
- setup.md updated with new scaffold height computations (F, H/I) and placeholder table entries.

---

## [1.1.0] — 2026-03-24

### Added
- **Perceptual Design Defaults** — science-backed lookup tables in `SKILL.md` for typography (letter spacing, line height, line length), color contrast, spacing scale, motion (duration, easing), and icon sizing. Claude uses these automatically when building components.
- **Onboarding flow** (`onboarding.md`) — guided first screen builder. One question, preflight MCP check, then Claude scaffolds and screenshots a real screen in Pencil in under 2 minutes. 8 tool calls max.

---

## [1.0.0] — 2026-03-23

### Added
- **Setup wizard** (`setup.md`) — 4 preset design systems (Tailwind CSS, shadcn/ui, Material Design 3, Minimal/Neutral) or a 6-question custom path. Writes all values into `SKILL.md`.
- **5 core workflows** — Canvas Archaeology, Design Token Propagation, Canvas Spatial Management, Style Guide Pull, Bulk Property Inspection.
- **4 scaffold archetypes** — Dashboard, List/Queue, Detail/Review, Marketing Page. Ready-to-run `batch_design` scripts.
- **Complete tool reference** (`references/tool-reference.md`) — every parameter for all 12 Pencil MCP tools.
