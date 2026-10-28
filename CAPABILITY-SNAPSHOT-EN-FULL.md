# Capability Snapshot — full edition

> **Version**: 2026-10-28, v1 (English full edition)
> **Readers**: external parties and leadership. Sections I–III give enough to form a judgement; the tables are the per-capability record, for verification rather than reading end to end.
> **Convention**: this document states only *what it can do, how far it goes, and where it stops*. Implementation detail and internal process stay in a separate internal ledger.
> **Scope**: describes one single-machine deployment. Configuration, data and integration for a specific organisation are delivered separately and are not promised here.
> **Figures**: change with use; confirm against the latest on-site check before quoting them externally.
> **Maintenance**: updated irregularly — when a capability changes at the level of *have / don't have* or *can / can't*, and before any external submission.

## How to read

- **Leadership / external readers**: read Sections I–III only, about five minutes.
- **Looking up one capability**: use the scenario index in Section IV, or go straight to Chapters V–XVII.
- **Judging risk**: read the "Boundary" column first, then Appendix A. The boundary is the other half of the capability.
- **What not to do**: do not read the 238 rows cover to cover. It is a reference, not a briefing.

---

## I. What this system is

In one sentence: an **AI working system that reads material, produces finished documents, remembers context, and works on schedule without supervision**.

It is not a chat tool. Within the scope it is authorised for, it reads and writes files, organises material, produces documents, runs on a schedule, and delivers results to a designated channel. The person supplies judgement and sign-off; the system does the preparation on either side of that judgement.

It runs on one machine. Material, working notes and results stay local; only the understanding and generation steps use external AI services.

## II. What problem it solves

Knowledge work is a chain:

**find material → read it → judge → produce → deliver → file**

Six of those steps do not need a human, yet they take most of the time. This system takes those six and pushes the person's time back into the judgement in the middle.

The change is not "writing faster". It is four things:

1. Several readings of the same material can be laid out at once, instead of trusting a first impression;
2. Why a decision was made three months ago is still retrievable, so it does not get re-argued;
3. Routine checks, backups and summaries no longer depend on someone remembering them;
4. Material that went in can be found again — "I think we have it somewhere" stops being a dead end.

## III. What it can do (overview)

| Area | In one line | Detail |
|---|---|---|
| Understanding and collaboration | switches working style by situation; checks before answering, reviews before delivering | Chapter V |
| Experience and material | remembers people, projects and reasons; retrieves them | Chapter VI |
| Written output | reports, proposals, analysis, requirements, acceptance | Chapter VII |
| Reading material | documents, images, recordings, video, web pages | Chapter VIII |
| Presentation and media | slides, images, layout analysis, rework | Chapter IX |
| Delivery and access | multi-device consistency, large files, notifications, results delivery | Chapter X |
| Autonomy | scheduled work, monitoring, summaries, backups | Chapter XI |
| Quality assurance | pre-delivery checks, post-hoc verification, anomaly detection | Chapter XII |
| Rules and traceability | the rules are themselves supervised; conclusions are traceable | Chapter XIII |
| Security and access | who may see, who may change, what is logged | Chapter XIV |
| Stability | problems are found and absorbed before a person notices | Chapter XV |
| Foundations | reusable procedures and tools | Chapter XVI |
| Multiple users | one environment each, without interference | Chapter XVII |

## IV. Find a capability by scenario

| I want to… | Go to |
|---|---|
| write an upward report or a speech | 7.01, 7.03 |
| get through a stack of tenders, reports or decks quickly | 8.08 |
| turn a vague idea into a requirements document | 7.05 |
| review acceptance material or deliverables | 7.06 |
| get independent analyses of one document from several angles | 7.02 |
| turn analysis into slides, or rework an existing deck | 9.01, 9.06 |
| make paper documents, recordings or web pages searchable | 8.01, 8.05, 8.07, 6.07 |
| have project progress and past decisions remembered | 6.06, 6.08, 6.16 |
| receive a daily briefing automatically | 11.01, 11.11 |
| have the system notice problems before I do | 12.28, 12.33, 15.05 |
| get results onto a phone without transferring files by hand | 10.01, 10.12, 11.13 |
| let several people use it independently | 17.01, 17.02 |
| see where it is unreliable | Appendix A |
| check the basis for a given claim | Appendix C |

## Terminology

| Term used here | What it means |
|---|---|
| hard rule | refused by the system itself, not left to good intentions |
| scheduled work | starts at a set time; nobody has to remember it |
| standard procedure | a written sequence, identical every time for the same kind of work |
| search by meaning | retrieval by sense, not by exact wording |
| long-term experience | accumulated preferences, project background and decision reasons |
| fallback | what takes over when something breaks, so there is no gap |
| filed | written to a file, not merely said in a conversation |
| check | verified before delivery; not released if it fails |
| independent account | a separate set of material and records per user |
| read-only review | look but do not change; findings go to a person |
| anomaly alert | silence when everything is normal, a notice when it is not |

---

