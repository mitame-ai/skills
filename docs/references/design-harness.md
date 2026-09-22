# Design harness research references

Research date: **2026-09-22 (Asia/Tokyo)**. This is the source log for the English `build-design-harness` skill in this workspace. Summaries and implementation choices are original synthesis; the linked material remains authoritative for what its authors actually report.

## How the research is packaged

This file is the bibliography for maintainers. It is not a reading prerequisite for using the skill. Website links are kept here, outside `build-design-harness/`.

- [Skill entrypoint](../../build-design-harness/SKILL.md): concrete deliverables and the implementation sequence.
- [Design concepts](../../build-design-harness/references/concepts.md): standalone principles, conditions of use, and practical implications. Source attribution is retained only in this bibliography.
- [UI build specification](../../build-design-harness/references/patterns.md): artifact layout, connected contract examples, state transitions, and a runnable token-pipeline example.
- [Verification implementation](../../build-design-harness/references/verification.md): executable assertions, report semantics, rejection/correction proof, and evidence handling.
- [Communication-design build specification](../../build-design-harness/references/communication.md): brief, brand rules, narrative, editable patterns, export checks, and contextual review.

The bundled token generator and tests are original, dependency-free implementation examples. They demonstrate generation and drift enforcement, not a complete UI harness. Example values are illustrative and must not become a target project's brand policy without a project-specific basis.

## Reading scope and evidence

The research covers official websites, event announcements, social posts, practitioner blogs, published slide transcripts, and public GitHub repositories. Both requested events were checked directly in their rendered Peatix pages. Those pages and the Design Harness site initially returned incomplete text to the web reader; browser inspection recovered their content. Speaker Deck transcripts were read for the substantive talks listed below. No private event recording was obtained or implied.

`#1` and `#2` below identify the first event and its official **2nd** edition; the first event's published title does not include `#1`. Some agenda titles differ from the titles speakers used for their published decks. Dates are event dates unless a separate publication date is stated. All URLs below were accessed or inspected on the research date. Repository links use mutable branches unless otherwise noted; implementation details should be rechecked before reuse. Repositories were inspected, not installed or executed.

## Concept and official examples

### C1 — Design Harness community site

- Author: Design Harness / Lumilinks.
- URL: <https://design-harness.com/>
- Read: definition, four-layer model, example directory, article links, and event index in the rendered page.
- Lesson: combine design-system knowledge with a process for inspecting and improving generated work. A harness covers more than the appearance of a single screen.
- Use: the skill's opening model and its product/communication scope. The four responsibilities do not prescribe a universal folder structure.

### C2 — Kogiso, “デザインハーネスとは何か”

- Published: 2026-05-08.
- URL: <https://note.com/kgsi/n/n707d989e1a44>
- Read: definition, four responsibilities, and practical adoption patterns.
- Lesson: design systems provide existing foundations; the weak point is often verification and connecting feedback to the next task.
- Use: start from existing sources and implement a complete production/check/revision path. DESIGN.md, Storybook, and MCP are examples of that path, not mandatory products.

### C3 — Atlas public demo

- Author: Lumilinks.
- URL: <https://demo-ds.design-harness.com/>
- Read: live overview, source-data explanation, navigation to foundations, patterns, rules, and experiments.
- Lesson: people, agents, documentation, and validation can share the same underlying design information.
- Use: source ownership and composition guidance. This is explicitly a demo, not proof of general production reliability.

### C4 — CrossRel event index

- Author: CrossRel.
- URL: <https://crossrel.jp/>
- Read: event links and second-event description.
- Use: verified the organizer and the intended emphasis of the second event; followed official event links rather than inferring the series from search results.

## Design Harness #1 — 2026-07-09

### E1 — Official first-event page

- Organizer: CrossRel. Venue: PKSHA Technology, Hongo TK Building.
- URL: <https://peatix.com/event/5053623/>
- Published alias: <https://design-herness.peatix.com/view> (the spelling is the actual published URL).
- Read: rendered date, scope, agenda, and speaker descriptions. The main sessions began at 19:00 JST; admission began at 18:30.
- Coverage: brand differentiation, four-layer UI harnesses, browser QA and review loops, small-team prototyping, organizational adoption, design participation, and Framer's agent experience.
- Use: identify the original talks and retain the distinction between standard quality and decisions that belong to people. Agenda descriptions were not treated as measured outcomes.

