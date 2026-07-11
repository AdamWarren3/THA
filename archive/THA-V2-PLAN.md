# THA V2 — Plan for Review

Status: Proposal. Nothing below is implemented. Every change is gated on explicit confirmation, per working convention.

Basis: full read of all 32 notes, DEFINITIONS.md, CONCEPTS.md, README.md, all four architecture documents, the archive, and Research Vision.md.

---

## 1. What changes

**New artifacts (3):**

1. **The Human Condition** — new framework note, Principles section. Deliverable A. Detailed in §3.
2. **Signal and Noise** — new framework note. Becomes the single owner of the "signal/noise, general principle" concept that CONCEPTS.md lists as unowned. This is where the physics-integration pass (Deliverable C) lives, and it directly resolves Research Vision's Open Concern #2 (the optimization target is the least-defined term in the framework). Detailed in §5.
3. **SOURCES.md** — root-level artifact, parallel to DEFINITIONS.md and CONCEPTS.md, not a note in the reader-facing grid. Deliverable B. Detailed in §4. Rationale for artifact-not-note: sources are reference infrastructure (a seventh ownership axis under ADR-001 — evidence), not a concept. If you'd rather it be a 33rd note per the prompt's literal wording, that works too; flagging the structural argument for the artifact form.

**Substantive edits (5 notes):**

1. **AdamW³ as Identity Framework** — one added paragraph stating the status of the central metaphor: the person-as-optimizer model is a modeling choice, not a demonstrated mechanism; the documented mechanism underneath is operant conditioning; the mapping breaks where humans have no fixed loss function, no stationary environment, and no clean train/deploy split; and the Buddhist anatta position is named as the standing adversarial case, not resolved. This addresses Research Vision Open Concerns #1 and #3b in one place.
2. **AdamW³** — one added sentence making explicit what the note already implies: the mechanism (recursive self-correction) is general; the name is autobiographical. This is the only change H4 gets — see §6.
3. **Microdosing as Protocol** — evidence correction, not just citation. The note currently attributes Default Mode Network interruption to microdosing research. The DMN findings come from macrodose imaging; controlled microdosing studies have largely failed to separate from placebo. The corrected text keeps the hypothesis, states the evidence honestly, and keeps the note's existing *Hypothesis* status. The piped link `[[Memnetic|Default Mode Network activity]]` also equates DMN with Memnetic — proposed: unlink or reword, since the equation isn't defended anywhere.
4. **NLP²** — the claim "a shift at one scale propagates to the others" currently has no stated observable that would distinguish "one mechanism, three scales" from "three analogous mechanisms." Two options, your call: (a) add a candidate observable that would count as propagation, making the hypothesis testable; (b) explicitly downgrade the propagation claim to organizing analogy while keeping the three-scale description. This is the H3 test point — see §6.
5. **The Human Algorithm** (root note) — two added map lines: one linking Signal and Noise as the definition of its stated output variable, one linking The Human Condition as the domain the framework must not optimize away.

