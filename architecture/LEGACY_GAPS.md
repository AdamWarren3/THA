# THA — Legacy Gaps

*This document is part of THA's development architecture. It is intended for maintainers rather than readers and is not part of the framework itself.*

Historical record of architectural mismatches that predated the ADR they conflict with. Entries are never deleted — closed gaps stay logged with a reference to the task that resolved them.

---

## LG-001 — Navigation sidebar duplicated Index metadata

**Predates:** ADR-001
**Status:** Open
**Description:** The navigation sidebar in index.html is a second, independently-authored copy of note id / number / title / tag — the same information already held in the `notes` array. Written before ADR-001 existed. Not a violation — a gap to close.
**Closed by:** IT-001
