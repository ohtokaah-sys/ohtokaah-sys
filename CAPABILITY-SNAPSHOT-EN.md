# Capability Snapshot — an always-on AI operator, in plain language

> Version 1.0 · 2026-10-28 · English executive edition
> The full ledger (238 capability entries across 13 areas, in Chinese) is maintained separately; this page is the version you can hand to someone who has ten minutes.

## What this is

A hosted AI operator that runs on one machine and works through the tools a person already uses: it reads files, writes documents, keeps long-term context, runs scheduled jobs, and delivers results to a phone or a browser.

It is not a chat window. The person supplies the judgement; the system does the work around it — finding material, reading it, drafting, checking, delivering, filing.

Data, working notes and results stay on the machine. Only the understanding and generation steps use external model services.

## The problem it removes

Knowledge work is a chain: **find → read → judge → produce → deliver → file.**

Six of the seven steps do not need a human, but they consume most of the time. This system takes those six and pushes the person's time back into the middle step.

What changes in practice:
1. Several readings of the same material can be laid out side by side instead of trusting the first impression.
2. Why a decision was made three months ago is still retrievable, so it does not get re-argued.
3. Routine checks, backups and summaries do not depend on anyone remembering them.
4. Material that went in can be found again — "I think we have it somewhere" stops being a dead end.

## At a glance

| Measure | Value |
|---|---|
| Capability entries in the ledger | 238, across 13 areas |
| Ledger entries covered by this snapshot | 243 / 243 (100%, machine-checked) |
| Known limitations documented | 14 |
| Scheduled jobs running unattended | 209 (23 model-driven, 186 script-only) |
| Operating cost model | pay per use, no licence fee; balance alerts and a daily cost report |

## Capability map

| # | Area | What it covers | Entries |
|---|---|---|---|
| 1 | Working style | rules applied before answering, five collaboration modes, task routing, time and confidence labels | 12 |
| 2 | Memory and knowledge | multi-layer memory, decision records, semantic search, retention rules | 27 |
| 3 | Written output | upward reporting, strategic proposals, requirements, acceptance review, translation, financial-sheet checks | 16 |
| 4 | Reading material | scanned documents, images, recordings, video, web pages, long documents | 13 |
| 5 | Presentation and media | slide generation and rework, layout analysis, image generation, style corpora | 10 |
| 6 | Delivery | multi-device consistency, large files, notifications, attachments, long-task behaviour | 22 |
| 7 | Autonomy | daily brief, overnight analysis, reminders, backups, queueing, cost reporting | 18 |
| 8 | Quality assurance | pre-delivery checks, cross-model review, post-hoc verification, watchdog coverage | 36 |
| 9 | Governance | rule ownership, change history, retirement criteria, terminology, dependency maps | 18 |
| 10 | Security and access | layered interception, credential handling, authentication, approval boundaries | 23 |
| 11 | Stability | rollback, state restoration, degradation paths, rebuild safety | 29 |
| 12 | Foundations | reusable procedures, script library, tool evaluation | 9 |
| 13 | Multi-user | per-account isolation, profile-scoped knowledge, shared-procedure review | 5 |

## Three examples, with the boundary attached

| Task | What it produces | Where it stops |
|---|---|---|
| Read a hundred-page tender or deck | structure, key figures, logic chain, risk list | fast mode and deep mode cost differently; the choice is the user's |
| Turn execution-level material into an upward report | strategic narrative with data support and risk anticipation | it restructures; it does not invent facts |
| Keep a project's history | decisions, premises, and the conditions under which they would be reversed | a human still confirms the record periodically |

## Known limitations (published, not discovered later)

1. Account isolation is at the application layer; someone with access to the underlying machine can bypass it.
2. Message delivery requires the recipient to have contacted the system first; long silences can block proactive pushes.
3. Some Android devices have no system-level push; a separate app is required.
4. Reminder records are append-only and uncapped; long use needs manual cleanup.
5. A long-running job's keep-alive proves the connection is up, not that the job is progressing.
6. Some interception rules read the command text only, not external configuration.
7. Semantic search depends on an external service; when it is unavailable the system falls back to keyword search.
8. Image understanding is external and slow (tens of seconds per image), but accurate; there is no local fallback.
9. Some scheduled jobs check only that credentials exist, not that the service is reachable.
10. A page killed or frozen by the OS loses intermediate streamed content; the saved part survives.
11. Backup deletion is protected; some cleanup still requires manual confirmation.
12. Generated content still needs human review; labels and cross-checks reduce risk, they do not replace judgement.
13. Single-file transfer is capped at 1 GB.
14. Written descriptions can lag reality; the ledger entry's date and verification command are the ground truth.

## How this document stays honest

Every capability entry carries an internal reference back to the ledger. A machine check verifies, on each update, that every ledger entry appears exactly once and that no entry is invented. The check fails the build; it is not advisory.

Two rules govern what may appear here: no implementation detail, and no personal data. The ledger keeps the process; this page keeps the result.
