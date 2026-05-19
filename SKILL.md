---
name: nursing-paper-polishing
description: Polish, restructure, translate, draft missing sections for, or audit nursing, midwifery, digital health, and medical SCI manuscripts for a target journal or publisher style, with IJNS as a built-in profile. Use when the user asks for nursing SCI English polishing, target-journal writing adaptation, missing paragraph or section completion from uploaded notes/files, IJNS/JMIR/Elsevier/Wiley journal adaptation, Journal of Advanced Nursing as a Wiley journal, journal-specific abstract/highlights/title rewriting, exemplar article scans from the target journal, format checks, causality and overclaim checks, scoping/systematic review polishing, research paper polishing, or inclusive medical language revision.
metadata:
  author: Harston
---

# Nursing SCI Journal Polishing

Use this skill to polish nursing, midwifery, digital health, health services, and medical manuscripts for a target journal. Preserve the author's meaning, data, study design, and intellectual contribution. Do not invent evidence, citations, mechanisms, novelty claims, methods, or implications.

## Source References

Load these references as needed:

- `references/ijns-requirements.md` when the target is IJNS or a similar Elsevier nursing journal.
- `references/journal-adaptation.md` when the target is JMIR, Elsevier, Wiley, a Wiley journal such as Journal of Advanced Nursing, or another journal/publisher.
- `references/exemplar-article-scan.md` when the user specifies both a target journal and article content/design, or asks to adapt wording to published articles from that journal.
- `references/section-completion.md` when the user asks to write, complete, rebuild, or fill a missing paragraph/section from uploaded notes, partial drafts, tables, figures, reviewer comments, or other manuscript materials.
- `references/inclusive-medical-language.md` for medical, nursing, aging, disability, sex/gender, race/ethnicity, stigma, or participant-description language checks.

## Default Stance

- Polish for clarity, restraint, methodological transparency, and relevance to international nursing and health care readers.
- Treat study design as the first constraint on language.
- Make the contribution precise: what uncertainty is reduced, what question is clarified, or what practice, policy, workforce, education, or methods issue is better understood.
- Prefer evidence-informed wording over promotional claims.
- Keep nursing context visible without overstating local generalizability.
- Use inclusive, person-respecting, internationally understandable language.
- Apply the inclusive medical language standard across all target journals unless the journal has stricter wording.
- Avoid frequent em dashes. Prefer commas, parentheses, semicolons, or shorter sentences.
- Avoid overly symmetrical parallel sentences that sound artificial.
- Avoid repeating the same sentence frame, transition, or opening pattern more than twice in nearby paragraphs.

## Target Journal Detection

Before polishing, identify the target from the user's instruction, uploaded template, manuscript title page, or journal URL.

Use this priority order:

1. User-provided journal instructions, template, or editorial email.
2. Current official author guidelines from the journal or publisher website.
3. Built-in profile in `references/journal-adaptation.md`.
4. Publisher-level rules, such as Elsevier, Wiley, or JMIR.
5. General nursing SCI language standard.

If the target journal is named and its current instructions are not available in the skill references, search the official author guidelines before applying journal-specific formatting. Use publisher or journal official pages first. If browsing is unavailable, ask the user to upload or paste the author guidelines and continue with general language polishing only.

If no target journal is specified, default to IJNS-style constraints for nursing SCI rigor and load `references/ijns-requirements.md`.

Do not transfer one journal's format to another. For example, do not apply IJNS article highlights to JMIR unless JMIR requests them, and do not apply JMIR's AMA style to IJNS unless the target journal requests AMA.

## Journal-Adaptive Workflow

Do not follow the Nature-style writing order by default. Use a design-first and reporting-first order:

1. Identify target journal or publisher: IJNS, JMIR, an Elsevier journal, a Wiley journal such as Journal of Advanced Nursing, or another named journal.
2. Identify article type: research paper, review, discussion paper, letter/commentary, editorial, protocol, viewpoint, implementation report, research letter, or brief report.
3. Identify the study design: randomized trial, quasi-experimental study, cohort, cross-sectional survey, qualitative study, mixed-methods study, psychometric/instrument validation, systematic review, scoping review, discussion paper, or methods paper.
4. Identify the relevant reporting guideline before polishing: CONSORT, STROBE, COREQ, SRQR, PRISMA, PRISMA-ScR, JBI scoping review guidance, COSMIN, GRRAS, TRIPOD, CHEERS, TIDieR, SAMPL, or another suitable EQUATOR guideline.
5. Extract journal-specific constraints: abstract headings and word count, keywords, highlights or significance statement, main text headings, references, tables/figures, anonymization, data availability, AI disclosure, and formatting.
6. If the target journal and article content/design are specified, perform an exemplar article scan before polishing. Find 2-3 comparable full-text articles from the same journal or publisher family, prioritizing the same study design.
7. Identify the exact manuscript section being polished or completed, such as Abstract, Introduction, Methods, Results, Discussion, Limitations, Conclusion, Highlights, or title page. If the section is not explicit, infer it from headings and content; if inference is unsafe, ask for the section before doing a section-specific rewrite.
8. Audit Methods and Results first, because they determine what the rest of the manuscript can legitimately claim.
9. If the requested section is missing or only notes are provided, use `references/section-completion.md` to draft evidence-constrained prose before polishing.
10. Polish Discussion, Limitations, and Conclusions next, keeping interpretation tied to the findings.
11. Revise Background after the evidence logic is clear, using it to justify the problem, gap, and objective.
12. Polish Abstract, Title, Keywords, highlights, significance statement, impact statement, or social media abstract last according to the selected journal.
13. If the user provides a `.docx`, tables, figures, captions, or asks for submission readiness, audit formatting consistency after language revision.

## Exemplar Article Adaptation

When a target journal and study design/content are available, use `references/exemplar-article-scan.md`.

The scan should:

- Search the target journal first, then the publisher family if the journal has too few matches.
- Prefer 2-3 recent or highly relevant full-text articles using the same design.
- Require the same study design plus at least one content match whenever possible.
- Exclude articles whose full text or relevant manuscript section cannot be accessed. Abstract-only pages, metadata records, indexing pages, and citation databases are not sufficient exemplars.
- Maximize topic similarity first, then relax topic components stepwise. Use same-design full-text articles with no topic overlap only as the last same-journal fallback.
- Extract section-specific patterns only. For example, use Abstract exemplars to revise abstracts, Introduction exemplars for gap logic, Methods exemplars for reporting sequence, and Results exemplars for statistical reporting.
- Compare patterns across exemplars and synthesize the writing logic; do not copy sentences or imitate one article too closely.
- Cite or list the exemplar articles used in revision notes when internet search was performed.

## Missing Section Completion

Use `references/section-completion.md` when the user uploads only a missing paragraph file, a rough outline, tables, figures, extracted results, reviewer comments, or partial manuscript notes and asks Codex to write or complete a manuscript section.

Completion is allowed only when enough author-provided evidence is available. Keep the user's evidence as the ceiling for every claim.

Do:

- reconstruct the section's rhetorical job from the target journal profile and same-section full-text exemplars;
- map each sentence to an author-provided fact, table, figure, result, method detail, or cited source;
- use `AUTHOR_INPUT_NEEDED: [specific missing item]` when essential evidence is absent;
- draft the missing paragraph or section, then apply the same polishing, causality, inclusive-language, and target-journal checks.

Do not:

- invent findings, mechanisms, sample sizes, effect sizes, eligibility criteria, dates, databases, tools, ethics approval, registration numbers, citations, limitations, or implications;
- write Results from no data, Methods from no protocol, or Discussion claims from no findings;
- disguise missing information with vague polished language.

## Causality Guardrail

Before rewriting claims, classify the design as causal or non-causal.

