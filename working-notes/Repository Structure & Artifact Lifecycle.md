# Repository Structure & Artifact Lifecycle

## Observation

As THA grows, the repository is beginning to develop distinct classes of artifacts with different levels of authority. While individual artifacts are governed, the repository itself does not yet explicitly define the purpose or authority of each folder.

The introduction of `/working-notes` highlighted this distinction. It serves a fundamentally different role than `/notes`, `/articles`, or `/architecture`.

## Initial Thought

Rather than treating every document equally, the repository may benefit from defining the *authority* of each location.

For example:

- **/notes** — Canonical knowledge.
- **/articles** — Reader-facing narrative and exposition.
- **/architecture** — Governance, process, and repository operation.
- **/working-notes** — Drafts, experiments, observations, questions, and speculative ideas. Content here is intentionally non-canonical and may contradict itself.

The important distinction is not the folder itself, but the authority assigned to its contents.

## Possible Lifecycle

Working Note
↓
Experiment
↓
Evidence
↓
Review
↓
Canonical Artifact

Not every working note should graduate. Some may simply document an avenue that proved unproductive.

## Open Questions

- Should repository structure itself become part of the canonical architecture?
- Should folder authority be documented in `ARCHITECTURE.md`, `README.md`, or elsewhere?
- Does every folder require a defined lifecycle, or only canonical ones?
- Should future AI collaborators treat `/working-notes` differently from canonical artifacts by default?

## Status

Observation only.

No architectural decision is proposed at this time. Revisit if additional artifact types emerge or if contributors begin interacting with the repository without prior context.
