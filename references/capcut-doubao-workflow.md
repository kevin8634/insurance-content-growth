# Jianying + Doubao Workflow

This Skill prepares the production pack before the user works in Jianying and Doubao. It does not call either product, render MP4 files, or publish content.

## Division of Labor

- Skill: topic, insurance-safe copy, scene prompts, timeline, subtitles, cover, CTA, and review notes.
- Jianying: digital-human narration, voice, captions, visual assembly, music, transitions, disclosure label, and export.
- Doubao: short illustrative inserts, normally 15 seconds each, subject to the user's current quota and product limits.

## Recommended Assembly

1. Create or select the digital human in Jianying.
2. Paste the approved narration without changing product facts or numbers.
3. Generate no more insert prompts than the available daily quota. Default to a maximum of five when the user explicitly provides a five-clip budget.
4. Generate each insert independently in 9:16. Keep the prompt self-contained because clips may not preserve context between generations.
5. Import the inserts into Jianying and place them only at the mapped narration ranges.
6. Add subtitles, cover text, transitions, sound effects, background music, and the AI-generated-content disclosure in Jianying.
7. Review the final assembled video, not only the script. Confirm that inserts do not imply an unsupported insurance result.
8. Export the video and retain the script version, prompt pack, source references, and review decision together.

## Prompt Anatomy

Every insert prompt should specify:

- Visual subject and setting
- One visible action
- Camera angle and movement
- Lighting, color, mood, and realism level
- Continuity cues for the previous and next insert
- 9:16 vertical framing
- No subtitles, logos, watermarks, policy documents, exact money figures, medical outcomes, or identifiable real people unless explicitly authorized

Use scenes that explain a concept: a family reviewing a checklist, a calendar, a calm consultation setting, an abstract safety net, or a person organizing documents. Do not use a hospital discharge, payment receipt, stamped policy, or smiling customer as visual proof of a claim unless the user supplies and approves the source.

## Editing Rules

- Keep the digital human as the factual narrator and return to it before a new claim or boundary statement.
- Use inserts to create visual rhythm, not to introduce new facts.
- Do not allow generated clips to cover required disclaimers or insurer/product identification.
- Prefer hard cuts or short dissolves; avoid distracting transitions in professional insurance content.
- Keep background music below the voice and duck it further during exclusions, conditions, and CTA.
- Add a visible AI-generated-content disclosure when required by applicable rules and platform workflow.

## Failure Handling

- If an insert produces text, logos, distorted hands, fake documents, or a misleading event, regenerate with a stronger negative prompt or omit the insert.
- If the script changes after any insert is generated, regenerate the timeline mapping and mark the previous production pack obsolete.
- If a user has fewer generations than planned, keep C1 and C2, remove decorative inserts, and preserve the factual digital-human sections.
