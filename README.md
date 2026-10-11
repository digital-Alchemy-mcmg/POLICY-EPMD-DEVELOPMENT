# POLICY/EPMD Reconciliation System — Master Implementation Plan
Status: IMPLEMENTATION BASELINE / Operator acceptance required at gates
Date: 2026-10-11
Repository: digital-Alchemy-mcmg/POLICY-EPMD-DEVELOPMENT

## Objective
Build a continuous, human-governed Prime Order reconciliation pipeline. Preserve deterministic authority, source provenance, sequential domain advancement, bounded questioning, and verified handoffs. This is a plan, not proof of an operating automation.

## Authority and separation
- Operator: sole acceptance, rejection, or alternative-decision authority.
- Muse: workload continuity, exclusive UUID minting at intake, contextual questioning, email dispatch, and receipts. Does not independently resolve or seek collisions.
- GPT: scheduled email pickup into review bay; interactive reasoning and proposed resolutions; sends only Operator-approved output onward.
- Reconciliation Spark: administrative routing, approved-payload pickup, two carbon copies, Canon Collector ingestion, collision-report evaluation, branch/replenishment.
- Ontology Spark: structural graph extraction, provenance, integrity; no semantic adjudication.
- Canon Collector NotebookLM: semantic collision reporting, not collision resolution. Attempt UUID terminates here.
- Sequence-and-Corpus NotebookLM: prepares next domain according to accepted PO sequence and specialized corpus; separate from Canon Collector.
- GitHub: versioned master specification and accepted records. Drive/Local System Gateway: working surfaces, not competing canon.

## Phase 1 — Pre-pipeline work
P1-01 Spark: inventory all POLICY NotebookLM notebooks via authorized browser access. Produce searchable taxonomy: exact title, URL, topic, specialized function, PO/domain coverage, evidence, access status, overlaps/gaps. Preserve specialized notebooks; never invent coverage.
P1-02 Gemini: inventory historical Google Drive POLICY corpus. Produce source manifest with title, path, identity, date/version, topic, authority status (accepted / historical / disputed / unknown), and provenance. No automatic canon promotion.
P1-03 Sequence owner: freeze the prescribed PO/domain order and prepare three initial Muse domain workloads plus three GPT email workloads (preload). Do not treat historical contradictions as ordering authority.
P1-04 Access owner: create isolated Canon Collector in clean account, share Editor to Spark account; test whether Spark's Add Source workflow can actually select and write to shared notebook. Block if test fails.
P1-05 Instruction owner: prepare per-system pre-context priming and system instructions; Muse POLICY vocabulary, scope, authority, historical drift, source routing.
P1-06 NotebookLM owner: define fixed artifact types and artifact-generation prompts; Reflector Plate collision source instructions; source-grounded collision report format.
P1-07 Data architect: define graph primitives (subject, predicate, object, node, edge, relation type, source, validity, confidence/authority status), data table matrices, immutable ledger headers, analytics-ready frames for resources, finance, population, metrics, formulas and future game values. Never invent values.
P1-08 Governance owner: draft historical-drift ignore list: currency, promos, elections, Mayor Mode, alternative endings and other early drift. Preserve history, exclude from active canon/questions/ontology unless Operator authorizes; classify ambiguous matches for review.
P1-09 Muse owner: design minimum/maximum question coverage: decision authority, conceptual management, subject/game-mechanic relations, cause/effect, dependencies, state transitions, constraints, consequences. Define sufficiency and stop rules, no endless interview or can-kicking.
P1-10 Architect: produce workflow diagram, ERD, queue-state model, UUID lifecycle, branch decision diagram, folder permissions, and audit flow.
Gate 1: inventory, taxonomy, schemas, priming, PO order, access test, question coverage, and diagrams reviewed; blockers named.

## Phase 2 — Pipeline construction
P2-01 Gateway owner: create one Local System Gateway root 'Muse/' with 'Muse Intake/', 'Reconciliation Spark Intake/', and 'Ontology Intake/'. Define owner/write/read boundaries. Working folders may be backed by Drive; verify actual access paths.
P2-02 Muse owner: scheduled pickup from Muse Intake; UUID + date/time + PO + domain + section front matter; batch questions, email subject restricted to those five fields; receipt and retry/dedup; no collision handling until collision payload arrives in its own intake.
P2-03 GPT runner owner: two-hour scheduled email poller, maximum five email workloads in GPT queue, UUID dedup, review landing bay. Runner retrieves only; does not reason/approve unattended. Verify permissions and runtime.
P2-04 Approval GUI owner: question, ambiguity/statement, GPT proposal, Operator approve / deny / alternative, explicit decision record. GUI used only for approvals; no silent acceptance.
P2-05 Reconciliation Spark owner: retrieve approved packet; split identical UUID-bearing copies to ontology and Canon Collector; collect Canon collision report; collision true -> aggregate all collisions into one new Muse intake workload; collision false -> request next domain from Sequence-and-Corpus notebook and send to Muse intake. Each new Muse intake mints new UUID. Track parent/cause links.
P2-06 Ontology Spark owner: receive carbon copy, extract structural relations only, write graph and provenance ledger, validate node/edge schemas.
P2-07 Ledger owner: intake/handoff, canon cycles/collisions, ontology graph/provenance. Fixed headers, immutable receipts, no full source prose in spreadsheet.
P2-08 Workload owner: preload GPT with 3 email workloads and Muse with 3 sequential domain workloads; Muse cannot see GPT queue; baseline two-hour polling. Separate supply from pickup frequency. Do not claim guaranteed uninterrupted work.
P2-09 Integrator: wire prompts, Reflector Plate, exclusion controls, notebook source selection, graph schemas, and approvals; test end-to-end with disposable sources.
Gate 2: verified receipts for every handoff, actual cross-account notebook write, UUID transitions, collision true/false branches, five-email cap, Operator gate, and recovery from failures.