### E1-A — r.kagaya, “エンジニアにデザインハーネスを”

- Published: 2026-07-09. The agenda used a browser-QA/design-review title; the deck explicitly identifies the first event.
- URL: <https://speakerdeck.com/rkaga/design-harness-from-an-engineers-perspective>
- Read: browser-visible transcript, particularly slides 11–20 and 25–26; direct web-reader retrieval failed.
- Lesson: define the process leading to acceptance, including observable evidence, invariants, stopping conditions, and a way to return unresolved work to a person.
- Use: explicit evidence statuses, bounded iteration, and verification through the actual workflow. Do not rely on an agent's statement of completion.

### E1-B — Hiromi Maeo, “凡庸を落とすハーネス”

- Organization: enhanced. Published: 2026-07-09.
- URL: <https://speakerdeck.com/hiromimaeo/fan-yong-woluo-tosuhanesu>
- Read: transcript, particularly slides 5–12.
- Lesson: branding can require testing the distinctiveness of intent, while leaving execution room for judgment. The talk's substitution exercise makes generic positioning easier to discuss.
- Use: optional branding critique in the communication reference. It is not an automated truth test or a reason to demand novelty in routine UI/code.

### E1-C — Haruka Shimizu, “1000人規模の組織でデザインハーネスを導入するための第一歩”

- Organization: PKSHA Technology. Published: 2026-07-09.
- URL: <https://speakerdeck.com/pkshadeck/1000ren-gui-mo-nozu-zhi-dedezainhanesuwodao-ru-surutamenodi-bu>
- Read: transcript covering initial scope, testing, distribution, feedback, and adoption.
- Lesson: validate with a small audience, assign domain owners, and make adoption and feedback convenient before expanding across a varied organization.
- Use: one complete pilot and an explicit maintenance path. A company-wide deployment is not a prerequisite for a useful harness.

## Design Harness #2 — 2026-09-15

### E2 — Official second-event page

- Organizer: CrossRel. Venue: Tokyo Portcity Takeshiba, Office Tower 30F.
- URL: <https://peatix.com/event/5139487/>
- Read: rendered date, scope, agenda, and nine speaker descriptions. Sessions began at 18:30 JST; admission began at 18:00.
- Emphasis: communication design, brand, graphics, marketing material, and how to preserve contextual judgment alongside product/UI practices.
- Speakers represented Reiwa Travel, Timee, SoftBank, Findy, Framer, Money Forward, Light Light, CONCENT, and Goodpatch.
- Use: ensure the skill supports communication work as well as product UI. Topic descriptions establish the event's scope, not efficacy claims.

### E2-A — Akari Katakai, “デザインハーネスをつくるハーネス”

- Organization: Goodpatch. Published: 2026-09-15.
- URL: <https://speakerdeck.com/katakai/dezain-hanesu-o-tsukuru-hanesu-dare-demo-jisharashii-dezain-o-tsukureru-you-ni-suru-shikumi>
- Read: transcript, especially slides 7, 10–16, 18–19.
- Lesson: reuse a common building process while extracting service-specific content; include how the resulting harness will be used and maintained in everyday work.
- Use: reusable workflow with product-specific context, plus feedback ownership. The presentation's synchronization mechanism is not made a requirement for a single project.

### E2-B — Sayaka Kubouchi, “Agentic Design Workflowを育てる『三層デザインハーネス』の現在地”

- Organization: SoftBank. Event: 2026-09-15; deck published 2026-09-17 with some modifications.
- URL: <https://speakerdeck.com/sayadesign2/agentic-design-workflow-o-sodateru-sansou-dezain-hanesu-no-genzaichi>
- Read: description and transcript covering validation findings and design decision records.
- Lesson: correct components do not ensure a coherent page; missing composition guidance should become explicit improvement work and recorded decisions.
- Use: composition contracts and scoped shared/product/task knowledge. The talk describes continuing validation and future measurement, not a completed universal solution.

### E2-C — Kohei Nishikawa / niccy, “LP制作のための熱量ハーネス”

