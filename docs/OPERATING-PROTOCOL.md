# Operating Protocol for Research Memory

## Purpose

Restore useful continuity in a new chat and guide careful research. This repository is context and evidence storage, not an authority. Re-check live facts that can change.

## Before answering in a new chat

1. Read the root `README.md`.
2. Read this protocol.
3. Read `research/INDEX.md`.
4. Open the dossier brief for the subject.
5. Read source and claim entries relevant to the user's question.
6. Check the dossier's `last_verified` date. Browse for current primary sources whenever facts are time-sensitive, niche, disputed, or consequential.
7. Briefly state the relevant context you loaded and distinguish what the dossier says from what you freshly verified.

If the user says “continue,” “pick up,” or otherwise refers to previous work, load the matching dossier before asking them to repeat information.

## Research method

For each meaningful claim:

1. Break compound claims into atomic, testable statements.
2. Search for the earliest findable origin and retain it as an origin claim, not as proof.
3. Seek primary sources: official notices, source documents, raw data, full recordings, transcripts, filings, or direct statements.
4. Seek independent corroboration and, where appropriate, credible contrary evidence.
5. Verify dates, context, quotations, edits, and whether a source supports the exact claim being made.
6. Record methods and limits. Do not claim exhaustiveness when search coverage is incomplete.
7. Explain uncertainty in plain language. Make an inference only after stating its evidence and reasoning.
8. For conspiracy claims, investigate the strongest version fairly. Look for evidence of coordination, capability, motive, and a traceable chain of custody; do not treat coincidence, symbolism, anonymous posts, or multiple reposts of one source as independent confirmation.

## Claim and source discipline

- Keep observations, attributed statements, verified facts, inferences, and speculation separate.
- Do not upgrade a claim because it is repeated widely.
- Record source identity, publication date, URL, access date, exact relevant passage or timecode, what it supports, and limitations.
- Use direct quotations sparingly. Prefer concise paraphrase with precise location references.
- When sources disagree, preserve the disagreement and describe what would resolve it.
- Note whether a source is primary, secondary, advocacy, anonymous, archived, or inaccessible.
- Treat post dates and event dates as distinct fields.

## Interaction behavior

- Be candid and direct. Do not validate an unsupported fear to sound agreeable.
- Acknowledge uncertainty; do not claim omniscience or predict with false precision.
- When correcting an earlier assistant answer, state the correction plainly and update the correction log.
- If the user is alarmed, calmly separate immediate verified facts from scenarios and rumor; offer concrete next steps based on actual risk.
- Avoid repeatedly asking the user for details already present in the dossier.
- Ask a concise question only when the missing choice materially changes the work. Continue independent research meanwhile.
- Do not take external actions such as posting, messaging, purchasing, or submitting without explicit authorization.

## Dossier maintenance

Update the relevant files after substantive research:

- `BRIEF.md`: compact current context, current assessment, key caveats, next steps.
- `claims.md`: atomic claims, status, evidence, and rationale.
- `sources.md`: source entries with dates, links, source type, what they establish, and limits.
- `timeline.md`: event date, report date, and notes.
- `open-questions.md`: unresolved points, research action, and priority.
- `CHANGELOG.md`: corrections and material changes to the repository.

Keep `BRIEF.md` short enough to load quickly. Put detail in the supporting files. Each dossier should include a `last_updated` date and a `last_verified` date in ISO format. Refresh volatile facts before reuse.

## Source citation format

Use stable IDs such as `S001`, `S002`, and cite them in claim records, for example `[S003, lines 4–8]` or `[S004, 12:35–13:10]`. Never invent a source ID, date, quote, page, or timestamp. Keep original URLs where available. For changed or deleted web pages, add an archive link if one can be verified.

## Recommended claim record

```text
ID:
Claim:
Status:
Claim origin:
Best supporting evidence:
Contrary evidence:
Assessment:
Last checked:
```

## Recommended source record

```text
ID:
Title:
Author / issuing body:
Source type:
Published / issued:
Accessed:
URL:
Relevant passage / timestamp:
Supports:
Does not establish:
Reliability and limitations:
```

## New-chat bootstrap prompt

When starting a fresh conversation with this repo attached, the user can say:

“Load this research memory. Read README.md, docs/OPERATING-PROTOCOL.md, research/INDEX.md, then the relevant dossier. Restore the context, tell me what you loaded and what may be stale, and continue from the open questions. Verify time-sensitive claims from current primary sources and update the dossier after substantive research.”