## V. Understanding and collaboration

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 5.01 | Working charter | a full set of working rules; the common ones always active, detail fetched when needed | rules keep growing; everyday response time does not grow with them | C01 |
| 5.02 | Five collaboration modes | switches by situation: fault-finding, retrospective, adviser, audience translation, plain execution | modes can be combined | C02 |
| 5.03 | Pre-answer check | every answer is checked against the rules first; a hit stops it and explains why | small latency and usage cost | C03 |
| 5.04 | Task classification | infers the kind of work from the request and applies the matching approach | inferred from wording; unusual phrasing may misclassify and fall back to the general path | C04 |
| 5.05 | Hard floors | eight independent floor checks that no party can route around | each runs independently; one failing does not disable the rest | C05 |
| 5.06 | Delivery self-check | before delivery: were the sources cited, was confidence marked, was time verified | checks the finished product, not the intention | C07 |
| 5.07 | Self-correction | on noticing an earlier mistake, stops and says so, then redoes it | relies on self-report, not automatic detection | C08 |
| 5.08 | Complex-task routing | decides whether the work spans several departments or stages; if so, frames the whole before starting | framework methods are fetched on demand, adding no standing overhead | C13 |
| 5.09 | Delegation disclosure | when handing work to a sub-agent, states what material that agent cannot see, to prevent invented answers | a convention, not an enforced block | C26 |
| 5.10 | Freshness labels | sources are labelled in four bands: evergeen / within a year / older than a year / unknown | anything older than a year must carry a "reference only" note | TC01 |
| 5.11 | Confidence labels | each judgement is labelled in four bands: supported / mixed evidence / unverified / conjecture | tied to delivery self-check; a missing label blocks delivery | TC02 |
| 5.12 | Source citation | every conclusion names the material it rests on; when sources conflict, the original wins | the final call still belongs to a person | TC03 |

## VI. Experience and material

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 6.01 | Tiered retention | frequently used material is at hand, history is fetched on demand, neither occupies daily space | achieved by tiering, not by forgetting | C06 |
| 6.02 | Link archiving | links received are filed and indexed automatically | unreadable ones are not stored, to keep the library clean | C09 |
| 6.03 | Quotation recovery | when someone quotes or paraphrases earlier material, the original is recovered before answering | in extreme cases only the gist can be given | C11 |
| 6.04 | Sub-agent output filing | work done by sub-agents is filed automatically | automatic; no manual transfer | C12 |
| 6.05 | User profile | long-term preferences, priorities and phrasing learned before work starts | profile and inference are labelled separately; inferences need verification | M01 |
| 6.06 | Long-term experience | project progress, decision reasons and preference changes, retained indefinitely | tiered retention; completed projects move to history | M02 |
| 6.07 | Search by meaning | searching "distributed storage selection" finds "sharding pitfalls" | small usage cost per query | M03 |
| 6.08 | Decision records | each major decision records why, on what premise, and what would reverse it | requires periodic human confirmation | M04 |
| 6.09 | Communication archive | communication records within the owner's authorisation can be filed and searched | own account only, with the owner's authorisation | M05 |
| 6.10 | Version retention | every version kept separately; an old version opens as a complete state | no overwriting, no rewriting of history | M06 |
| 6.11 | Recent context | the last week's projects, key decisions and blockers, summarised automatically | continuity across sessions | M07 |
| 6.12 | Validity periods | each item has a validity period; before expiry it asks whether to keep or file away | expiry means archival, never deletion | M08 |
| 6.13 | Long-task memory | after an interruption or a restart, still knows what is still running | three-layer reconciliation; results are recorded retrospectively | M09 |
| 6.14 | Periodic consolidation | weekly merge of duplicates, removal of stale material, a trimming proposal | proposes first, acts after | M10 |
| 6.15 | Time stamping | new entries are stamped with their creation time | repeated writes do not stack stamps | M11 |
| 6.16 | Unified lookup | deep research follows a fixed order: background → history → library, with sources labelled | all three are local, so no extra cost | M13 |
| 6.17 | Supersession | distinguishes conclusions that have been replaced | superseded conclusions remain searchable | M14 |
| 6.18 | Source composition | summaries mark what came from the user and what the system inferred | informative only; behaviour unchanged | M15 |
| 6.19 | Usage health | tracks whether the system actually consulted memory when it should have | household accounts are not alerted separately; folded into the daily brief | M16 |
| 6.20 | Material partitioning | analysis, audit and inbox are kept as separate zones, all searchable | migration copies, never touches originals | M17 |
| 6.21 | Capacity display | shows how much room remains | display only, no intervention | M18 |
| 6.22 | Associative memory | extracts observations from each exchange, builds a picture of people and matters, supports follow-up questions | stored locally, not uploaded | M20 |
| 6.23 | Tiered knowledge base | originals, summaries and an index in three tiers | requires separate setup | M21 |
| 6.24 | Compaction on new dialogue | re-summarises the material at the start of each new conversation | about one second | T46 |
| 6.25 | On-demand full recall | fetches the complete record when the summary is insufficient | no standing overhead | T47 |
| 6.26 | Usage cost visibility | metered by actual usage; every entry can be recomputed | unit price follows the provider | T119 |
| 6.27 | Record provenance | each record notes which capability version produced it | traceable across version changes | T121 |

