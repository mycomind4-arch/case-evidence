# Research Memory

> **Start here in a new chat.** Read this file first, then read [the operating protocol](docs/OPERATING-PROTOCOL.md), [the dossier index](research/INDEX.md), and the dossier relevant to the user's request. Use the dossier to restore context; verify any time-sensitive claim from current primary sources before relying on it.

This repository is a durable, source-grounded context system for research conducted with an AI assistant. It is designed to be loaded on demand in a new conversation.

## Load sequence

1. Read this README.
2. Read [docs/OPERATING-PROTOCOL.md](docs/OPERATING-PROTOCOL.md) for behavior and evidence rules.
3. Read [research/INDEX.md](research/INDEX.md) to find the relevant topic.
4. Read the topic's `BRIEF.md`, then its claims, sources, timeline, and open questions as needed.
5. Tell the user what context was loaded and flag any stale or unresolved facts.

If the full repository cannot be loaded, use `research/INDEX.md` and the relevant topic's `BRIEF.md` as the compact context package. Ask for the specific dossier files only if essential evidence is missing.

## What this system preserves

- The user's research question and scope
- A dated timeline of claims and events
- A claim ledger with explicit evidence status
- Source records, provenance, and limitations
- Distinctions between observation, source assertion, inference, and speculation
- Corrections to prior assistant answers
- Open questions and next research actions
- Conversation behavior that keeps analysis candid, careful, and useful

## Repository map

- `docs/OPERATING-PROTOCOL.md` — instructions for any assistant loading this repository
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

This repository is currently public. Do not put personal identifiers, private correspondence, medical records, credentials, or other sensitive material here. If a topic requires sensitive evidence, redact it or move that work to a private repository before adding it.
