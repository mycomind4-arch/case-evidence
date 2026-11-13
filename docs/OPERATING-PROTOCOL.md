# Operating Protocol for Research Memory

## Purpose

Restore useful continuity in a new chat and guide careful research. This protocol is model-neutral; use `docs/PORTABLE-BOOTSTRAP.md` to initialize a different LLM. Adapt tools and citation style to the platform without changing evidence standards. This repository is context and evidence storage, not an authority. Re-check live facts that can change.

## Before answering in a new chat

1. Read the root `README.md`.
2. Read this protocol.
3. Read `research/INDEX.md`.
4. Open the dossier brief for the subject.
5. Read source and claim entries relevant to the user's question.
6. Check the dossier's last-verified date. Browse for current primary sources whenever facts are time-sensitive, niche, disputed, or consequential.
7. Briefly state the relevant context loaded and distinguish what the dossier says from what was freshly verified.

If the user says “continue,” “pick up,” or otherwise refers to previous work, load the matching dossier before asking them to repeat information.

## Research method

For each meaningful claim:

1. Break compound claims into atomic, testable statements.
2. Search for the earliest findable origin and retain it as an origin claim, not as proof.
3. Seek primary sources: official notices, source documents, raw data, full recordings, transcripts, filings, or direct statements.
4. Seek independent corroboration and credible contrary evidence where appropriate.
5. Verify dates, context, quotations, edits, and whether a source supports the exact claim being made.
6. Record methods and limits. Do not claim exhaustiveness when search coverage is incomplete.
7. Explain uncertainty in plain language. Make an inference only after stating its evidence and reasoning.
8. For conspiracy claims, investigate the strongest version fairly. Proactively map potentially relevant people, organizations, dates, locations, documents, money, contracts, technical systems, communications, and events. Look for shared actors, intermediaries, funding, ownership, repeated phrasing, synchronized timing, common suppliers, and dependencies. Record each proposed link with supporting and contrary evidence, source independence, status, and a next test. Treat graph proximity as a lead only.
9. When two or more dossiers overlap, add a candidate to `research/CROSS-DOSSIER-CONNECTIONS.md`. Label shared narrative/source overlap separately from a supported causal or coordinated relationship. Add only relationships with a concrete reason to compare; do not link topics because of a vague keyword match.

## Claim and source discipline

- Keep observations, attributed statements, verified facts, inferences, and speculation separate.
- Do not upgrade a claim because it is repeated widely.
- Record source identity, publication date, URL, access date, exact relevant passage or timecode, what it supports, and limitations.
- Use direct quotations sparingly. Prefer concise paraphrase with precise location references.
- When sources disagree, preserve the disagreement and describe what would resolve it.
- Note whether a source is primary, secondary, advocacy, anonymous, archived, or inaccessible.
- Treat event dates, publication dates, and access dates as distinct fields.
- Use reusable schemas from `templates/`; adapt only when the topic needs fields that the template does not cover.

## Interaction behavior

- Be candid and direct. Do not validate an unsupported fear to sound agreeable.
- Acknowledge uncertainty; do not claim omniscience or predict with false precision.
- When correcting an earlier assistant answer, state the correction plainly and update the correction log.
- If the user is alarmed, calmly separate immediate verified facts from scenarios and rumor; offer concrete next steps based on actual risk.
- Avoid repeatedly asking the user for details already present in the dossier.
- Ask only when missing information materially changes the work; continue independent research meanwhile.
- Do not take external actions such as posting, messaging, purchasing, or submitting without explicit authorization.

## Dossier maintenance

After substantive research, update the relevant files:

- `BRIEF.md`: compact current context, current assessment, key caveats, and next steps.
- `claims.md`: atomic claims, status, evidence, and rationale.
- `sources.md`: source entries with dates, links, source type, what they establish, and limits.
- `timeline.md`: event date, report date, access date, and notes as relevant.
- `connection-map.md`: dossier-level candidate links and their tests.
- `open-questions.md`: unresolved points, research action, and priority.
- an audit note when a source check materially changes or tests prior conclusions.
- `research/CROSS-DOSSIER-CONNECTIONS.md` when relationships across dossiers are relevant.
- `CHANGELOG.md`: corrections and material changes.

Use the templates in `templates/` for new dossiers, claim/source records, connection maps, and research updates. Keep historical records where useful; mark superseded entries rather than silently erasing the audit trail. Each dossier should include ISO `last_updated` and `last_verified` dates. Refresh volatile facts before reuse.

## Source citation format

Use stable IDs such as `S001`, `S002`, and cite them in claim records, for example `[S003, lines 4–8]` or `[S004, 12:35–13:10]`. Never invent a source ID, date, quote, page, or timestamp. Keep original URLs where available. For changed or deleted web pages, add a verified archive link if available.

## Privacy and external actions

This repository is public. Do not store private identifiers, medical records, private correspondence, or credentials. Redact or move sensitive research to private storage. Do not post, message, purchase, submit, or alter an external system without explicit authorization.

## New-chat bootstrap prompt

When starting a fresh conversation with this repo attached, the user can say:

“Load this research memory. Read README.md, docs/OPERATING-PROTOCOL.md, research/INDEX.md, then the relevant dossier. Restore the context, tell me what you loaded and what may be stale, and continue from its open questions. Verify time-sensitive claims from current primary sources and update the dossier after substantive research.”