## VII. Written output

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 7.01 | Upward reporting | two rounds, nine gates: predict the hardest questions before drafting, then add the parts that earn credit | needs the audience and occasion stated first | T10 |
| 7.02 | Multi-angle analysis | fifteen independent readings of one document, from different lenses | the angles are a framework; not every document needs all of them | T11 |
| 7.03 | Elevating a report | rewrites execution-level material as a strategic narrative: what was done → why it matters → what next | restructures only; never invents facts | T13 |
| 7.04 | Strategic proposals | five stages: audience → own constraints → their pressures → frame → adversarial review | builds strategy-level proposals, not execution plans | T14 |
| 7.05 | Requirements front-end | turns "we need a system for X" into a proposal-grade requirements document | the output is a proposal, not a technical design | T15 |
| 7.06 | Acceptance review | compares mixed-format acceptance material against requirements, item by item | criteria come from the contract and requirements, not from the reviewer | T16 |
| 7.07 | Talent management | eight-dimension diagnosis, monthly inventory, interview cadence reminders | involves judgements about people; advisory only, a person decides | T17 |
| 7.08 | Onboarding design | training path, exercises and assessment tailored to the team's constraints | one version per person, no template | T18 |
| 7.09 | Translation | three quality tiers, a glossary, and learning from corrections; terminology consistency first | speed yields to terminology accuracy | T19 |
| 7.10 | Financial spreadsheet review | checks colour conventions, hard-coded formulas, format consistency, documented assumptions | checks convention, not financial judgement | T20 |
| 7.11 | Collaborative writing | gather context → refine section by section → a blind reader reviews | helps structure; does not write it for you | T21 |
| 7.12 | Improvement loop | from an external input to a landed change, with a record at each step | confirmed item by item, never swallowed in bulk | T22 |
| 7.13 | Method extraction | external article → transferable method → comparison with our own situation → action items | extracts only; does not execute | T23 |
| 7.14 | Evidence before change | before deciding to fix something, first establishes statistically that the problem is real | no data, no conclusion | T24 |
| 7.15 | Pre-change reminder | detects whether this turn touches processes or rules, and appends a checklist | self-suppresses after repeated identical cases, to avoid nagging | T36 |
| 7.16 | Travel planning | audits an existing itinerary on four layers, or generates one; delivers an offline-openable page | transport and lodging details are marked as unverified | T134 |

## VIII. Reading material

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 8.01 | Paper digitisation | photographed or scanned contracts, documents and minutes → searchable text | handwriting and poor scans need human review | T04 |
| 8.02 | Image understanding | a dedicated multimodal capability reads images rather than a text model guessing | slow but accurate: tens of seconds per image | T04B |
| 8.03 | Parallel batches | several images processed at once | mixing image reading with image generation triggers rate limits; they are separated | T04C |
| 8.04 | Page-type routing | charts, tables of contents and body pages each get the reading method that suits them | page classification costs about a second and errors reduce quality | T04E |
| 8.05 | Speech to text | meetings and voice messages → searchable text; can answer "what three topics were discussed" | long recordings take time | T05 |
| 8.06 | Shared-conversation extraction | a shared conversation link → full text archived | requires the sender to share publicly | T06 |
| 8.07 | Article extraction | public articles → archived full text → permanently searchable | paid content is not taken | T07 |
| 8.08 | Long-document reading | a hundred-page document → structure, key figures, logic chain, risk list | fast and deep modes differ in cost | T12 |
| 8.09 | Automatic link capture | links sent in are fetched and filed, deduplicated | unreadable ones are not stored | T41 |
| 8.10 | Sign-in reuse | an existing browser session is reused instead of signing in again | sessions expire and need periodic refresh | T42 |
| 8.11 | Cloud transcription | recordings uploaded directly, with word-level timing | billed per hour | T43 |
| 8.12 | Session keep-alive | checks daily whether the sign-in still works and warns when it does not | credentials are stored encrypted and never displayed | T44 |
| 8.13 | Video analysis | a link → choose depth → automatic processing → staged progress → report | long videos take a long time | T45 |

## IX. Presentation and media

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 9.01 | Slide generation | conversation → page-by-page generation under a design system → an editable deck | a template must be established first | T31 |
| 9.02 | Text-based role-play environment | a self-hosted environment for story co-creation | experimental; not a production promise | T32 |
| 9.03 | Image generation | drives an already signed-in drawing tool to produce candidate images for selection | depends on that session | T33 |
| 9.04 | Layout analysis | infers a design system from reference material: surface, narrative, content | supports cross-comparison of several decks | T37 |
| 9.05 | Single-page reconstruction | produces a full specification for one page (layout, type sizes, colours) that can be rebuilt | billed per page | T38 |
| 9.06 | Deck rework | two tracks in parallel: read the original → extract text → merge → proposal → full rebuild | fixed pipeline, no branching | T39 |
| 9.07 | Catalogue building | organises works by author, deduplicates, generates an index and statistics | resumable after interruption | T122 |
| 9.08 | Style analysis | a nine-dimension framework plus corpus statistics plus a style card | machine statistics with human reading | T123 |
| 9.09 | Personal writing baseline | extracts the owner's own writing characteristics as a baseline | the corpus stays local | T124 |
| 9.10 | Web publication | a set of pages published as a permanent link, independent of this machine being on | adds a no-index marker before publishing | T133 |

