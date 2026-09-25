# RelayDesk: from search question to supported answer

[Back to portfolio](../README.md)

**Independent demonstration · Fictional product · Specification version 1.0 · September 2026**

A small support team sees the same customer issue arrive as several tickets. The team lead wants to know why this happens, whether tickets can be combined, and what information the support team needs if the problem continues.

This project follows that question from discovery to action. It includes content someone can read, knowledge an assistant can reference, and rules for handling uncertainty.

## The project at a glance

| Decision | Choice and reason |
| --- | --- |
| Audience | A small-team support lead who needs an answer without a long setup guide |
| Entry question | “Why are we getting duplicate support tickets?” |
| Content sequence | Explain the problem → check the product rules → complete the task → escalate if needed |
| Knowledge boundary | All product behavior comes from the fictional specification below |
| Main risk | An answer could recommend combining unrelated conversations or promise an unavailable undo |
| Evidence boundary | This is a designed sample, not a deployed product or a measured campaign |

## Explore the deliverables

1. [Content strategy and search brief](01-content-strategy.md): intent, prioritization, page roles, metadata, and editorial decisions.
2. [Search article](02-search-article.md): a complete reader-facing explanation.
3. [Task guide](03-help-guide.md): a procedure with checks and a clear completion state.
4. [Product facts and knowledge records](04-product-facts-and-knowledge.md): the source of truth, structured FAQ, ownership, and version rules.
5. [AI instructions and evaluation](05-ai-instructions-and-evaluation.md): answer boundaries, worked examples, and test cases.
6. [Measurement and maintenance](06-measurement-and-maintenance.md): how to evaluate usefulness and respond to content or product changes.

## What the project demonstrates

The same fact appears differently depending on the reader's task. “Only open tickets from the same customer can be merged” becomes a short limitation in an article, a prerequisite in a guide, and an explicit answer constraint for an assistant. The meaning stays consistent.

A further decision is just as important: merging tickets organizes an existing conversation; it does not prevent future duplicate submissions. The content repeats that distinction at the points where a reader might otherwise assume the problem is solved.

## Scope and authorship

RelayDesk is invented for this sample and is separate from the PulseDesk sample in my technical portfolio. Product behavior is deliberately limited to make the knowledge and review process inspectable. Keywords are editorial hypotheses, not search-volume research. Worked answers are illustrative, not recorded model outputs. The evaluation suite has not been run against a model or a live service.

This portfolio sample was prepared with AI assistance. It demonstrates content and review design; it does not claim production implementation, paid-search management, or measured customer impact.