Treat language as causal only when the design supports causal inference, such as a well-conducted randomized trial, a robust quasi-experimental design, or an explicitly justified causal inference framework. Even then, preserve the exact estimand and assumptions.

For non-causal designs, including cross-sectional studies, descriptive surveys, qualitative studies, scoping reviews, most systematic reviews, psychometric validation, exploratory mixed-methods work, and correlational analyses:

- Do not write causal verbs such as `enhance`, `improve`, `promote`, `prevent`, `reduce`, `increase`, `lead to`, `result in`, `drive`, `impact`, `influence`, or `determine` unless the sentence is only reporting an observed association and cannot be read as causal.
- Replace causal or interventionist wording with cautious alternatives:
  - `may inform`
  - `may support`
  - `has the potential to support`
  - `could guide`
  - `is associated with`
  - `was related to`
  - `may help identify`
  - `may provide a basis for`
  - `could be considered when developing`
  - `warrants further evaluation`
- Avoid policy or practice imperatives from descriptive evidence. Use `may be useful for`, `could be considered`, or `future intervention studies are needed to evaluate`.
- Keep conclusions aligned with results. Do not claim effectiveness, benefit, risk reduction, improved outcomes, or clinical utility unless directly tested.

## IJNS Section Logic

### Title

- Prefer the IJNS pattern `Topic: method/design`.
- State the population, phenomenon, intervention, or method clearly.
- Do not include abbreviations.
- Avoid causal or effectiveness claims unless the design directly supports them.
- For submission-facing work, remind the author to provide a short article title for the manuscript header.

### Abstract

- Keep the abstract concise, factual, and stand-alone.
- Use the structure required by the relevant reporting guideline or IJNS template.
- Keep the optional social media abstract to 140 characters when the user is preparing full IJNS submission materials.
- For research papers, usually use: `Background`, `Objective`, `Design`, `Setting(s)`, `Participants`, `Methods`, `Results`, `Conclusions`, and `Registration` when relevant.
- For reviews, usually use: `Background`, `Objective`, `Information sources`, `Methods`, `Results`, `Conclusions`, and `Registration` when relevant.
- In Results, include point estimates and confidence intervals when statistical results are reported.
- In Conclusions, only state conclusions that follow directly from the reported findings.

### Article Highlights

Use the IJNS headings:

- `What is already known`
- `What this paper adds`

Write two or three single-sentence bullets under each heading. Each bullet should be short, outcome-focused, and no more than 85 characters when the user is preparing submission materials. Do not describe the paper's process as the contribution.

### Background

- Open with the nursing, patient, caregiver, workforce, policy, education, or health service problem.
- Move quickly to what is known, what remains uncertain, and why the uncertainty matters.
- End with a clear objective or research question.
- Avoid long generic statements about global burden unless they directly justify the study.

### Methods

- Make the design, setting, participants, sampling, measurement, data collection, analysis, ethics, consent, and registration transparent.
- For intervention studies, describe the intervention and comparator precisely enough for readers to judge reproducibility.
- For psychometric studies, state instrument development, validation sample, reliability, validity, criterion comparison when relevant, and whether the full instrument is available.
- For reviews, state databases, dates, eligibility criteria, screening, extraction, appraisal, synthesis approach, and registration.
- Use active clarity where appropriate, but keep methods impersonal and reproducible.

### Results

- Report what was observed before interpreting what it means.
- Prefer point estimates, confidence intervals, and clinically or practically meaningful effect sizes over p-value-centered prose.
- Avoid `significant` as a substitute for magnitude, direction, or uncertainty.
- Do not duplicate tables. Summarize the most decision-relevant findings and point readers to tables for detail.
- Keep qualitative findings grounded in themes, participant perspectives, and illustrative evidence without overgeneralizing.

### Discussion

