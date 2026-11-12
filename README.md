# Research Memory

> **Start here in any new chat.** Attach this repository or provide its files. Use [the portable bootstrap prompt](docs/PORTABLE-BOOTSTRAP.md), then read [AGENTS.md](AGENTS.md), [the operating protocol](docs/OPERATING-PROTOCOL.md), [the dossier index](research/INDEX.md), and the dossier relevant to the user's request. Verify time-sensitive claims from current primary sources before relying on them.

This is a model-neutral, source-grounded research memory for restoring context and behavior across different LLMs. It stores the common research method and evidence record; each LLM must use the tools available in its current environment and must not pretend to have capabilities it lacks.

## Load sequence

1. Attach or provide this repository to the LLM.
2. Use the prompt in `docs/PORTABLE-BOOTSTRAP.md`.
3. Read this README, `AGENTS.md`, and `docs/OPERATING-PROTOCOL.md`.
4. Read `research/INDEX.md`, then the relevant topic's `BRIEF.md`.
5. Open claims, sources, timeline, and open questions as needed.
6. Tell the user what context was loaded and flag stale or unresolved facts.

To evaluate a fresh chat's ability to audit rather than merely retrieve context, use [the blind audit prompt](docs/BLIND-AUDIT-PROMPT.md). It asks the model to make an initial assessment before reading the prior audit.

If the full repository cannot be loaded, use the bootstrap file, index, and relevant brief as the compact context package. The user may need to attach or paste files depending on the LLM platform. This repository does not automatically connect to every LLM or persist in a model's memory by itself.

## What this system preserves

- The user's research question and scope
- A dated timeline of claims and events
- A claim ledger with explicit evidence status
- Source records, provenance, and limitations
- Distinctions between observation, source assertion, inference, and speculation
- Corrections to prior assistant answers
- Open questions and next research actions
- A consistent cross-model research behavior

## Repository map

- `AGENTS.md` — investigative research agent behavior
- `docs/PORTABLE-BOOTSTRAP.md` — copyable prompt for any LLM
- `docs/BLIND-AUDIT-PROMPT.md` — prompt for independent source audit in a fresh chat
- `docs/OPERATING-PROTOCOL.md` — detailed context restoration and evidence rules
- `research/INDEX.md` — topic directory and latest status
- `research/<topic>/BRIEF.md` — compact rehydration brief
- `research/<topic>/claims.md` — atomic claims and evidence status
- `research/<topic>/sources.md` — source log with dates and provenance
- `research/<topic>/timeline.md` — dated event and reporting timeline
- `research/<topic>/open-questions.md` — unresolved questions and next steps
- `CHANGELOG.md` — significant repository changes and corrections

## Evidence labels

Use these labels consistently:

- **Verified** — directly supported by reliable evidence, with a citation or source record.
- **Corroborated** — supported by multiple independent sources.
- **Contradicted** — reliable evidence conflicts with the claim.
- **Unverified** — evidence is insufficient or the source cannot be authenticated.
- **Inference** — a reasoned conclusion derived from stated evidence; explain the reasoning.
- **Speculation** — a possible explanation that currently lacks adequate evidence.
- **Unknown** — not established either way.

Never change a claim's status silently. Record why and when it changed.

## Privacy and safety

This repository is currently public. Do not put personal identifiers, private correspondence, medical records, credentials, or other sensitive material here. If a topic requires sensitive evidence, redact it or move that research to a private repository before adding it.
