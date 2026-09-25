# Measurement and maintenance plan

[Project overview](README.md)

**All metrics below are proposed. No analytics or customer results have been collected.**

## What success would mean

Readers understand whether a merge is appropriate, can complete the eligible task, and know when further investigation is needed. Fewer contacts alone would not establish success: people might abandon the task or fail to find support.

| Question | Proposed measure | Interpretation limit |
| --- | --- | --- |
| Does the page reach the intended audience? | Relevant query impressions and clicks, grouped by intent | Search visibility is not task success |
| Does the article lead to useful help? | Article-to-guide clicks divided by article sessions | A reader may receive the answer without clicking |
| Can readers complete the task? | Voluntary task-success responses after guide use | Respondents may not represent all readers |
| Are the same questions recurring? | Merge-related contacts per 100 merge attempts | Requires event data and a consistent issue taxonomy |
| Are assistant answers supported? | Fully supported product claims divided by all product claims in reviewed responses | Review a representative sample; retain critical-failure counts separately |
| Does escalation work? | Appropriate escalations divided by cases requiring escalation | A lower escalation rate is not automatically better |

## Proposed collection and analysis

Agree on an issue taxonomy with support: eligibility, procedure, failed attempt, mistaken merge, and recurrence. Establish a baseline window before changing content. Compare equivalent windows, noting product changes, audience mix, and ticket volume. Treat a before-and-after difference as an observation, not proof of causation.

Where feasible, test one content change at a time with an appropriate comparison group. For small samples, report counts and uncertainty rather than a confident percentage improvement. Keep raw customer conversations out of public analysis and use approved, minimal event data.

## Illustrative signals and decisions

These are hypothetical scenarios, not findings.

| Signal | Next investigation | Possible content response |
| --- | --- | --- |
| Readers open the guide but repeatedly ask about permissions | Check the visibility and wording of prerequisites | Move the role requirement closer to the entry point |
| Readers expect merging to stop future duplicates | Inspect article wording and assistant answers | Make the cleanup/prevention distinction more explicit |
| Assistant answers invent attachment handling | Inspect retrieval and unknown-answer behavior | Add an explicit unknown record and expand evaluation cases |
| Helpfulness rises but mistaken merges also rise | Check warning comprehension and confirmation design | Pause promotion of the flow and review content with product |

## Product-change workflow

If product introduces undo in a future version, P5 becomes a blocking dependency. Before publishing guidance, product must establish eligibility, limits, and exact procedure. Then update RD-K04, the article, the task guide, assistant rules, and E01/E05/E10. Keep version-specific guidance separate so the new rule is not applied to older customers without evidence.

Suggested responsibilities: product confirms behavior; support contributes issue patterns; content owns language and source traceability; the AI implementation owner manages retrieval and runtime controls. These are proposed roles for the sample, not a claim about a past team's process.

## Change log

| Version | Date | Change | Validation status |
| --- | --- | --- | --- |
| 1.0 | 2026-09-24 | Initial portfolio sample | Editorial and link checks only; no live product or model test |
