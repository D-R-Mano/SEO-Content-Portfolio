# Content strategy: investigate repeated support tickets

[Project overview](README.md)

## The brief

**Reader:** A support lead noticing several tickets that appear to describe the same issue.  
**Reader outcome:** Distinguish a repeated submission from a separate issue, understand the available action, and know when to seek help.  
**Business hypothesis:** Clear guidance could reduce avoidable follow-up contacts about ticket handling. This hypothesis requires validation; it is not an observed result.

The scenario assumes a recurring question, not a real support-data finding. In a live project I would first check anonymized support themes and search queries before deciding its priority.

## Intent and page map

| Reader question | Intent | Content response | Next step |
| --- | --- | --- | --- |
| Why are we getting duplicate tickets? | Understand | Search article explaining checks and limitations | Read the merge prerequisites |
| How do I combine two tickets? | Complete a task | Task guide | Verify the merged conversation |
| Why is Merge unavailable? | Diagnose | Short FAQ linked to the prerequisites | Check role, status, and customer |
| Can I undo a merge? | Understand a limitation | Direct answer with escalation | Contact a workspace admin; do not promise recovery |
| Why do duplicates keep appearing? | Investigate recurrence | Distinguish cleanup from prevention | Record ticket IDs and contact support |

Candidate phrases: “duplicate support tickets,” “merge support tickets,” “support ticket merge unavailable.” These are unvalidated topic hypotheses. No search volume, keyword difficulty, or ranking forecast is implied.

## Page roles and metadata

| Page | Suggested title | Suggested meta description |
| --- | --- | --- |
| Search article | Duplicate Support Tickets: What to Check First | Check whether tickets describe the same issue, learn when merging is appropriate, and understand what a merge will not fix. |
| Help guide | Merge Two Tickets in RelayDesk | Check your role, ticket status, and customer before merging two RelayDesk tickets. Learn what changes and what to do if Merge is unavailable. |

The article addresses the broad question. The guide owns the product procedure. Each links to the other where the reader's next task changes. These are content specifications for a future website; a Markdown repository does not implement HTML meta descriptions or establish search performance.

## Editorial choices

- Lead with the decision the reader must make: are these really the same issue?
- Explain limitations before the procedure because merging cannot be undone in the sample product.
- Avoid a promise to “eliminate duplicates.” The feature consolidates existing tickets only.
- Keep hypothetical causes separate from verified product facts. The sample does not diagnose an integration fault.
- Use “ticket,” “customer,” and “merge” consistently across the article, guide, and FAQ.

## Prioritization and review

For this sample, prioritize the task guide and irreversible-action warning first, the explanatory article second, and the assistant answers third. Correctness of the source content is a dependency for automation.

In a real workflow, product would confirm behavior, support would review likely questions, and the content owner would check usability and consistency. The accessibility review would check heading order, descriptive links, and whether critical meaning is available in text rather than color alone.

**Release gate:** every procedural statement matches the [product specification](04-product-facts-and-knowledge.md), all next-step links resolve, and unresolved behavior questions are held for review.
