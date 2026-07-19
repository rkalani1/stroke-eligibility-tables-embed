# AutoMedBench-Lite Gate for Eligibility Table Updates

Use this gate before accepting AI-generated changes to eligibility tables, embed code, copy-paste tables, or public-demo instructions.

This gate evaluates whether the update was checked. It does not make the tables current, approved, or operational.

## S1 Plan

- Identify the exact table, trial, criterion, contact field, or embed behavior being changed.
- State whether the change is content, presentation, documentation, or deployment guidance.
- Define stop conditions for source uncertainty, conflicting criteria, or missing review.

## S2 Setup

- Inspect `index.html`, `protocol_tables_preview.html`, `TELESTROKE_COPY_PASTE_TABLES.md`, `COMPLIANCE.md`, and any source materials.
- Confirm all examples are synthetic or public.
- Identify manual render checks for the table and embed view.

## S3 Validate

- Match each table row to study-owner-approved or IRB/HSD-approved source material where applicable.
- Preserve NCT IDs, criterion wording, review dates, and contact-routing caveats exactly.
- Confirm the personal GitHub Pages URL is not framed as approved for organizational embedding.
- Confirm no PHI, participant data, confidential contacts, or operational workflow details are introduced.

## S4 Execute

Make the smallest scoped table or embed update after S1-S3 are complete.

## S5 Submit

Report changed files, source trace, render/manual checks, residual owner review, and no-PHI confirmation.

## One-Shot Prompt

```text
Apply the stroke-eligibility-tables-embed AutoMedBench-Lite gate. Write S1 Plan, S2 Setup, and S3 Validate before editing. Then execute the scoped change and submit changed files, source trace, render checks, residual owner review, and no-PHI confirmation. Stop if current eligibility-source validation cannot be completed.
```