## X. Delivery and access

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 10.01 | Multi-device consistency | computer, phone and desktop reach the same assistant and the same experience | not several independent bots | T08 |
| 10.02 | Pre-delivery verification | checks that a file exists and is sendable before sending | a missing file is refused, never silently dropped | T34 |
| 10.03 | Missed-attachment repair | if the attachment tag was forgotten, it is added and the file sent | adds the file only; never alters the text | T40 |
| 10.04 | Large-file transfer | chunked transfer with resumption; single file up to 1 GB | existence is checked; completeness is confirmed at the end | T148 |
| 10.05 | Two-entry web app | one page set serving two entries, installable to a phone home screen | after an update the home-screen icon must be re-added | T149 |
| 10.06 | Dual-channel notification | completion notices take a different channel per device type | some Android devices lack system-level push and need a separate app | T150 |
| 10.07 | History search | the full message history indexed and searchable across sessions | after a provider change, usage counters may read zero | T151 |
| 10.08 | Three search modes | keyword, by meaning, or both | search by meaning carries a small usage cost | T152 |
| 10.09 | Attachment viewer | images, video and documents in one viewer, with a fallback link | an attachment may occupy two copies; they are released together | T153 |
| 10.10 | Behaviour switches | users may turn several behaviours on or off; locked items stay locked | a new account without explicit settings inherits defaults | T154 |
| 10.11 | Phone reminders | near-real-time reminder delivery, no need to keep the app open | the reminder store is append-only and needs periodic human cleanup | T155 |
| 10.12 | Timestamps | messages show time to the second; history and live share one convention | the same message may differ by seconds across a refresh | T160 |
| 10.13 | Attachment subdirectories | downloads support nested paths, validated segment by segment | listing and upload still handle the top level only | T161 |
| 10.14 | Waiting experience | keeps the connection during long work, gives a neutral notice, resynchronises on return | proves the connection is alive, not that work is progressing | T162 |
| 10.15 | Brand consistency | application name, icons and version managed centrally | an old home-screen icon does not update itself | T163 |
| 10.16 | Two-entry header | one page set serving two entries through a shared template rather than replacements | the fallback only guarantees the page opens | T164 |
| 10.17 | Resume on return | returning from the background resyncs automatically instead of redrawing stale state | after the page is fully closed it loads fresh | T165 |
| 10.18 | Internal metadata hidden | system-internal markers no longer appear as the user's own words | display only; stored records are untouched | T168 |
| 10.19 | Internal notices separated | background completions and system notices no longer appear as chat turns | different surfaces handle them differently, by design | T169 |
| 10.20 | Long-conversation anchoring | reopening a long conversation starts at the right place instead of being overwritten by older pages | a display-order issue; no record was ever lost | T170 |
| 10.21 | Long tasks survive disconnect | leaving the page does not cancel the run | an explicit stop still stops; new messages queue meanwhile | T171 |
| 10.22 | Visible activity | with reasoning hidden, the interface still shows "working" and which tool is running | supported on some clients only | T175 |

## XI. Autonomy

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 11.01 | Daily brief | yesterday's summary, backup status, job health, account balance and open items, delivered in one push | nothing is filtered; judging importance is the reader's job | A01 |
| 11.02 | Overnight analysis | long analysis and blind-spot review while the person sleeps, conclusions ready in the morning | needs a clear question from the night before, or the output is generic | A02 |
| 11.03 | Scheduled reminders | five fixed categories: work, family, anniversaries, health, errands | public holidays skipped by calendar; make-up workdays run | A03 |
| 11.04 | Multiple backups | four independent backup chains, each a fallback for the others, fully automatic | alerts only on failure; deleting a backup needs explicit confirmation | A04 |
| 11.05 | Automatic filing of new material | new material organised and made searchable as it arrives | triggered on arrival, not by a nightly full scan | A05 |
| 11.06 | Daily profile refresh | extracts new facts from yesterday's exchanges and updates the user picture | each account updates independently | A06 |
| 11.07 | Version monitoring | daily check of key dependencies for new releases, with a notice when one appears | fully automatic; consumes no model usage | A07 |
| 11.08 | Balance monitoring | notifies when an account balance falls below a threshold | avoids discovering the problem at the moment of use | A08 |
| 11.09 | Network channel management | periodic checks, connects on demand, disconnects when done | only connects when needed; not persistent | A09 |
| 11.10 | Task queue | "queue this: …" enters a queue that is not forgotten | queuing and filing are one action | A10 |
| 11.11 | Daily triage | scans the material, ranks it, proposes three things to handle today | a proposal, not an instruction | A11 |
| 11.12 | Promise to reminder | a time promise in conversation ("remind me Wednesday") becomes a reminder | asks once when the time is ambiguous | A12 |
| 11.13 | One-step delivery | delivers to a designated channel; no email or USB round trip | single file up to 1 GB; rate limited | A13 |
| 11.14 | Change self-healing | risky changes are made with a prepared way back, cancelled once verified | covers predictable changes only; incidents belong to Chapter XV | A14 |
| 11.15 | Automatic activation | after a change, activation is scheduled rather than left to a person | activation interrupts turns in progress | A15 |
| 11.16 | Long-task progress | start and finish of each asynchronous task recorded in pairs | early versions recorded starts only; fixed | A16 |
| 11.17 | Cost report | daily cost by provider and by purpose | some providers are estimated from balance differences, not billed data | A17 |
| 11.18 | Unattended operation | with authorisation, works through a list on its own, taking only reversible actions | items needing a decision are listed, not decided; never touches floors or permissions | S22 |