- Organization: Findy. Event and deck: 2026-09-15.
- URL: <https://speakerdeck.com/niccy/lp-seisaku-no-tame-no-netsuryou-hanesu-hito-no-netsuryou-o-ai-tono-seisaku-ni-tsunagu>
- Read: transcript, especially brief, story, wireframe, and selection rationale sections.
- Lesson: preserve the audience, intent, missing facts, and reasons for choosing a narrative as the work moves between artifacts.
- Use: the communication-design path. The particular number of questions, alternatives, or catalog patterns is not generalized into a requirement.

### E2-D — Kota Saito, “デザイナーの判断をAIにつなぐ ── 審美眼をハーネスする試み”

- Organization: CONCENT. Event and deck: 2026-09-15.
- URL: <https://speakerdeck.com/kotasaito_cnt/dezaina-no-handan-o-ai-ni-tsunagu-shinbi-me-o-hanesu-suru-kokoromi>
- Read: transcript, especially slides 20–36.
- Lesson: aesthetic judgment concerns relationships among purpose, information, audience, and expression. Fixing local spacing can leave the underlying communication problem unchanged.
- Use: contextual preference/decision records and brief-specific review. This is exploratory practice, not a claim that taste has been fully mechanized.
- Corroborating company report, published 2026-09-18: <https://www.concentinc.jp/news-event/news/2026/09/design-harness-2ndevent/>.
- Advance announcement, published 2026-09-04: <https://www.concentinc.jp/news-event/seminar/2026/09/design-harness-2nd-202609/>.

## Practitioner blogs and additional research

### P1 — Tetsuo Hashimoto, LayerX / Bet AI Day 2026

- Published: 2026-09-03. This is a separate event, not Design Harness #1 or #2.
- URL: <https://speakerdeck.com/layerx/bet-ai-day-2026-session05>
- Title: “デザインハーネス：専門職の判断基準をコードのように運用する”.
- Read: transcript, particularly slides 13–21.
- Lesson: observable rules with IDs and strengths make reviews traceable; lack of a relevant rule should remain visible as inability to evaluate.
- Use: rule metadata and honest evaluation states. General advice is kept separate from compliance decisions. Reported internal results were not independently reproduced.

### P2 — Money Forward Design, code-prototype workflow

- Published: 2026-09-01.
- URL: <https://note.com/mfdesign/n/n51eb399cefc0>
- Title: “開発を速くする、ハーネスで支えるコードプロトのデザインプロセス”.
- Read: rationale, knowledge organization, and generation/review flow.
- Lesson: operational knowledge needs a short entrypoint with task-specific detail; interactive prototypes expose states and inconsistencies that static pictures can conceal.
- Use: progressive loading and real flow validation. The article's multi-agent organization and migration away from design files are local choices, not defaults imposed by this skill.

### P3 — Sansan Product management & Design, learning logs

- Published: 2026-09-02.
- URL: <https://note.com/sansan_cpo/n/n0df771f4ef2f>
- Title: “AIプロトタイピングの精度を上げる—デザインハーネスをチームで育てる方法”.
- Read: reported failure modes, collection/curation process, and current limitations.
- Lesson: collecting corrections is different from deciding which ones should affect future work; route accepted knowledge to the relevant scope.
- Use: curated feedback instead of indiscriminate memory injection. The author explicitly says it is too early to validate the effect.

### P4 — Jiun / MIXI, starting with design review

- Published: 2026-08-28.
- URL: <https://note.com/nanapink0503/n/n4d5ae2ccf3f5>
- Title: “『デザインハーネス』って、結局何をすればいい？ まずはデザインレビューから”.
- Read: review-first proposal and embedded organizer post.
- Lesson: a small, scoped review workflow can reveal missing team judgment criteria without first building a generation platform.
- Use: respect review-only adoption when that is the requested task.

### P5 — Anthropic, generator/evaluator experiments

- Published: 2026-03-24.
- URL: <https://www.anthropic.com/engineering/harness-design-long-running-apps>
- Title: “Harness design for long-running application development”.
- Read: frontend evaluator, calibration, revision behavior, and application QA sections.
- Lesson: inspecting working artifacts and calibrating rubrics can improve evaluation, while iterative scoring can also produce convergence, increasing complexity, and revisions a person likes less.
- Use: inspect evidence, bound retries, preserve good revisions, and avoid equating a higher score with better product judgment. No mandatory agent count or iteration count is adopted.

## GitHub implementation references

### G1 — lumilinks-hq/atlas-design-system

