# THA — Architecture Decision Records

*This document is part of THA's development architecture. It is intended for maintainers rather than readers and is not part of the framework itself.*

---

## ADR-001: Single Source of Truth

**Principle:** Every artifact has one authored source of truth. Every other representation is a derived view that is regenerated, never edited directly.

**Corollaries:**
- One owner per piece of information — no two artifacts store the same fact.
- Views never own data; they render it.
- Derived artifacts are regenerated from their source, never hand-edited.
- Navigation is independent of taxonomy — how readers move through THA is not dictated by how notes are tagged.
- Concepts are not notes — a Map node names an idea; it expands to the note IDs that elaborate it, but the idea and the note are different objects.
- Tags are metadata, not navigation — Core/Identity/Practice/Principles/Context/Tools classify notes; they don't have to be how readers browse them.
- Status is orthogonal to tags and concepts — a term's maturity (Established Principle / Working Model / Hypothesis / Working Term / Open Question) is a separate axis from which category or concept it belongs to.

**Artifact map:**

| Artifact | Authored Source | Derived View(s) |
|---|---|---|
| Index | `notes` data (id, num, title, tag) | Homepage grid, navigation sidebar, note metadata lookups |
| Definitions | Definition entries (term, meaning, status, linked note) | Definitions page |
| Map | Concept assignments (CONCEPTS.md) | Interactive concept map |
| Reading Paths | Path definitions (ordered note-ID sequences per reader question) | Reading Paths page |
| Dependency Graph | Existing note links (`showNote()` calls already inside note bodies) | Graph JSON / visualization |

Note: Dependency Graph owns no authored data of its own. Its source is the links already written inside notes — it is a pure derived view of content that lives elsewhere.

---

## Terminology

**Legacy Gap** — an architectural mismatch that predates the ADR it conflicts with. No blame; expected during maturation. Never disappears once logged — remains as historical record, marked Open or Closed (with a reference to the task that closed it). See LEGACY_GAPS.md.

**ADR Violation** — new work, written *after* an ADR existed, that fails to comply with it. Action: fix it, or consciously supersede the ADR. Reserved for future issues — everything currently logged predates ADR-001 and is therefore a Legacy Gap, not a Violation.

**Implementation Task** — actionable, concrete work that satisfies an ADR or closes a Legacy Gap. Disappears once completed, or moves to a completed archive. See IMPLEMENTATION_TASKS.md.

**Deferred Decision** — a choice consciously postponed until a stated trigger condition is met. Not a Legacy Gap (nothing predates a broken standard) and not an Implementation Task (nothing is being built now). Instances are logged, with their trigger condition, in DEFERRED_DECISIONS.md. Once triggered, a Deferred Decision resolves into either a new ADR or an Implementation Task — it does not simply get edited in place.

---

## Change log

- 2026-07-04 — ADR-001 established. Retroactively covers the Constructive Displacement rebuild (note renumbering, duplication cleanup in Peace is the Protocol / Sovereign Signal) and the five-artifact Guidebook architecture: Index, Definitions, Map, Reading Paths, Dependency Graph.
- 2026-07-04 — THA Architecture v1.0 frozen. Further changes expected from implementation experience, not further design review.
- 2026-07-04 — Deferred Decision term added; DD-001 (contributor architecture) logged in DEFERRED_DECISIONS.md.
