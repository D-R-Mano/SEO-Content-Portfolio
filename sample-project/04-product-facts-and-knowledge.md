# RelayDesk product facts and knowledge records

[Project overview](README.md)

## Source of truth

**Document ID:** RD-SPEC-1.0  
**Status:** Current within this fictional sample only  
**Effective date:** 2026-09-24  
**Proposed review roles:** Product owner verifies behavior; content owner maintains published guidance. These are workflow roles, not named participants in a real project.

| ID | Product fact |
| --- | --- |
| P1 | Only admins and team leads can merge tickets. Agents cannot merge tickets. |
| P2 | Both tickets must be open and belong to the same customer. |
| P3 | From the source ticket, choose More → Merge ticket, enter the destination ID, review the confirmation screen, and choose Confirm merge. The screen shows both IDs and the customer. |
| P4 | Source messages appear in the destination conversation in chronological order. The source is closed and references the destination. The destination retains its owner and status. |
| P5 | A merge cannot be undone. |
| P6 | Merging does not change routing or prevent future duplicate submissions. |
| P7 | For an unexpected failure, contact support with both ticket IDs and the time of the attempt. For a mistaken merge, contact a workspace admin. Restoration is not promised. |

## Deliberately unspecified

The sample does not define attachment handling, notifications, audit logs, subscription plans, APIs, regional differences, or reopening behavior. No content or assistant answer should fill these gaps with invented features. Similar products are not evidence for RelayDesk behavior.

## Knowledge records

| Record | User question | Approved answer | Source |
| --- | --- | --- | --- |
| RD-K01 | Who can merge tickets? | An admin or team lead can merge tickets. An agent cannot. | P1 |
| RD-K02 | Which tickets are eligible? | Both tickets must be open and belong to the same customer. Review the conversations to confirm that merging is appropriate. | P2; editorial review guidance |
| RD-K03 | What happens to the original ticket? | The source closes and references the destination. Its messages appear in the destination in chronological order. | P4 |
| RD-K04 | Can I undo a merge? | No. Contact a workspace admin if a merge was made in error; restoration is not promised. | P5, P7 |
| RD-K05 | Will merging stop duplicates? | No. Merging does not change routing or prevent future duplicate submissions. | P6 |
| RD-K06 | What if Merge is unavailable? | Check your role, whether both tickets are open, and whether they belong to the same customer. If eligible, contact support with the ticket IDs and attempt time. | P1, P2, P7 |

## Example structured record

```json
{
  "id": "RD-K04",
  "intent": "undo_merge",
  "question": "Can I undo a merge?",
  "answer": "No. Contact a workspace admin if a merge was made in error; restoration is not promised.",
  "source_document": "RD-SPEC-1.0",
  "source_fact_ids": ["P5", "P7"],
  "product_version": "1.0",
  "status": "current_in_sample",
  "reviewed_on": "2026-09-24",
  "review_trigger": "Change to merge reversibility or recovery guidance",
  "owner_role": "content_owner",
  "escalation_role": "workspace_admin"
}
```

The review date records preparation of the sample, not approval by a real product team. In production, a verified owner and approval record would replace the illustrative fields.

## Maintenance rule

A product change triggers a review of the fact, every dependent knowledge record, the help guide, the article, and the affected assistant tests. Conflicting or superseded records must be excluded from the approved answer set until the product owner resolves them. Preserve the prior version for an audit trail; do not silently overwrite the source history.