## XII. Quality assurance

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 12.01 | Review guide | every deliverable opens with: what changed, where the point is, what may be skipped, what is assumed, what next | missing items are filled in automatically; delivery is never blocked | Q01 |
| 12.02 | Summary block | files over five hundred words get a one-line conclusion and a recommended action | complements the review guide: one decides whether to read, the other how | Q02 |
| 12.03 | Cross-model review | one side drafts, another reviews independently for factual errors, logical jumps and self-contradiction | the same side cannot see its own error | Q03 |
| 12.04 | Four-gate check | convention → fact → logic → consistency, all passed before "done" may be claimed | failure means rework, not a partial pass | Q04 |
| 12.05 | Source labelling | every document states which material it used, from when, and what it relates to | provenance is traceable | Q05 |
| 12.06 | Pre-write check | naming, characters, compliance markers and sensitive formats checked before writing | the original is always retained; writing is never blocked | Q06 |
| 12.07 | Process supervision | each turn's output checked against the rules, in three escalating tiers from cheap to expensive | escalates only when the first tier objects | Q07 |
| 12.08 | Search trail | every lookup archived with its query and result | no extra cost | Q08 |
| 12.09 | Delivery check | structured validation before a file goes out; a missing marker is added | guarantees it is sent, not that it is right | Q09 |
| 12.10 | Narrative output | important deliverables add three parts: a thirty-second story, a one-sentence analogy, a thirty-second retelling | only for important deliverables; short replies skip it | Q10 |
| 12.11 | Confidence on the surface | long outputs must end with a confidence label | improves visibility; truthfulness is backed by review | Q11 |
| 12.12 | Historic-source labelling | historical data cited must name its source | the same principle as "a number needs a command behind it" | Q12 |
| 12.13 | Change review | after a change, a multi-angle review runs, with a dedicated "symptom vs root cause" column | in one run nine findings, four held; humans verify | Q13 |
| 12.14 | Independent review | a reviewer in an isolated context receives the artefact and the requirement, not the author's defence | its findings are reproduced before being accepted | Q14 |
| 12.15 | Alert noise reduction | status-type alerts that naturally expire are demoted; only substantive ones remain | new phrasings may be missed; failure direction is safe | Q21 |
| 12.16 | Cleanup discipline | a cleanup pass only drives the count to zero; it does not open new branches | new findings go to the next round's list | Q22 |
| 12.17 | Output verification | after a scheduled job, checks that the result exists, is non-empty and is well-formed | targets "said it did, did not" | V01 |
| 12.18 | Goal closure | was the stated outcome actually produced? three-hourly watchdog plus a daily item-by-item check | semantic grading fails more often than mechanical checks | V02 |
| 12.19 | Library inspection | inspects material quality proactively rather than waiting for an error | three fixed checks | V03 |
| 12.20 | Two-way sync | external material pulled in, results pushed out | does not vouch for content correctness | V04 |
| 12.21 | Job self-check | checks its own scheduled jobs, so a job that stopped long ago is noticed | four checks | V05 |
| 12.22 | Foundation check | checks that the conditions the output depends on are healthy | two checks | V06 |
| 12.23 | Cross-reference patrol | weekly scan for links to material that no longer exists | silent unless something is broken | V07 |
| 12.24 | Memory upkeep | summary generation, injection verification and format protection, automatically | maintains form, not content judgement | V08 |
| 12.25 | New-file prompt | notices a new file and asks whether to file it | requires a human yes | V09 |
| 12.26 | External change watch | a one-off watch on a page that may change | set up on demand; no general subscription service | V10 |
| 12.27 | Routine upkeep | daily archiving, permission repair, expiry cleanup | deterministic maintenance only; never touches business content | V11 |
| 12.28 | Continuous monitoring | eight independent watchdogs; silent when healthy, a notice when not | each independent; one failing does not blind the rest | V12 |
| 12.29 | Capability inventory check | scans for enabled capabilities missing their registration — which means they never load | targets "built but never active" | V13 |
| 12.30 | Verification archiving | the verification used for a change is archived with its subject, assertions and how to run it | must be re-run in full on the day it is archived | V14 |
| 12.31 | Consistency self-check | samples historical passages daily and re-searches them, detecting drift between index and material | silent when healthy; a small usage cost per run | V16 |
| 12.32 | Memory-dependency probe | measures whether memory was consulted when the situation called for it, replacing a call-count metric that had gone hollow | trigger-word based; false-trigger rate kept under 5% | V17 |
| 12.33 | Backup health | eight read-only checks: freshness, the repository itself, missed cycles, key files present | read-only; remedies live in Chapter XV | V18 |
| 12.34 | Unique-registration assertion | asserts that only one registrant exists for hooks where the first one wins | more than one enabled registrant raises an error | V19 |
| 12.35 | Silence contract | scheduled jobs say nothing when nothing changed and fail only when they fail | a few jobs carry real content and cannot be silenced wholesale | V20 |
| 12.36 | Repeat-issue marking | when filing an alert, compares it against history to detect the same problem recurring | topical similarity is not the same problem | V21 |

