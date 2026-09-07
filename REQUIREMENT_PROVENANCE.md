# Provisional requirement provenance and evidence-review map

## Scope and status

Fork baseline: `1cbc74c2d6e5096392fbf7fa48b9136f65810cd7` (2025-08-30), tree
`0c87bc158e9e5fb9453b607da35287da6e03cdf5`. The identical commit/tree was
also read in `Entkenntnis/robot-karol-online`. This proves document lineage,
not the original author/requester of every requirement or a platform mandate.

Six root Markdown documents were read as text: README, QUESTSCRIPT, RKO-MODULE,
KAROL-X-PYTHON, MATERIAL-LEHRKRAEFTE and WEB RESOURCES. The large gallery, linked
images/PDFs/websites, exercise data, application source, CI and runtime behavior
are not fully reviewed here. This is not a claim about every instruction in
all subdirectories. Root tree inspected; recursive response exceeded display
limits. All inherited files remain byte-for-byte unchanged by this amendment.

Each row is a bounded starting point for [a source-equipped reviewer](PROVENANCE_REVIEW_TEMPLATE.md),
not a claim of final message-level attribution. **Original origin unresolved**
is compatible with verified upstream document lineage. Requirements already
presented as operative stay operative; examples and research notes stay such.
Rationales below are stated purposes or explicit unknowns, not invented history.
No individual confirmation by this fork's user was found in the inspected sources.

## Source-specific review rows

| ID | Exact location / clause | Original origin | Rationale | Applicable status | Evidence question |
|---|---|---|---|---|---|
| RK-01 | [README.md][source-1] — Übersicht: Playful introduction to sequence, loops and conditionals. | Unresolved | Stated goal: introduction to algorithmic thinking; origin of each scope choice unknown. | Documented product goal in the inherited baseline; no fork-user confirmation evidenced. | Which upstream educational/design source selected these topics? A curriculum mention alone does not establish an external mandate. |
| RK-02 | [README.md][source-1] — Sprache / Anweisungen, Steuerung, Bedingungen, Eigene Anweisungen: Documented command/control/condition syntax and behavior. | Unresolved | Historical choice of each syntax element unknown. | Existing language reference, not newly proposed here. | Split individual syntax/behavior clauses when tracing compatibility requests or design history. |
| RK-03 | [README.md][source-1] — Sprache / Hauptprogramm: Only the main-program block executes when several parts exist; connected code has a fallback. | Unresolved | Unknown; a practical reason must not be reconstructed as history. | Existing documented execution selection. | Find original introduction/compatibility decision; distinguish the two cases. |
| RK-04 | [README.md][source-1] — Textmodus: Object-style spelling, legacy * syntax, comment forms and ignored semicolons. | Unresolved | Unknown original rationale; compatibility is suggested by the wording, not proved as the original motive. | Documented accepted syntax. | Trace each independent compatibility choice to its introducing commit and discussion. |
| RK-05 | [README.md][source-1] — Aufgabensammlung / umfangreiche Beispiele / Links / Trivia: Hosted or self-hosted tasks, illustrative algorithms, reference links and character pronouns. | Unresolved | Educational/examples context is stated; detailed historical reasons unknown. | Mixed documentation and examples; neither a fork deployment authorization nor a universal new requirement. | Extract any normative clause before classification; preserve attribution and avoid treating examples as user instructions. |
| RK-06 | [README.md][source-1] — Entwicklung / Betrieb: Development/build flow, output directory, cross-origin isolation example, backend customization. | Unresolved | Purpose stated: running/building the app and supporting Python mode. | Existing operational guidance; exact platform-mandate provenance not independently checked. | Separate local choices from actual browser/runtime constraints; cite versioned interface evidence for the latter. |
| RK-07 | [QUESTSCRIPT.md][source-2] — Opening / __ide_run_client: QuestScript replaces normal control; client runs in a fresh environment with documented variable transfer. | Unresolved | Stated purpose: inspect code variables/functions as well as world changes. | Existing local API contract; not a statement about all Python runtimes. | Locate the design discussion; split fresh globals, copied inputs, outputs and protected __ide_ names. |
| RK-08 | [QUESTSCRIPT.md][source-2] — Opening / __ide_set_progress / __ide_get_progress: World-completion logic, no-change result, and explicit progress override. | Unresolved | Unknown original rationale for acceptance semantics. | Documented exercise-completion state, not approval of a product requirement. | Which task/design source chose each completion criterion? A learner click is not rule confirmation. |
| RK-09 | [QUESTSCRIPT.md][source-2] — __ide_prompt / __ide_exit / __ide_sleep: Prompt/continue behavior, immediate exit, and prefer __ide_sleep over time.sleep. | Unresolved | Unknown original rationale for the sleep preference. | Existing API/preference; prompt confirmation is local UI interaction. | Find runtime/design justification and any original request; keep button semantics separate from provenance approval. |
| RK-10 | [QUESTSCRIPT.md][source-2] — __ide_get_outputs / __ide_get_inputs / __ide_set_world / Beispiel: I/O inspection and experimental world mutation; example task checks. | Unresolved | Stated purpose: verify print/input and control worlds. | Documented API; world setter explicitly experimental, example not a global acceptance rule. | Preserve the experimental/no-check warning; trace target selectors, types and coordinate convention separately. |
| RK-11 | [RKO-MODULE.md][source-3] — Rectangle / Roboter-Steuerung: Geometry, mutability, directions and robot methods. | Unresolved | Stated purpose: shape the Python experience; detailed original choices unknown. | Existing API description and examples. | Split method contracts, defaults and examples; find introducing upstream decisions. |
| RK-12 | [RKO-MODULE.md][source-3] — tick / resetCanvas / exit / clearOutput / sleep: Frame tick default 20, elapsed-time result, canvas and output lifecycle. | Unresolved | Stated purpose for tick: animation pacing; original default selection unknown. | Documented defaults/methods. | Was 20 requested, chosen, or inherited? Trace return-unit and lifecycle rules independently. |
| RK-13 | [RKO-MODULE.md][source-3] — enableArrowKeys / isPressed: Enable arrow keys before querying pressed state. | Unresolved | Dependency stated, underlying historical design rationale unknown. | Existing documented precondition, not confirmed user preference. | Find implementation/interface history supporting the precondition; repetition in the note adds no provenance. |
| RK-14 | [RKO-MODULE.md][source-3] — Audio und Musik: Synth/Drumkit contracts, duration conventions, positive integer BPM, volume integer range -100 to 12. | Unresolved | Function purposes stated; exact ranges/default origins unknown. | Existing local API constraints. | Split BPM/range/duration requirements and find local design versus named library constraints. |
| RK-15 | [KAROL-X-PYTHON.md][source-4] — Fernsteuerung: Register a key before querying it; key uses KeyboardEvent.key values. | Unresolved | Stated rationale: prepare the UI; the external key-values reference is named. | Existing local precondition plus claimed external representation. | Check versioned key-value interface separately; it does not establish the local registration design. |
| RK-16 | [KAROL-X-PYTHON.md][source-4] — Other examples: Sample programs including a bounded castle size, quiz, network example and Tetris. | Unresolved | Stated purpose: examples to try; historical choice of details unknown. | Illustrations, not universal product limits or authority to run/network now. | Only promote a sample constraint after finding a separate requirement; keep sample parameters as examples. |
| RK-17 | [MATERIAL-LEHRKRAEFTE.md][source-5] — Musterlösung / Lernpfad / Windows-Installer / Einstieg / Kahoot: Teacher-resource access and use instructions. | Unresolved | Resource purpose stated; original access/distribution decision not recovered. | Inherited instructions/pointers, not a fork release or contact policy. | Trace access workflow and distinguish upstream service instructions from fork-user requirements. |
| RK-18 | [WEB RESOURCES.md][source-6] — Entire annotated link list: External resource notes and evaluations. | Unresolved | Resource exploration visible; original research assignment unknown. | Reference/research notes, not adopted external mandates. | Identify an actual normative claim before treating any linked resource as a requirement. |