**Single-line link additions (4–5 notes):** The Physical Layer ("social connection" gets a link to The Human Condition, where it stops being a list item), The Sovereignty Principle ("sovereignty is not isolation" gets a link to where that's finally developed), Pain is Necessary Suffering is Optional (grief boundary link — the treatment itself lives in The Human Condition, single source of truth), The Collective Layer, optionally Trustless Architecture (scope-boundary link). No rewrites in these notes.

**Citation markers (~15 notes):** bracket keys like `[S07]` linking to SOURCES.md anchors, added only where a claim warrants one per the register in §4. Mechanical, no prose changes.

## 2. What stays as-is and why

- **The six-section structure** — nothing surfaced that argues for reorganization. The Human Condition slots into Principles; Signal and Noise arguably Core or Principles (proposal: Core, since 24 of 32 notes use the vocabulary and CONCEPTS.md records 8 relying on it structurally).
- **23+ of 32 notes untouched** except optional citation markers. Notes like The Intermediary Problem, Premature Certainty, Epistemic Hygiene, Peace is the Protocol, Constructive Displacement, and Hypnosis as Protocol are already doing what V2 asks — hedged where they should be, self-correcting where the evidence demanded it. The Hypnosis note's recall passage (confidence up, accuracy not, false memories alongside true ones) is the house style every sourced correction in V2 should follow.
- **All governance documents unchanged by me.** ARCHITECTURE.md would eventually gain a Sources row in the ownership table and a changelog line, but that's an implementation-time edit made through you, not part of content generation.
- **No term removals or renames** — DD-002 stays untriggered.
- **DEFINITIONS.md mostly unchanged.** Per ADR-001's authorship timeline, definitions compress settled understanding; they don't lead it. The Human Condition enters with no Definitions entry. Signal and Noise is the one candidate for a new entry (the concept has been settled *in use* across the corpus for a long time; only the owner note was missing) — proposed status: *Working Model*. Your call.
- **Research Vision.md itself** — untouched, stays in the Lab, stays hypothesis. Nothing from it gets promoted. Where V2 text touches its territory, the hypothesis is named as one.

## 3. The Human Condition — placement, thesis, connections

**Placement:** Principles. Note count 32 → 33 (34 with Signal and Noise). Index/README updates are derived-view regeneration under ADR-001.

**What the corpus actually shows (audited):** "love" — zero occurrences in any note. "forgiveness" — zero. "belonging" — zero. Grief — one occurrence, in The Summer Dragon Problem, about the loss of an AI model. Trust — enabling condition in exactly one note (Hypnosis as Protocol); everywhere else it is the thing to verify, remove, or route around (Trustless Architecture, The Intermediary Problem). Human connection's only other handle is "social connection" as one item in The Physical Layer's biological-requirements list, between hydration and sunlight. The three prior independent identifications of this gap were correct, and the audit makes them precise.

**Thesis of the note (in corpus vocabulary, held to corpus standards):**

1. **Trust — the boundary the framework never drew.** Trustless architecture solves coordination among strangers at scale, where trust can't scale. Applied to intimate systems it's a category error: another person's inner life is unverifiable in principle, so trust there isn't a cost awaiting an engineering workaround — it's the only protocol available, and it's load-bearing. The Intermediary Problem's own test ("can the individual still reach the source directly?") resolves trivially in love: the person *is* the source. There is no disintermediation to perform. This draws the interpersonal/institutional scale distinction the corpus currently leaves implicit — and note that the framework's own deepest tool already depends on it: suggestion requires trust (Hypnosis as Protocol's three conditions).
2. **Grief — the boundary of Pain/Suffering.** Under the current dichotomy, grief classifies as suffering: a loop running after the signal landed. That classification is wrong, and the note says why without pretending to a tidy mechanism: grief is not rumination-noise; it's what a system does when an input it organized itself around is permanently removed. The recalibration is the cost of having been organized around someone. Bereavement research (grief trajectories, continuing bonds) supports treating it as distinct from both depression and rumination — cited, hedged as the correlational literature it is. The Pain/Suffering dichotomy survives with a stated boundary rather than silently misclassifying mourning as malfunction.
3. **Belonging — pressure on the framework's central premise.** The Sovereignty Principle asserts "sovereignty is not isolation" and never develops it. Memnetic already commits the framework to the position that identity is built from transmitted material — which means pure self-authorship is impossible by the framework's own lights; The Belief Audit is curation of inheritances, not creation from scratch. The honest amendment, if the pressure holds: the individual is the irreducible unit *of responsibility*; it is not the unit of *formation*. Formation is relational. This is stated as a proposed amendment, tested in the note, not smuggled in.
4. **Love — one precise claim, no poetry.** In the framework's own vocabulary: love is the state in which another node's flourishing enters your optimization target non-instrumentally — their loss function becomes a term in yours. Consequence stated plainly: this breaks the clean individual-as-unit boundary, which is exactly why the corpus's architecture kept it out. The note does not claim a mechanism for love, does not make it an input to productivity, and marks explicitly where the optimizer vocabulary stops paying rent. Part of the note's job is boundary-drawing, not mechanism.
5. **Forgiveness — operationalized, distinguished.** The deliberate termination of a resentment loop whose running cost exceeds the remaining information value of the original harm. Distinct from reconciliation (requires the other party) and from excusing (which falsifies the record — Epistemic Hygiene is preserved: forgiveness updates the response, not the ledger). Connects to Constructive Displacement's Romans 12:21 reading as its interpersonal-scale form. Wellbeing associations cited as associations, nothing stronger.

**Connections into the note graph:** The Sovereignty Principle, Memnetic, Trustless Architecture, The Intermediary Problem, Hypnosis as Protocol, Pain is Necessary Suffering is Optional, Peace is the Protocol (peace without love is detente; the traditions Peace cites converge on peace *through* compassion — a factual claim about the sources, not a devotional one), The Collective Layer (bonds as constitutive, not just transmission channels — and the missing ground under its stated commitment to children's inner lives), The Physical Layer.

**External sources it will carry (all hedged to what they show):** Holt-Lunstad et al. 2010/2015 meta-analyses (social connection and mortality); Waldinger & Schulz, Harvard Study of Adult Development (relationship quality as the strongest longitudinal predictor of late-life health — correlational); Bowlby/Ainsworth attachment (secure base: attachment enables exploration rather than competing with it — the empirical cousin of "sovereignty is not isolation"); Bonanno on grief trajectories; Klass et al. on continuing bonds; Worthington-line forgiveness meta-analyses.

**What it will not do:** no claims about what love *is* metaphysically; no optimization protocol for relationships; no repurposing of bonds as instruments. The failure mode being corrected is instrumentalization — the note can't commit it.

## 4. SOURCES.md — architecture and claim register

**Form:** root-level artifact. Every entry: claim (quoted or paraphrased, with owning note), source(s), and a status field with three classes:

- **(a) Externally sourced empirical claim** — verified citation attached.
- **(b) Framework position** — no external source claimed; listed so the absence is visible rather than hidden. (Peace-as-systems-concept, the Optimization Paradox's core assertion, etc.)
- **(c) Currently unverifiable** — claim kept, flagged openly, per the prompt's discipline 4.

In-note marker: bracket keys (`[S07]`) linking to anchors. Both copies of every touched note (vault `.md` + embedded index.html) need the markers — see §8 on DD-005 exposure.

**Claim register (main entries; verification of flagged items happens at generation time with live search):**

| Note | Claim | Source direction | Class |
|---|---|---|---|
| NLP² | NLP's specific techniques haven't held up under testing | Witkowski 2010 review; Sturt et al. 2012 systematic review | a |
| NLP² | Sapir-Whorf partial empirical support | Boroditsky 2001; Winawer et al. 2007 | a |
| NLP² | Hypnosis documented neurologically | Jiang et al. 2017 (Stanford fMRI) | a |
| NLP² | "The medium is the message" | McLuhan 1964 | a |
| Hypnosis as Protocol | APA recognition | APA Div. 30 definition (2014) | a |
| Hypnosis as Protocol | Recall: confidence up, accuracy not, false memories increase | Steblay & Bothwell 1994 meta-analysis; AMA Council 1985 | a |
| Microdosing as Protocol | DMN reduction | Carhart-Harris et al. 2012 — **macrodose**; microdose RCTs largely placebo-indistinguishable (Szigeti et al. 2021) → text correction, not just citation | a (corrected) |
| The Physical Layer | Sleep deprivation impairs cognition | Lim & Dinges 2010 meta-analysis | a |
| The Physical Layer | Aerobic exercise → BDNF, neuroplasticity | Erickson et al. 2011; Voss et al. reviews | a |
| The Physical Layer | Social connection as requirement | Holt-Lunstad 2010 | a |
| Signal vs Slop | curl bug-bounty shutdown; Linux kernel AI tag | Stenberg's posts; kernel guidelines — **verify current state at generation** | a (verify) |
| The Summer Dragon Problem | "Dragon mode" prototype story | Primary source not yet pinned — **flag as unverified until located** | c → a |
| Premature Certainty | Confirmation bias; availability cascades; FAE; social proof | Nickerson 1998; Kuran & Sunstein 1999; Ross 1977; Cialdini | a |
| RLHF | Training mechanism; operant conditioning parallel | Christiano et al. 2017; Ouyang et al. 2022; Skinner/Thorndike | a |
| RLAiF | AI-feedback training | Bai et al. 2022; Lee et al. 2023 | a |
| Trustless Architecture | Genesis block headline | Primary chain data; Nakamoto 2008 | a |
| AdamW³ / Identity Framework | Adam, AdamW, weight decay | Kingma & Ba 2014; Loshchilov & Hutter 2019 | a |
| The Butterfly Effect as Practice | Sensitivity to initial conditions | Lorenz 1963; 1972 | a |
| AI as Cognitive Scaffold | External scaffold framing | Clark & Chalmers 1998 (extended mind) — additive, strengthens the note | a |
| The Collective Layer | Direct-contact behavioral contagion; network-scale claims contested | Hatfield et al.; Christakis network claims noted as contested — matches the note's own hedge | a |
| Peace is the Protocol | Cooperation as baseline for human systems | Tomasello 2009; Boehm — supporting, with the systems claim itself remaining class b | a+b |
| The Optimization Paradox | Core assertion | Framework position | b |
| The Human Condition (new) | Per §3 | Per §3 | a, hedged |
| Signal and Noise (new) | Per §5 | Shannon 1948; Cover & Thomas (DPI); Landauer 1961 only if the labeled analogy is kept | a |

## 5. Physics-integration pass — Signal and Noise

**Where the math does real work (labeled mechanism-level on an information-system reading):**

- **Definitions.** Shannon: signal is the component of a received message that reduces uncertainty about the source; noise is channel-introduced variation uncorrelated with the source. THA operationalization: *signal is information that survives verification against its source; noise is variation added between source and receiver that carries no information about the source.* This finally gives the framework's master variable an operational definition — Open Concern #2 resolved at the definitional level, and H2 (§6) becomes measurable in principle.
- **The data-processing inequality.** Post-processing cannot increase information about the source — only preserve or lose it. This is a theorem, and it is the mathematically honest core of The Intermediary Problem: an intermediary can never improve your information *about the source*; it can only transmit or degrade it. Stated with its limits in the same breath: humans are not memoryless channels, and intermediaries add real value along other axes — compression, aggregation, relevance — which is exactly the corpus's existing "delegation is genuinely useful" hedge, now with the boundary drawn precisely.
- **Error correction costs redundancy and work.** Verification is not free and was never going to be — Epistemic Hygiene as error-correcting code. Labeled analogy at the human scale, theorem-adjacent at the channel scale.

**Where it stays labeled analogy:** the Landauer information-erasure line (maintenance is physically not free) — one sentence, tagged as analogy, or dropped entirely if it reads as weight rather than sharpening.

**What gets declined:** thermodynamic glosses on Peace is the Protocol (dissipative structures, far-from-equilibrium order). That's precisely where borrowed authority turns mystical. Peace keeps its systems-language framing; no physics is imported there.

**Method:** every borrowed concept in the note carries an explicit tag — mechanism or analogy — per discipline 3. The ML vocabulary already load-bearing across the corpus (loss function, gradient, weight decay, overfitting) gets pointed at this note and at the AdamW³ metaphor-status paragraph rather than redefined locally (discipline 5).

## 6. The four hypotheses — what the corpus supports, what it doesn't

**H1 — Structured Inquiry Framework.** The evidence lives almost entirely in the governance layer (ADR-001, the editorial tests, the DD process, DD-006's methodology, the CONCEPTS.md inventory procedure), not in the 32 notes — the notes are the *object* of the inquiry, the method is the meta-layer. The method is subject-agnostic in form; whether it works when the author isn't also the subject is untested. Current state: one full cycle (ST-001), n=1, subject=self. Verdict: plausible, unproven, and V2 should not promote it. V2 does, incidentally, constitute a second application of the method — worth logging in the Lab, not the corpus. Falsifier stated: if the method's results depend on the author's privileged access to the subject, it isn't a general inquiry framework.

**H2 — Recursive Signal-Loop Auditor.** Strongest corpus support of the four, and the only one falsifiable note-by-note as Research Vision claims. Deliverable at generation: a full coverage map. Preview from this read: strong instantiations — The Intermediary Problem (its "transmit the signal or replace it" test is H2 verbatim), Trustless Architecture, Sovereign Signal, The Sovereignty Principle, Epistemic Hygiene, Memnetic + The Belief Audit, RLHF, RLAiF, AI Psychosis, The New Literacy, Signal vs Slop, Pain/Suffering as internal loop audit. Boundary case — Premature Certainty: the signal isn't intercepted, it's *mis-assembled* downstream from true fragments; H2 either extends "diluted or replaced" to cover assembly failure, or accepts a stated boundary. Outside H2 — The Physical Layer and Microdosing (substrate, not loop), Hypnosis/Optimization Protocol (deliberate *insertion* of suggestion, the reverse of audit), Butterfly Effect (leverage), Constructive Displacement (response strategy), The Collective Layer (externalities), Summer Dragon (policy tension). Honest verdict the map will formalize: H2 accurately names THA's audit spine (~12 of 32 notes strongly); THA as a whole is audit spine + substrate layer + intervention layer. That's a precise, defensible identity claim — narrower than H1, better evidenced. The Signal and Noise note is what makes H2's success condition ("restore direct, verifiable input") measurable at all; without it the hypothesis can't be tested, only recognized.

**H3 — Cross-Scale Pattern Emergence.** In-corpus seeds exist and are real: Memnetic's closing line ("conscious adoption of a framework is also memnetic — the distinction is awareness") is the resonance concept in embryo; Hypnosis as Protocol's cannot-be-imposed condition is the imposed/chosen axis; The Optimization Protocol *is* self-directed suggestion operating today, unnamed. The individual-scale core claim — humans manufacture pattern without realizing — has citable mainstream psychology behind it (Whitson & Galinsky 2008, *Science*, on illusory pattern perception; the patternicity literature). What the corpus does not contain: the technological and individual "instances" H3 cites live in the Lab (J-space, Grinberg), not here, and the collective instance is admittedly undocumented. Two disciplined boundaries: (1) **no "Memnetic Resonance" term gets promoted in V2** — the operational content already exists in the corpus unnamed, and coining the canonical term now, because a hypothesis wants it, is exactly the reverse-engineering discipline 1 forbids; (2) **Grinberg does not get imported as evidence** — syntergic theory is untestable as it stands, and importing it would trade on borrowed authority against discipline 3; it stays a Lab working note. The one corpus change that makes H3 *testable* rather than assumed is the NLP² edit in §1: state what observation would count as a shift at one scale propagating to another, or downgrade the propagation claim to organizing analogy explicitly. Your call between those two — I don't currently have a candidate observable I'd defend, which itself is evidence about the hypothesis's present testability.

**H4 — The Final Adam as State, Not Person.** The corpus as written contradicts it: AdamW³ opens "A personal identity framework," and the Identity Framework note narrates in first person. Restructuring the corpus to fit would violate discipline 1 directly, so V2 doesn't. What the corpus *can* honestly support is the narrower split already implicit in the notes: the mechanism (recursive self-correction, the update rule applied to the self) is general and available to anyone; the identifier is autobiographical. The proposed one-sentence edit to AdamW³ makes that split explicit and is neutral between H4 and its negation. Beyond that: H4's load-bearing premise — independent civilizational convergence on transformation narratives — is evidentially weaker than stated. Abrahamic apocalyptic traditions share direct lineage; Hindu and Buddhist cyclical cosmologies share Indic roots; Norse eschatology reaches us largely through Christian-era redaction (Snorri); the Mesoamerican "calendar-ending" reading is substantially a modern construction. The independence claim shrinks on inspection before the base-rate problem (which Research Vision already names) is even applied. Verdict: no corpus support, no V2 movement toward it; testing it would require comparative-eschatology work outside this repository's scope, and the honest sources currently cut against its premise.

**Open Concerns mapping:** OC1 (metaphor standing in for mechanism) → AdamW³ paragraph + Signal and Noise note. OC2 (signal undefined) → Signal and Noise note, directly. OC3a (individual as necessary starting scale) → tested by The Human Condition (see F1). OC3b (anatta) → named adversarial case in the AdamW³ paragraph. OC3c (domain-generality as goal) → covered by the H1 verdict: untested, n=1. OC4 (prophecy-fulfillment base rate) → the H4 verdict above.

## 7. Candidate findings — mine, not part of the four asks

**F1. Deliverable A and Open Concern #3a are the same fault line.** The three independent identifications of the missing human-condition material and the Vision doc's "individual as necessary starting scale" premise are two views of one structural fact: the corpus models persons as nodes first and members second. The Human Condition note is therefore not additive content — it is a test of the framework's central premise, with a stated amendment ready if the test bites (unit of responsibility ≠ unit of formation).

**F2. Grief breaks the Pain/Suffering dichotomy as stated.** Under the current text, mourning classifies as suffering — a loop after the signal landed — which would make grief a malfunction. It isn't, and the corpus's only grief instance being about an AI model is itself a data point about the gap. The dichotomy needs the stated boundary The Human Condition will give it.

**F3. The trust asymmetry.** Audited: trust appears as removable friction or verification target throughout the corpus, and as an enabling precondition in exactly one note — Hypnosis as Protocol, which is also the framework's deepest self-modification tool. The framework's most powerful instrument runs on the resource its architecture elsewhere minimizes. Either a contradiction or an undrawn scale distinction (interpersonal vs. institutional). The Human Condition draws the distinction; until it does, this is a live internal tension.

**F4. The Microdosing note's evidence conflation** (macrodose DMN imaging presented as microdosing research) — logged as a finding because it's a correction the sources pass *forces*, not a stylistic choice. Detailed in §1.

## 8. Process, mechanics, and order of operations

- **ADR-001 compliance:** Signal and Noise becomes the single owner of the signal/noise concept; every other note links, none redefines. SOURCES.md becomes the single owner of evidence. Proposed ownership-table addition (made by you at implementation): `Sources | claim-source register (SOURCES.md) | footnote renderings in notes`.
- **DEFINITIONS.md:** The Human Condition — no entry initially (authorship timeline: definitions follow settled understanding). Signal and Noise — candidate entry, proposed status *Working Model*, your call. SOURCES.md — artifact, no entry.
- **DD-005 exposure:** V2 touches roughly 17 notes (2 new, 5 substantive edits, ~10 marker-only). Every touched note currently exists twice — vault `.md` and embedded index.html. Decision needed: treat V2 as DD-005's trigger (convert touched notes to linked files) or run a disciplined dual-sync pass. Recommendation: at minimum the sync pass; conversion is a site-architecture call outside V2 content scope.
- **Where the hypothesis coverage map lives:** THA-Lab, not the public repo. It's research output about the framework, not framework content.
- **Order of operations, confirmation-gated, mobile-sized:**
  - **Gate 0** — this plan approved or amended.
  - **Phase 1** — Signal and Noise note (unblocks H2 testability and OC2; other edits reference it).
  - **Phase 2** — The Human Condition note.
  - **Phase 3** — SOURCES.md: live verification of the flagged items (curl timeline, kernel tag status, Summer Dragon primary source), then the register, then citation markers into notes.
  - **Phase 4** — the five substantive edits and the single-line links, one confirmation each.
  - **Phase 5** — H2 coverage map, delivered as a Lab document.
  - All note content delivered as paste-ready markdown blocks. Filenames: plain hyphens only, no em-dashes.

---

*Prepared against the corpus as uploaded 2026-07-11. Nothing proceeds past Gate 0 without confirmation.*