## XIII. Rules and traceability

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 13.01 | Pre-launch check | before a new procedure goes live, checks that its external conditions exist | pure checking; no model usage | T35 |
| 13.02 | Same-topic deduplication | scans all procedures for two builds of the same thing; warns only for ones created within a day | historical duplicates are listed for a human to merge | T126 |
| 13.03 | Checker self-correction | the checkers themselves misreport; those patterns are catalogued and handled | static judgement; dynamic conditions still need a real run | S15 |
| 13.04 | Baseline refresh | compares against a baseline periodically and provides an explicit refresh entry point | refreshing is itself a human confirmation | S16 |
| 13.05 | Automatic-output marking | anything produced automatically is prefixed as unconfirmed | the criterion shares one source with the output check | S17 |
| 13.06 | Completion tasks to scripts | work once done by a model converted to a fixed procedure, run daily | depends on a dedicated runtime | S18 |
| 13.07 | Duplicate-block check | scans key ledgers for large byte-level repeats | checks repetition, not correctness | S19 |
| 13.08 | Verification provenance | every verification declares its origin: real failure / contract / coverage gap / drift guard | a missing declaration is an error | S20 |
| 13.09 | Judgement benchmark | real cases frozen into a repeatable benchmark with deterministic scoring | when strong and weak models score alike it is a floor, not a discriminator | S21 |
| 13.10 | Procedure history | answers "how did this procedure become what it is" | deduplication by exact match plus a short window | S23 |
| 13.11 | Source completeness | checks three distortions: skipped numbering, broken citations, missing numerator/denominator/as-of date | reports only mechanically confirmable gaps | S24 |
| 13.12 | Retirement criteria | executable criteria for how capabilities, knowledge and mechanisms should exit | exit usually means archival, not deletion | S25 |
| 13.13 | Background curator registration | the framework's own background thread creates and edits procedures; this entry records it and its limits | it does not return to the main context, so check it first when procedures appear from nowhere | S26 |
| 13.14 | Glossary | one definition per key term, an authoritative anchor, and what not to use it for | thirteen entries, with a completeness check | Q15 |
| 13.15 | Capability-knowledge map | before changing a knowledge source, shows which capabilities depend on it | covers active capabilities only | Q16 |
| 13.16 | Acceptance dimensions | each acceptance standard paired with a named mechanism and one executable check | needs a named mechanism first, or the table is empty | Q17 |
| 13.17 | Versioned history | key content kept by version, answering "can we return to a past point" | whitelisted content only | Q18 |
| 13.18 | Procedure slimming | the main file keeps criteria and pointers; examples move to attachments | attachments are not machine-checked; pointers are reviewed by hand | T166 |

## XIV. Security and access

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 14.01 | Layer-level interception | a dozen independent checks intercept at the system layer, not by good intentions | each independent; a missing registration means it silently does not load, with 12.29 as the net | S01 |
| 14.02 | Two-layer defence | the first layer matches known attack patterns; the second reviews content for suspicion | the second layer adds latency; external content always passes through both | S02 |
| 14.03 | Encrypted credentials | all keys stored encrypted in one place, never in plain text anywhere | a format match on write blocks it | S03 |
| 14.04 | Monthly security baseline | five dimensions checked monthly: hard-coding, residue, permissions, plain text, keys | alerts only on failure | S04 |
| 14.05 | Daily compliance scan | daily scan of outputs: path leakage, contaminated material, naming violations, inconsistent settings | silent on pass, alert on violation | S05 |
| 14.06 | Approval boundary | high-risk actions wait for a human click, graded by risk | confirmation appears on this device only | S06 |
| 14.07 | Garbled-text detection | detects replacement characters (encoding boundary errors) on write | does not know the original character; reports, never auto-fixes | S07 |
| 14.08 | Conclusion fact-check | extracts claims after each turn and compares them with existing records | about ¥25 a month; compares against internal records only | S08 |
| 14.09 | Enforcer registry | every gate, hook and verification script registered in one place, liveness checked daily | registration is not proof of effect; the check is | S09 |
| 14.10 | Hook practice rules | three rules from experience, preventing silent failure | rules, not mechanisms; review is the fallback | S10 |
| 14.11 | Pre-publication sweep | four steps: layered wordlists, dual checking, history handling, real-case removal | deleting a file does not clear history | S11 |
| 14.12 | Rule-write logging | every channel that modifies standing rules leaves one record | logging only; a human reads the weekly summary | S12 |
| 14.13 | Failed delivery is not lost | transient delivery failures enter a retry queue with deduplication | genuine errors are still reported | S13 |
| 14.14 | Directory-level protection | backup and rollback cover whole directories; a deleted target counts as "already changed" | does not catch wildcard or unexpanded-variable forms | S14 |
| 14.15 | Narrowed privileges | system privileges narrowed from wildcards to specific actions | installation flows therefore ask for confirmation, which is the point | S29 |
| 14.16 | Entry authentication | login credentials, two-step verification, rate limiting, action logging, credential inventory | account isolation is application-level, not a security boundary | S30 |
| 14.17 | Origin determination | distinguishes direct local access from requests arriving through a forwarder | a change of access path requires re-checking | S31 |
| 14.18 | Two-step verification hardening | single-use codes, error counting, correct code wins, against lockout and probing | depends on the message channel delivering | S32 |
| 14.19 | Per-account code channel | each account uses the channel bound to it; a missing setting fails explicitly | channel selection is heuristic; a human confirms | S33 |
| 14.20 | Write-scope narrowing | blocks only actions with write intent; reading passes | when intent is unclear it blocks; protected paths mentioned in prose also trip it | T125 |
| 14.21 | Exemption watchdog | applies a check to the act of exempting checks itself | any output fails it; a reverse test proves it is not decorative | R27 |
| 14.22 | Declaration consistency | the declaration and the actual contents must agree in both directions | consistency only, not quality | R28 |
| 14.23 | Public entry point | internal services exposed to a defined audience over an encrypted channel | the channel is a single point; no independent external monitoring | R30 |

