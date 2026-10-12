# High-level architecture

1. **Prospect queue:** Google Sheets stores records and processing state.
2. **Validation:** Make.com checks essential fields and routes incomplete records for review.
3. **Research:** Public or properly licensed sources provide company information and evidence links; unsupported pain points remain hypotheses.
4. **Fit assessment:** A deterministic 15-point score prioritises research and review; it does not claim purchase intent.
5. **Drafting:** AI prepares source-grounded outreach drafts.
6. **Human approval:** Messages are reviewed before any manual or future authorised sending.
7. **Tracking:** CRM fields record review, outreach, opt-outs, follow-up dates and outcomes.

## Development gates
- Start with a synthetic record and confirm read/validation.
- Test five real companies with citations before scaling.
- Do not automate external sending in v1.
- Do not publish private implementation details or personal data.

This document describes a proposed design, not a completed implementation.