- Start with the principal findings, not a repeat of the background.
- Explain how findings relate to prior nursing and health services literature.
- Separate interpretation from implication.
- Discuss uncertainty, transferability, feasibility, and equity when relevant.
- Avoid repetitive transition chains such as `Moreover`, `Furthermore`, or `In addition` across consecutive paragraphs.

### Limitations

- Name limitations that matter for interpretation, not generic disclaimers.
- Link limitations to their likely effect on findings, transferability, bias, or precision.
- Do not over-apologize. State what the design can and cannot support.

### Conclusions

- Use a restrained three-part close: central finding, practical or scholarly meaning, and boundary.
- For non-causal work, close with wording such as `These findings may inform...` or `Further studies are needed to evaluate...`
- Do not introduce new results, recommendations, or unsupported clinical claims.

## Sentence-Level Style

- Aim for 15-28 words per sentence in polished prose.
- Keep one main proposition per sentence when reporting methods or results.
- Vary sentence openings across a paragraph.
- Do not use the same transition word more than once in adjacent paragraphs. Track `Moreover`, `Furthermore`, `In addition`, `However`, `Therefore`, and `Taken together`.
- Avoid more than two uses of the same structure, such as `This study...`, `These findings...`, or `It is important to...`, in a short section.
- Avoid excessive triads and polished but empty parallelism, such as three consecutive clauses with identical rhythm.
- Prefer precise verbs: `examined`, `estimated`, `described`, `explored`, `identified`, `synthesized`, `compared`, `evaluated`, `was associated with`.
- Avoid promotional verbs: `revolutionize`, `transform`, `dramatically improve`, `breakthrough`, `novel` unless novelty is justified.
- Define unavoidable abbreviations at first use, but avoid abbreviations in title and abstract unless firmly established.

## Formatting and Layout Audit

When the user asks for submission formatting, works in a Word manuscript, or provides tables/figures, apply the target journal's instructions first. If the target journal allows free-format submission or gives no specific formatting rule, apply these defaults as a consistency standard:

- Use `Times New Roman` consistently across the main manuscript.
- Use 12 pt font for the main text, abstract, headings, references, and figure/table captions unless a template explicitly differs.
- Use double line spacing for the main manuscript and references; keep spacing consistent across sections.
- Use single-column layout and editable Word-compatible text.
- Use consistent heading hierarchy and avoid decorative heading styles.
- Keep margins, paragraph indents, before/after spacing, page numbering, and header short title consistent.
- Use italics only where required, such as statistical symbols, species names, or template conventions; remove leftover template instruction italics before submission.
- Ensure tables and figures use readable, consistent typography: usually 10-11 pt Times New Roman for table body text and 8-10 pt for figure panel labels or axis text, with no unnecessary styling.
- Keep table titles above tables and figure captions below figures, unless the user's target template requires another placement.
- Define all abbreviations used in tables or figures in table notes or figure captions.
- Check that table and figure numbering follows order of first citation in the text.
- For final polish, report any formatting deviations separately from language revision notes.

## Output Format

Default output:

1. Polished text.
2. `Revision notes:` with 3-5 short bullets covering design-language fit, target-journal structure, causality restraint, statistical clarity, and style variation.
3. `Causality check:` one sentence stating whether causal language was allowed, restricted, or removed.

If an exemplar article scan was performed, add:

4. `Exemplar basis:` with the 2-3 full-text articles used, their DOI/URL when available, access source, and the section-level patterns that informed the revision. State if fewer than 2 full-text exemplars were available.

If formatting was requested or a manuscript file was provided, add:

5. `Formatting check:` with concise notes on font, size, line spacing, headings, tables, figures, captions, abbreviations, and unresolved items.

If the user asks for tracked reasoning or teaching feedback, provide:

- `Original`
- `Polished`
- `Why changed`

If the manuscript section is underdeveloped, first give a brief `Structural diagnosis`, then provide the polished version.

If the section was drafted from notes or partial materials, add:

- `Evidence used:` with the author-provided inputs that supported the draft.
- `Author input needed:` listing any placeholders or missing evidence.