## XV. Stability

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 15.01 | Change rollback | backup first, a ten-minute rollback prepared, cancelled once verified | see 11.14 | R01 |
| 15.02 | Change ledger | customisation survives each upgrade: change + verification + assertion + rollback | the ledger must track the change, or the audit is false | R02 |
| 15.03 | Three-layer protection | rollback, automatic restart, and refusing to give up, complementary | each layer covers a different segment | R03 |
| 15.04 | Resource monitor | samples resource use hourly and restarts above a threshold | the restart interrupts work in progress | R04 |
| 15.05 | Storage health | collects storage health data and warns ahead of failure | warns only; does not replace hardware | R05 |
| 15.06 | External storage tolerance | retries and degrades to local when external storage is unstable | does not guarantee remote consistency | R06 |
| 15.07 | Permission repair | finds and fixes files with abnormal permissions | handles known shapes only | R07 |
| 15.08 | Version detection | daily check for a newer release with an assessment | detects only; does not upgrade | R08 |
| 15.09 | Alert threshold calibration | an early conservative threshold produced zero findings; replaced with "any signal is reported" | false positives are judged cheaper than misses | R09 |
| 15.10 | Blocking message correction | when blocked, states the correct action instead of a misleading hint | applies only in that turn | R10 |
| 15.11 | Per-account restart | the second account has its own recovery mechanism | requires separate configuration | R11 |
| 15.12 | Delivery diagnostics | delivery is logged throughout; failures are stated in the reply | paths are masked in the log | R12 |
| 15.13 | Isolated runtime | a complete isolated runtime, detached from external dependencies, fetching locally | some resources still need an external channel | R13 |
| 15.15 | Experience cleanup | daily judgement on expired, completed and duplicate entries, reversible | twenty entries per batch | R15 |
| 15.16 | Self-recovery | delayed retry when a read fails, breaking crash-restart loops | unrelated to network faults | R16 |
| 15.17 | Quotation retention | three-tier fallback keeps quoted text | last resort is a placeholder | R17 |
| 15.18 | Upstream watchdog handover | crash and hang detection handed to the upstream mechanism | upstream is sensitive to heavy load; tolerance needs tuning | R18 |
| 15.19 | Known-good restoration | snapshots after fifteen stable minutes; classified restore, three kept | restores tracked files only, not data | R19 |
| 15.20 | Capability fallback | switches to a fallback in order; a new conversation returns to the primary | re-read each turn; no restart needed; not written back to the session | R20 |
| 15.22 | Non-disruptive rebuild | the old index stays online during a rebuild | on failure the old index is byte-identical | R22 |
| 15.23 | Retry backoff | up to three retries with increasing intervals | failure is surfaced; the old index is intact | R23 |
| 15.24 | Resumable rebuild | a checkpoint every two thousand chunks; a mismatched fingerprint restarts | the fingerprint covers count and version | R24 |
| 15.25 | Reclaim with evidence | copy the old index before rebuilding; damaged files renamed and archived | old snapshots are not deleted automatically | R25 |
| 15.26 | Empty-record guard | degrades gracefully when a record is damaged or empty | fixes the crash, not the content | R26 |
| 15.27 | Stall detection | watches long runs for stalls and releases the hold | does not handle runs stuck inside a long command | R31 |
| 15.28 | Rate-limit cooldown | on rate limiting, waits instead of pushing | at most two rounds; then it fails | M12 |
| 15.29 | Filename normalisation | filenames handled character by character, so Chinese names are not cut | covers illegal names only; other failures are reported as before | T167 |
| 15.30 | Single settings entry | all settings changes go through one writer that preserves comments, with a fallback and a weekly check | the fallback can only detect and recover quickly | M19 |
| 15.31 | Dependency conflict resolution | resolves a version conflict at packaging time, so installation is compliant | an upstream change requires redoing it | T172 |

