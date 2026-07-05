# THA — Implementation Tasks

*This document is part of THA's development architecture. It is intended for maintainers rather than readers and is not part of the framework itself.*

Active work items. Remove or archive once completed.

---

## IT-001 — Generate navigation from notes data

**Closes:** LG-001
**Status:** Open
**Description:** Replace the hardcoded navigation sidebar in index.html with a generated view, sourced from the `notes` array — the same pattern already used for the homepage note-grid. Group by `tag` first (Core, Identity, Practice, Principles, Context, Tools), then render each note within its section, preserving the current visual grouping. The `notes` array becomes the sole authored source for numbering, titles, tags, ordering, and navigation.
