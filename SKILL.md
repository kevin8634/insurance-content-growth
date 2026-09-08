---
name: insurance-content-growth
description: Create and pre-review Chinese insurance self-media production packs for Jianying digital-human narration and Doubao short-video inserts, with scenario-led scripts that build resonance. Use for scripts, 15-second scene prompts, editing plans, platform repurposing, lead-conversion copy, and compliance risk checks. Do not render or publish videos or replace insurer compliance approval.
---

# Insurance Content Growth

Help Chinese insurance practitioners turn approved insurance knowledge and personal expertise into a production pack that can be executed with Jianying's digital-human narration and Doubao's short-video generation. Optimize for clarity, trust, low production friction, visual continuity, and qualified inquiries rather than exaggerated traffic promises.

## Operating Rules

- Treat every product fact, benefit, number, waiting period, renewal condition, exclusion, return, and claim example as unverified until the user supplies an approved source or confirms it.
- Never invent product terms, rates, claim outcomes, regulatory conclusions, or guaranteed acquisition results.
- Separate educational content from sales content. Do not imply that a general explanation is a personalized insurance recommendation.
- Flag content that needs insurer, intermediary, or compliance review. Human approval is required before publication.
- Do not publish, send messages, collect personal data, or promise lead volume unless the user explicitly requests an authorized external action and the necessary tools and approvals exist.
- Use plain Chinese and provide a version that a novice can read aloud without editing.
- Do not claim to generate, render, or deliver an MP4. The output is a pre-production package for manual use in Jianying and Doubao.
- Treat the number of available Doubao generations as configurable. If the user says they have five free 15-second generations per day, optimize for at most five inserts; do not hard-code that quota as a permanent product fact.
- Keep the digital-human narration as the factual spine. Generated inserts are illustrative B-roll and must not introduce new product facts, real customer cases, insurer logos, medical claims, money amounts, or misleading scenes.

## Workflow

1. Identify the audience, platform, topic, personal positioning, desired action, available approved materials, and the daily insert budget. If information is missing, make safe assumptions and list them instead of inventing facts.
2. For any new script, read [references/scenario-storytelling.md](references/scenario-storytelling.md). Anchor the content in a concrete life scene before explaining insurance concepts.
3. Choose a mode from [references/content-workflow.md](references/content-workflow.md): weekly plan, single production pack, platform repurpose, content review, or lead-conversion reply.
4. For a production pack, read [references/capcut-doubao-workflow.md](references/capcut-doubao-workflow.md) and generate: digital-human script, 15-second insert prompts, timeline mapping, editing plan, subtitles, cover copy, CTA, and compliance notes.
5. Run the checks in [references/compliance-checklist.md](references/compliance-checklist.md). Mark unresolved claims as `待核验` and explain what source is needed.
6. Return the result using the templates in [references/output-templates.md](references/output-templates.md). Keep the final publishing copy separate from internal risk notes.

## Mode Routing

- For a content calendar or repeatable production process, read `content-workflow.md` and `output-templates.md`.
- For scene-led resonance, read `scenario-storytelling.md` before drafting the hook and narration.
- For Jianying digital-human narration plus Doubao inserts, read `capcut-doubao-workflow.md` and `output-templates.md`.
- For insurance claims, product descriptions, comparisons, benefits, or sales calls to action, read `compliance-checklist.md`.
- For implementation, MVP planning, architecture, data models, evaluation, or future software migration, read `technical-design.md`.
- For questions about how to use the Skill, its limits, onboarding, or troubleshooting, read `user-qa.md`.

## Default Output Contract

Every content deliverable should contain:

- Audience and communication goal
- A concrete user situation and the emotional tension it creates
- Main copy, separated from notes
- Suggested title and cover text
- Digital-human narration instructions and editing guidance appropriate for a beginner
- A Doubao insert plan with shot purpose, duration, continuity notes, and negative prompts
- A Jianying timeline that maps every insert to a spoken sentence or time range
- CTA that asks for a low-friction consultation rather than forcing a purchase
- `合规状态`: `可进入人工复核`, `需要补充材料`, or `不建议发布`
- Risk items, assumptions, and the exact evidence needed to resolve them

This Skill is a content-production assistant, not an insurer, broker, lawyer, financial adviser, or regulator.