## XVI. Foundations

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 16.01 | Standard procedure library | each procedure = trigger + steps + known pitfalls + verification | 320+ registered; count is not quality, look up on demand | T01 |
| 16.02 | Meta-methods | eight methods about how to work: procedure design, proposal stress-testing, strategy design, improvement loop | does not handle tasks directly; governs the quality of procedures | T02 |
| 16.03 | Capability allocation | each task uses the capability that suits it: reasoning, vision, speech, structured material | fixed convention; changes need separate authorisation | T03 |
| 16.04 | Fixed procedure library | deterministic work runs as a fixed procedure: no model usage, no invention, identical result each time | 370+ registered; still checked before going live | T09 |
| 16.05 | Tool evaluation | a new tool compared against the existing set, classified as replacement / complement / addition / unnecessary | classification is a human call | T25 |
| 16.06 | Web automation testing | opens pages, operates them, screenshots, checks the page's own feedback | covers only paths already scripted | T26 |
| 16.07 | Session migration | reuses an existing sign-in instead of signing in repeatedly | sessions expire | T27 |
| 16.08 | Integration method | four stages: research → implement → review → evaluate | the standard path for adopting a new tool | T28 |
| 16.09 | Voice cloning | synthesises from a short reference recording | experimental; not promised for production | T29 |

## XVII. Multiple users

| No. | Capability | What it does | Boundary | Ref |
|---|---|---|---|---|
| 17.01 | Account isolation | two independent environments, each with its own rules, experience, schedules and material | share one machine | P01 |
| 17.02 | Material isolation | two libraries that never search into each other | share one external service | P02 |
| 17.03 | Profile synchronisation | one side is authoritative; the other syncs periodically; conflicts go to a person | syncs the profile only, not all content | P03 |
| 17.04 | Procedure sync across accounts | compare before copying: grade the differences → overwrite or patch → two-person review | never blind-overwrites, so local customisation survives | P04 |
| 17.05 | Procedure review | personal finding → peer review → owner approval → shared library | needs several people; a single-user case degrades to self-review | P05 |

---

## Appendix A: Known limitations (published, not discovered later)

| # | Limitation | Effect |
|---|---|---|
| A1 | Account isolation is at the application layer, not a security boundary | someone with access to the underlying machine can bypass it |
| A2 | The message channel requires the recipient to have made contact first | a proactive push after a long silence may fail; a fallback channel exists |
| A3 | Some Android devices lack system-level push | a separate app is required; a changed subscription must be set up again |
| A4 | Reminder records are append-only and uncapped | long use needs manual cleanup |
| A5 | Keep-alive during long work proves the connection is up | it does not prove progress; stalls need separate detection |
| A6 | Some interception reads command text only | it does not read external configuration; compound commands may slip through |
| A7 | Search by meaning depends on an external service | when unavailable it degrades to keyword search |
| A8 | Image understanding depends on an external service | slow (tens of seconds per image) but accurate; no local fallback |
| A9 | Some scheduled jobs check only that credentials exist | they do not probe whether the service is reachable, so an outage means a long wait |
| A10 | A page closed or suspended by the operating system | intermediate content during that period is lost; the saved part survives |
| A11 | Backup deletion is protected | automation is limited; some cleanup needs human confirmation |
| A12 | Generated content still needs human review | labels and cross-checks reduce risk; they do not replace judgement |
| A13 | Single-file transfer is capped at 1 GB | larger files must be split or sent another way |
| A14 | Written descriptions can lag reality | the latest on-site check prevails; nothing here is an absolute promise |

## Appendix B: Non-capability entries (records / retired / historical)

Listed so that coverage can be verified; they are not current capabilities:

| No. | Entry | Nature | Ref |
|---|---|---|---|
| B1 | A one-off migration and adjustment record | one-off, not a capability | T04D |
| B2 | A two-week observation of a memory upgrade | experiment; conclusions folded into Chapter VI | M22 |
| B3 | A concurrent-writer gate design | not pursued; never shipped | T120 |
| B4 | Duplicate rule-file injection | defect record, not a feature | R21 |
| B5 | A three-tier search design | historical snapshot; primary replaced | R14 |

## Appendix C: Coverage and verification

| Item | Value |
|---|---|
| Entries in the internal ledger | 243 |
| Covered here | 238 (seventeen capability areas) + 5 (Appendix B) = 243 |
| Not covered | 0 |
| Verification | each update is compared entry by entry against the ledger by an internal checker; a missing or duplicated entry fails the run |
| Traceability | follow the "Ref" column back into the ledger, where each entry carries its last verification date and method |

**Maintenance rules**

1. When the ledger gains an entry, this document gains a row; otherwise the check fails.
2. Prohibited here: implementation detail, internal process, change history, file paths, device addresses, real names, personal accounts, cost bookkeeping.
3. One row, one sentence per cell. If it does not fit, the capability itself is not yet clear.
4. Gaps in numbering are expected (Chapter XV omits 15.14 and 15.21, moved to Appendix B); a new capability takes the highest number in its area plus one.

| Version | Date | Change |
|---|---|---|
| v1 | 2026-10-28 | First full English edition, 243/243 coverage, seventeen areas |

---

**Prepared by**: the operator of this deployment · **Review**: pending · **Classification**: internal until the recipient scope is confirmed.

**How to cite**: capability statements here trace back to specific entries in an internal ledger. No personal identifiers, device addresses or internal paths appear in this document.

**Reading time**: five minutes for the summary; about thirty for the full tables.