## Phase 3 — Post-pipeline protocol
P3-01 Continuous cycle: Muse develops depth with time to inspect specialized notebooks and prepares questions; GPT reasoning only on Operator invocation; approved payloads return to Reconciliation Spark.
P3-02 Collision handling: Canon detects, Spark routes; Muse treats returned collisions as newly delivered workload. No silent semantic resolutions.
P3-03 Audit cycle: both Sparks run defined workflows; reconcile ontology structure, accepted POLICY statements, and versioned GitHub records; issue discrepancy report and decision requests.
P3-04 Checkpoint: audit semantic Canon and structural Ontology, require Operator acceptance, archive artifacts (mind maps, decks, accepted specs, collision/reconciliation, decisions, dependencies, graph/integrity/provenance); copy and rename frozen NotebookLM notebooks; keep working originals.
P3-05 Cleanup: only after accepted checkpoint and archive receipts, clean processed email/work queues while preserving evidence.
P3-06 Cadence control: default two-hour pickup; operator may add next sequence or change to hourly runners. Faster supply/polling must not reduce Muse's question-development time; track collision rate and quality before tuning.
Gate 3: replayable, inspectable cycle, accepted checkpoint, preserved artifacts, tested recovery.

## Parallel work packages — copy/paste prompts
### A — Spark NotebookLM taxonomy
Inspect accessible POLICY NotebookLM notebooks using authorized browser access. Produce an evidence-based searchable taxonomy (title, direct URL, topic, PO/domain, specialized functions, source status, overlaps, gaps, inspection receipt). Keep specialized notebooks intact. Report inaccessible items and uncertainty. No changes to canon.

### B — Gemini Drive corpus
Inventory POLICY Drive corpus without moving files. Build manifest with exact paths, identifiers, versions, source chronology, subjects, and accepted/historical/disputed/unknown status. Flag deprecated early drift. Never infer acceptance from recency. Return CSV-ready headers and evidence links.

### C — Data contracts and approval GUI
Specify YAML front matter, UUID lifecycle, queue states, immutable ledgers, collision report schema, ontology subject-predicate-object/node-edge graph model, analytics-ready tables, and Operator-only approval GUI. Deliver schemas, field dictionary, sample records clearly labeled synthetic, validation rules, and edge cases. No invented POLICY values.

### D — Workflow/ERD architecture
Create diagrams for Muse -> email -> GPT approval -> Reconciliation Spark -> Canon Collector + Ontology Spark -> collision true/false -> Muse; include separate Sequence-and-Corpus notebook, two-hour pollers, 3+3 preload, max-five GPT email queue, folder permissions, and UUID termination/new minting. Supply editable diagram source, ERD, handoff contracts, and failure/retry states. Do not introduce new decision authority.

### E — Muse priming and coverage
Prepare Muse POLICY priming, notebook taxonomy navigation, historical ignore-list enforcement, bounded min/max coverage matrix, and email/question templates. Required lenses: decision-making, conceptual management, game-mechanic relationships, cause/effect, dependencies, state changes, constraints, consequences. Muse keeps work moving, not collision adjudication. Provide test scenarios.

### F — NotebookLM prompts and audit
Prepare artifact prompts, Reflector Plate collision-detection instructions, Canon Collector output schema, Sequence-and-Corpus next-domain instructions, and dual-Spark checkpoint audit workflow. Ensure citations and provenance, distinct notebooks, no notebook-generated UUID, and no automatic collision resolution.

### G — Gateway and integration
Prepare root folder and access matrix, verify connectors/browser access, wire handoff receipts, test cross-account NotebookLM writes, build disposable end-to-end harness with both collision outcomes and Operator decision stop. Mark BLOCKED when action unavailable; never report configured as executed.

### H — Claude independent inspection
Audit each work package against this master plan. Produce PASS / FAIL / BLOCKED per acceptance criterion, exact evidence, authority-boundary violations, missing prerequisites, schema conflicts, contradictions, and minimal corrective assignments. No silent edits or expansion of scope. Recheck after repairs; do not certify untested runtime behavior.

## Integration order
Parallel first: A, B, C, D, E, F and access reconnaissance for G. Then reconcile names/headers/authority contracts. Next G implements, then H inspects artifacts and runtime receipts. Operator approves gates. Any conflicting vocabulary or authority boundary HALTS the affected integration only.

## Non-negotiable acceptance checks
1. Muse alone mints intake UUIDs; no notebook UUID creation.
2. UUID terminates at Canon Collector; new Muse workload receives new UUID, parent linked.
3. Canon Collector and Sequence-and-Corpus notebooks remain separate.
4. Historical exclusions never silently become accepted canon.
5. Ontology Spark cannot make POLICY semantic decisions.
6. No automatic GPT approval or reasoning in scheduled poller.
7. Question depth protected by bounded coverage and sufficient preparation time.
8. Five-email GPT queue ceiling and 3+3 preload modeled; no invented shared queue visibility.
9. Both collision branches verified.
10. Independent inspection plus Operator acceptance before freeze or cleanup.
