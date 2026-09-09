# Technical Design

## Current Release Scope

`v0.2.0` adds a bounded 7-day AI agent training experiment on top of the content-production Skill. It is not the complete V1 product and does not include cohort management, automated assignment collection, group messaging, payments, renewals, publishing, or outcome guarantees.

The training module produces learner work artifacts: an AI work map, AI insurance advisor profile, weekly content library, video production pack, customer-management workflow, role-play report, AI agent workflow, and 30-day action plan.

## Product Positioning

The Skill is the MVP for an eventual “insurance content growth and compliance pre-review” product. Its core value is not generic text generation or video rendering. It combines an insurance-domain content workflow, source-aware claims handling, beginner production guidance, a Jianying/Doubao production pack, and a human review checkpoint.

## MVP Scope

### In Scope

- User brief to weekly content plan
- Single short-video script and teleprompter copy
- Platform-specific repurposing
- CTA and public-comment reply suggestions
- Evidence labels and compliance pre-review
- Exportable structured output for manual Jianying and Doubao production
- 7-day training tasks, learner submissions, assignment feedback, role-play practice, and graduation assessment

### Out of Scope for MVP

- Automatic insurance recommendation or underwriting
- Automatic publication, direct customer outreach, or video rendering inside the Skill
- Final legal/compliance approval
- Product database without a controlled update process
- Collection or storage of health, identity, or financial data
- Claims or sales conversion guarantees
- Cohort database, automatic homework collection, group broadcast, payment, renewal, or coach CRM

## Suggested Software Architecture

1. `Brief Layer`: persona, audience, platform, topic, objective, and source uploads.
2. `Knowledge Layer`: versioned approved documents with insurer, product, effective date, region, and usage scope.
3. `Generation Layer`: mode-specific prompt and output schema.
4. `Claim Layer`: extract claims, attach evidence level, and block unsupported material claims.
5. `Review Layer`: rule checks plus human approval, with immutable version history.
6. `Delivery Layer`: paste-ready narration, Doubao prompt pack, timeline map, subtitle text, and Jianying assembly checklist. Video rendering remains external.
7. `Analytics Layer`: publish status, inquiry count, qualified inquiry, and user feedback. Do not infer sales causality from views alone.
8. `Training Layer`: day-specific task, input checklist, submission artifact, acceptance criteria, feedback, graduation result, and next-day handoff. Keep it stateless in the Skill; a future coach tool may persist cohort records.

## Data Model Minimum

- `creator_profile`: role, organization, licensed region, tone, target audience
- `source_document`: title, issuer, version, effective date, expiry date, access scope, hash
- `content_request`: brief, platform, objective, requested format, created by
- `content_version`: draft, evidence map, risk status, reviewer, approved time
- `lead_event`: source content, consent status, channel, qualification status
- `audit_event`: actor, action, timestamp, previous version, new version
- `production_pack`: narration version, insert prompts, insert budget, timeline map, editing plan, disclosure status

## Safety and Reliability

- Version every source and generated content item.
- Expire or quarantine source documents that are past their effective date.
- Keep generated copy, evidence mapping, and reviewer decision together.
- Redact sensitive data from logs and prompts.
- Require explicit confirmation before content is marked ready for publication.
- Make rule-based blocking deterministic; use the model for explanation and rewrite suggestions.
- Treat analytics as directional unless there is a controlled attribution method.
- Keep the approved narration version and the generated-insert version linked; never allow a later script edit to silently invalidate an already-reviewed production pack.

## Evaluation Plan

Test with realistic requests across education, product explanation, claims guidance, and lead replies. Score:

- Factual grounding: every material claim has acceptable evidence.
- Risk detection: blocking phrases and missing conditions are flagged.
- Usability: a novice can record the script without rewriting it.
- Platform fit: title, length, and structure match the selected platform.
- Conversion quality: CTA produces qualified questions without pressure.
- Stability: the same source and brief produce materially consistent risk decisions.

Start with 20 interviews and a concierge pilot. The strongest paid signal is repeated weekly use plus prepayment, not compliments or one-time generations.

## Migration Path

1. Skill-only: prompt workflow and manual source confirmation.
2. Lightweight web app: saved profiles, source uploads, reusable templates, and exports.
3. Team product: review queue, role permissions, document versioning, and audit trail.
4. Optional media layer: provider integrations only after the manual Jianying/Doubao workflow proves retention, cost tolerance, and compliance handling.
