# AI Client Acquisition Agent

**Status: In development — internal proof of concept, not a deployed client product.**

An internal B2B prospect research, qualification and human-reviewed outreach preparation workflow for a UK AI automation consultancy.

## Business problem
Prospect discovery, research, qualification and follow-up are time-consuming. This project explores evidence-grounded automation without inventing business problems or sending unsolicited messages automatically.

## MVP scope
- Research UK recruitment agencies: five initial prospects, then a target batch of 25.
- Record verifiable company facts, source URLs and research dates.
- Apply transparent fit scoring and exception handling.
- Prepare AI-assisted outreach drafts for explicit human approval.
- Track review and follow-up statuses.

## High-level workflow
Google Sheets → Make.com validation → research/enrichment → deterministic fit scoring → AI-assisted draft → human review → CRM tracking and notifications.

## Current progress
- [x] Imported a 26-column Google Sheets prospect tracker.
- [x] Confirmed Make.com Search Rows reads synthetic test record TEST-001.
- [x] Import and inspect a validation router with a fallback branch; verify synthetic opted-out and missing-website cases reach fallback.
- [x] Verify initial Router routing with three synthetic cases: valid record, opt-out and missing website.
- [ ] Complete expanded edge-case tests and evidence verification.
- [ ] Verify five real prospect records and evidence sources.
- [x] Test deterministic fit scoring and evidence-completeness routing with synthetic data; no outreach generation yet.
- [x] Verify a controlled Google Sheets write-back to the intended synthetic row (three cells updated).
- [ ] Implement separate human approval, suppression and contact-eligibility gates.
- [ ] Test AI-assisted draft generation (review only; no sending).
- [ ] Complete UAT and a safe demo.

## Disclosure
This public repository intentionally excludes complete scenario blueprints, proprietary implementation logic, credentials, account metadata, private prompts and real prospect records. Examples will be synthetic or redacted. No automated sending in v1.

## Licence
No open-source licence is granted at this stage. All rights reserved unless otherwise stated.

## Disclaimer
This is a self-directed internal development project; targets are not validated customer results.