[source-1]: https://github.com/sockpuppet9000/robot-karol-online/blob/1cbc74c2d6e5096392fbf7fa48b9136f65810cd7/README.md
[source-2]: https://github.com/sockpuppet9000/robot-karol-online/blob/1cbc74c2d6e5096392fbf7fa48b9136f65810cd7/QUESTSCRIPT.md
[source-3]: https://github.com/sockpuppet9000/robot-karol-online/blob/1cbc74c2d6e5096392fbf7fa48b9136f65810cd7/RKO-MODULE.md
[source-4]: https://github.com/sockpuppet9000/robot-karol-online/blob/1cbc74c2d6e5096392fbf7fa48b9136f65810cd7/KAROL-X-PYTHON.md
[source-5]: https://github.com/sockpuppet9000/robot-karol-online/blob/1cbc74c2d6e5096392fbf7fa48b9136f65810cd7/MATERIAL-LEHRKRAEFTE.md
[source-6]: https://github.com/sockpuppet9000/robot-karol-online/blob/1cbc74c2d6e5096392fbf7fa48b9136f65810cd7/WEB%20RESOURCES.md

## Exact next-pass workflow

Choose a row, split independently decidable clauses, and populate the worksheet
with original message/turn or upstream issue/design evidence. Record speaker,
context and supporting scope, original rationale or its absence, current rule
status, later confirmation and a correction trail. Search the original source,
not only a summary claiming what someone wanted. Keep contrary evidence visible.
No actual rollout has been inspected in this pass. The worksheet is also usable
when no rollout exists and the source is an upstream project decision.

## Provenance of this amendment

The distinction itself is an explicit first user request in conversation
`6a9e453e-97a0-83eb-8590-0a0bc0d2be7c`. After checkpoint 005, the user also
expressly welcomed the PRs as templates for precise attribution by a person or
agent holding original rollouts. The category vocabulary and retrospective
approach were identified as another agent's proposal. New AGENTS guidance,
row grouping, fields and this evidence procedure are this reviewer's design
proposal, not individually confirmed implementation details. Origin is not
quality; silence and general continuation do not confirm individual rules.

## Parallel draft and remaining scope

Draft PR #1 at `88829a73f75287efc33f625ffd8b313e8be4110f` proposes fork-status
and backlog text. Its metadata and manifest were read; its 14 additional packages
and full discussions are not yet reviewed here. They require a separate coverage
pass before combination. The earlier self-declared session entry is preserved,
not evidence of adopting that draft. This PR neither changes upstream nor
chooses synchronization, archive, deletion or a fork product. No application,
installer, model, service or deployment was executed; no private history imported.