- Repository: <https://github.com/lumilinks-hq/atlas-design-system>
- Experiment procedure inspected: <https://github.com/lumilinks-hq/atlas-design-system/blob/main/docs/EXPERIMENTS.md>.
- Read: README architecture, source ownership, rule-result handling, and experiment procedure.
- Lesson: keep baseline, harness-assisted, and feedback-corrected runs distinguishable; collect measurements before evaluating and preserve human-review items separately.
- Use: executable evidence, controlled comparisons, and avoiding duplicate authoritative data. The demo's recorded counts are not reproduced or used as performance promises.
- Access note: direct web-reader requests to the `design/` and `scripts/` directory pages failed; those directory contents were not claimed as inspected.

### G2 — BilLogic/harness-designing-plugin

- Repository: <https://github.com/BilLogic/harness-designing-plugin>
- Setup skill inspected: <https://github.com/BilLogic/harness-designing-plugin/blob/main/skills/hd-setup/SKILL.md>.
- Read: README's five-layer model and setup skill's existing-material discovery.
- Lesson: inventory the team's existing context and tools before selecting what needs building.
- Use: reuse-first discovery. Its five-layer taxonomy is an alternative framing; it is not silently merged with the Japanese community's four-layer model. Its installation flow, multi-agent orchestration, and repeated confirmation gates are not copied into this skill.

## Social sources

### S1 — Kogiso's second-event announcement and reply on X

- Original post: <https://x.com/kgsi/status/2090574411812548685>.
- Reply linking the official event and hashtag: <https://x.com/kgsi/status/2090574414790418741>.
- Posted: 2026-08-21 JST (2026-08-20 UTC; the embedded note rendering uses the earlier date).
- Read: both posts in the existing browser session after direct web-reader access returned HTTP 403. No new sign-in was requested.
- Use: verify the social announcement's connection to the official second event and discover `#デザインハーネス2`. Popularity and engagement are not evidence of design quality or harness effectiveness.

## Synthesis applied to the skill

| Skill decision | Supporting sources | Boundary retained |
| --- | --- | --- |
| [Connect four responsibilities](../../build-design-harness/references/concepts.md#connect-four-responsibilities) | C1, C2, E1-C, P4 | Four responsibilities do not require four packages or a large platform. |
| [Delegate execution while retaining intent](../../build-design-harness/references/concepts.md#delegate-execution-while-retaining-intent) | C2, E1-A, P4 | Execution delegation does not surrender product judgment or expand the requested scope. |
| [Preserve authority and distinguish kinds of knowledge](../../build-design-harness/references/concepts.md#preserve-authority-and-distinguish-kinds-of-knowledge) | C3, P1, G1, G2 | A template or demo stack does not replace the user's authoritative design information. |
| [Evaluate composition and relationships](../../build-design-harness/references/concepts.md#evaluate-composition-and-relationships) | E2-B, E2-D | Aesthetic preferences and local layout corrections are not universal rules. |
| [Preserve intent between production stages](../../build-design-harness/references/concepts.md#preserve-intent-between-production-stages) | E1-B, E2, E2-C, E2-D | Narrative selection and brand differentiation are conditional on the task and medium. |
| [Match evidence to the claim](../../build-design-harness/references/concepts.md#match-evidence-to-the-claim) | E1-A, P1, P5, G1 | Missing evidence and unresolved judgment remain visible. |
| [Bound evaluation and compare honestly](../../build-design-harness/references/concepts.md#bound-evaluation-and-compare-honestly) | E1-A, P5, G1 | A demo comparison is not a general quality benchmark. |
| [Make knowledge available at the point of use](../../build-design-harness/references/concepts.md#make-knowledge-available-at-the-point-of-use) | E2-A, E2-B, P2, G2 | Knowledge structure does not impose a tool migration, fixed layer count, or multiple agents. |
| [Curate feedback and design for adoption](../../build-design-harness/references/concepts.md#curate-feedback-and-design-for-adoption) | E1-C, E2-A, P3 | Raw logs and unreviewed anecdotes do not become global policy. |

The example rule record, decision record, result vocabulary, and verification menu in the skill are this workspace's synthesis. They are not attributed as a schema or standard defined by any one source. The research supports mechanisms and tradeoffs; it does not establish a single industry standard for “design harness.”
