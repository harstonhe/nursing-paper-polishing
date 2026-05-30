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
- `references/section-moves.md` when the requested revision needs section-specific writing logic for nursing, midwifery, health services, public health, or medical journals.
- `references/writing-diagnostics.md` before substantial polishing, reviewer-comment revision, paragraph rebuilding, or full-section rewriting.
- `references/phrasebank-playbook.md` when the section logic is clear and phrase-level support is needed for hedging, transitions, limitations, implications, or future work.
- `references/citation-positioning.md` when revising Introduction, Background, Discussion, literature comparisons, novelty claims, or reviewer-facing justification.
- `references/style-mechanics.md` for grammar, articles, abbreviation, number/unit, punctuation, register, and mechanical style checks after the main rewrite.
- `references/inclusive-medical-language.md` for medical, nursing, aging, disability, sex/gender, race/ethnicity, stigma, or participant-description language checks.
- `references/qian-systems-thinking.md` when the task involves complex revision planning, reviewer-comment triage, missing-section reconstruction, multi-source evidence synthesis, or repeated manuscript improvement loops.

## Default Stance

- Polish for clarity, restraint, methodological transparency, and relevance to international nursing and health care readers.
- Language serves the scientific argument. Do not polish sentences while leaving the section's reasoning, reporting logic, or evidence boundary broken.
- Treat study design as the first constraint on language.
- Make the contribution precise: what uncertainty is reduced, what question is clarified, or what practice, policy, workforce, education, or methods issue is better understood.
- Use the `claim-evidence-boundary` standard for every important sentence: what is being claimed, what supports it, and where the claim stops.
- Treat a manuscript as an evidence-control system: every claim needs an evidence input, every journal or reviewer requirement is a constraint, and every revision should reduce uncertainty or improve traceability.
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
6. Diagnose the failure mode before editing. Use `references/writing-diagnostics.md` to decide whether the issue is paper-type logic, section role, paragraph progression, claim-evidence mismatch, citation positioning, Results/Discussion mixing, or sentence-level mechanics.
7. For complex or repeated revisions, model the task as a feedback loop: identify the control goal, evidence inputs, journal/reviewer constraints, current error signal, and next revision action. Use `references/qian-systems-thinking.md` when helpful.
8. If the target journal and article content/design are specified, perform an exemplar article scan before polishing. Find 2-3 comparable full-text articles from the same journal or publisher family, prioritizing the same study design.
9. Identify the exact manuscript section being polished or completed, such as Abstract, Introduction, Methods, Results, Discussion, Limitations, Conclusion, Highlights, or title page. If the section is not explicit, infer it from headings and content; if inference is unsafe, ask for the section before doing a section-specific rewrite.
10. Load `references/section-moves.md` when the section's move order is unclear or the paragraph needs restructuring.
11. Apply the `claim-evidence-boundary` and claim-scope checks before sentence polishing. Remove, qualify, or mark unsupported claims.
12. Audit Methods and Results first, because they determine what the rest of the manuscript can legitimately claim.
13. If the requested section is missing or only notes are provided, use `references/section-completion.md` to draft evidence-constrained prose before polishing.
14. Polish Discussion, Limitations, and Conclusions next, keeping interpretation tied to the findings.
15. Revise Background after the evidence logic is clear, using it to justify the problem, gap, and objective.
16. Polish Abstract, Title, Keywords, highlights, significance statement, impact statement, or social media abstract last according to the selected journal.
17. Run phrase, citation, inclusive-language, causality, and mechanical style checks after the structure is correct.
18. If the user provides a `.docx`, tables, figures, captions, EndNote files, or asks for submission readiness, run formatting, citation/reference, encoding, and file-integrity QA after language revision.

## Diagnostic Workflow

Before rewriting a substantial paragraph or section, identify the main failure mode.

Prioritize fixes in this order:

1. `paper type`: the manuscript is using the wrong logic for its design or article type.
2. `section job`: the paragraph is doing the work of another section, such as Discussion inside Results.
3. `paragraph logic`: the paragraph lacks one controlling idea or mixes unrelated propositions.
4. `claim-evidence-boundary`: the claim has no evidence, the evidence has no point, or the implication exceeds the design.
5. `citation positioning`: prior work is misrepresented, uncited, over-flattened, or used to manufacture novelty.
6. `sentence polish`: grammar, concision, transitions, rhythm, and mechanics.

If a section is structurally underdeveloped, briefly state the structural diagnosis before the polished version unless the user asks for direct output only.

## Claim-Evidence-Boundary Standard

Every important scientific statement should pass three checks:

- `Claim`: What exactly is the sentence saying?
- `Evidence`: Which result, table, method detail, participant quote, statistic, protocol item, or verified source supports it?
- `Boundary`: What design limit, population limit, setting limit, uncertainty, or reviewer concern constrains the claim?

Repair common failures before polishing:

- claim without evidence: qualify, remove, or request author input;
- data without a point: add the specific interpretation supported by the data;
- implication without boundary: add scope, uncertainty, or future-work language;
- association written as mechanism: replace causal wording with design-appropriate wording;
- review evidence written as trial evidence: describe mapped, synthesized, or appraised evidence rather than effectiveness.

When evidence is missing, use `AUTHOR_INPUT_NEEDED: [specific missing evidence]` rather than smoothing over the gap.

## Claim-Scope Audit for Preliminary Evidence

Before polishing Abstract, Discussion, Implications, Limitations, and Conclusions, check whether the manuscript's application-level claims exceed its evidence level.

Apply this audit especially to exploratory, simulation, feasibility, pilot, descriptive, qualitative, psychometric, preclinical, algorithmic, and other non-implementation studies.

High-scope language includes:

- `clinical use`, `clinical decision-making`, `clinical decision support`, `practice recommendation`, `guideline development`, `deployment`, `implementation`, `real-world readiness`, `reliable support system`, `replacement of professional judgment`, and `rapid response`.

Unless the study includes prospective validation, real-world implementation, patient or service outcomes, clinical safety testing, or formal guideline-development procedures, move claims to the correct evidence level:

- from clinical decision-making to decision preparation;
- from implementation to feasibility or readiness for validation;
- from replacement to complementing professional judgment;
- from guideline development to informing future consensus work;
- from effectiveness or clinical utility to potential usefulness, association, or hypothesis-generating evidence.

Use evidence-appropriate language such as `preliminary refinement`, `prioritization`, `feasibility signal`, `early-stage support`, `preparation for expert review`, `requires professional calibration`, and `warrants prospective or real-world validation`.

## Results and Discussion Boundary

Keep Results and Discussion distinct across all study designs.

Results should:

- report what was observed, measured, coded, appraised, synthesized, or mapped;
- specify the relevant sample, condition, comparison, time point, table, figure, theme, estimate, or rating;
- use past tense for completed observations and avoid long explanations of meaning;
- avoid practice recommendations, causal explanations, mechanism claims, and broad implications.

Discussion should:

- interpret principal findings in relation to the research question and prior work;
- explain plausible reasons for patterns without presenting speculation as fact;
- state implications for nursing, clinical practice, education, policy, management, or future research within the evidence boundary;
- acknowledge uncertainty, transferability, equity, feasibility, and safety where relevant.

For reviews, Results report what the evidence base contains. Discussion explains what the mapped or synthesized evidence may mean and where it remains limited.

## Citation Positioning and Fairness

Use citations to position the manuscript honestly, not only to decorate claims.

Do:

- cite the source actually read and verified;
- distinguish prior evidence, prior interpretation, methods borrowed, frameworks adapted, and points of contrast;
- acknowledge what earlier studies established before stating what remains uncertain;
- make novelty precise and bounded by population, context, method, outcome, or evidence type.

Do not:

- cite a paper for a claim it did not make;
- use a secondary source when the primary source is available and necessary;
- imply that previous work was absent, weak, or irrelevant just to strengthen the present manuscript;
- write `no studies`, `first`, `novel`, `pioneering`, or `little is known` unless the literature search supports that exact scope.

## Length and Proportion Control

Before drafting or polishing a section, identify any journal-specific length limits for the manuscript, abstract, structured abstract subheadings, highlights, limitations, conclusion, tables, figures, and supplementary files.

Apply this priority order:

1. Follow explicit limits from the target journal's current author guidelines, article type instructions, templates, or editor/reviewer comments.
2. If the journal gives no section-specific limit, infer a reasonable section length from 2-3 accessible full-text exemplar articles from the same journal and same article type or method.
3. If no target journal is specified, default to concise IJNS-style proportions and the same-design nursing SCI exemplars available from the scan.

For Abstract, Limitations, and Conclusion:

- Keep the section proportional to the full manuscript and to the journal's published examples.
- Treat an abstract word limit as a ceiling, not a target. Unless the user asks for a full-length abstract, default to a submission-efficient version at roughly 65%-80% of the stated journal limit while preserving the complete logic loop.
- When the user provides a target-journal exemplar abstract, treat its word count, sentence count, subsection length, and information density as explicit constraints. If the first polished version is longer than the exemplar by more than about 15%-20%, compress it before delivery.
- For abstracts, perform a compression pass after drafting: remove secondary background, procedural detail, repeated metric explanations, non-decisive statistics, discussion-like interpretation, and claims that do not affect editorial judgment.
- Treat abstracts as engineered decision systems rather than shortened manuscripts. Identify the target reader's decision problem and the manuscript's main contradiction, then compress through five moves: gap, objective, design, decisive evidence, and bounded implication. Preserve only information that closes this logic loop.
- For abstracts reporting complex evaluations, compress by evidence layers rather than deleting metrics mechanically. Preserve one or two decisive indicators from each evidence layer that supports the manuscript's main claim, such as task performance, agreement or similarity, implementation feasibility, safety, acceptability, reliability, or human/expert validation. Prefer indicators that add non-redundant evidential value.
- Do not report all available metrics unless each changes the reader's decision. After compression, audit whether the retained indicators reflect the author's intended argument and whether all named outcomes, dimensions, and validation terms are consistent across Objective, Methods, Results, and Conclusions.
- Do not make limitations or conclusions longer than the evidence warrants.
- Avoid generic extended summaries in Conclusion. State the mapped evidence, its meaning for nursing/clinical audiences, and the research boundary.
- For scoping and systematic reviews, Limitations should address search scope, language/full-text restrictions, heterogeneity, evidence gaps, and review-process boundaries without implying that the review design was expected to establish causality.

For generated output:

- Keep the complete polished response under 8,000 characters unless the user or journal explicitly requests a longer text.
- Allocate words across sections according to rhetorical weight. Methods and Results may need more detail; Limitations and Conclusion should usually be compact unless the target journal's examples support a longer format.
- If the user's draft exceeds the target length, compress before adding new material.

## Exemplar Article Adaptation

When a target journal and study design/content are available, use `references/exemplar-article-scan.md`.

The scan should:

- Search the target journal first, then the publisher family if the journal has too few matches.
- Prefer 2-3 full-text articles from the target journal, same article type, and same or adjacent design published within the last 3 years.
- Use 4-5-year-old exemplars only if fewer than two suitable same-journal examples are available from the last 3 years, and state this limitation in revision notes.
- Avoid using exemplars older than 5 years to calibrate current abstract headings, word count, section density, or journal-format expectations unless the user explicitly provides that exemplar or no newer same-journal examples exist.
- Treat older classic methods or reporting papers as methodological references, not as current journal-style exemplars.
- Require the same study design plus at least one content match whenever possible.
- Exclude articles whose full text or relevant manuscript section cannot be accessed. Abstract-only pages, metadata records, indexing pages, and citation databases are not sufficient exemplars.
- Maximize topic similarity first, then relax topic components stepwise. Use same-design full-text articles with no topic overlap only as the last same-journal fallback.
- Extract section-specific patterns only. For example, use Abstract exemplars to revise abstracts, Introduction exemplars for gap logic, Methods exemplars for reporting sequence, and Results exemplars for statistical reporting.
- For abstract exemplars, extract operational constraints before rewriting: exact headings, total length, subsection length, sentence count per subsection, methods/design detail, findings/results density, conclusion scope, and final relevance/practice-implication brevity if such a subsection exists.
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
- Avoid turning descriptive or exploratory evidence into policy or practice imperatives. Use `may be useful for`, `could be considered`, or `future intervention studies are needed to evaluate`.
- Keep causal conclusions aligned with results. Do not claim effectiveness, benefit, risk reduction, or improved outcomes unless directly tested.

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
- If adapting to a provided journal exemplar, match its density as well as its structure: keep each subsection to 1-2 sentences when the exemplar does so, avoid turning findings/results into detailed mini-results, and keep any final relevance, application, or practice-implication subsection compact.
- Do not add a `Clinical Relevance` heading unless the target journal, author guidelines, template, or user-provided exemplar uses that heading. For Journal of Nursing Scholarship, use the JNS-style abstract headings only when JNS is the target or exemplar basis.
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

When the user asks for submission formatting, works in a Word manuscript, or provides tables/figures, apply the target journal's explicit instructions first. If the journal is silent and the user gives formatting instructions, follow the user. If neither is available, apply these defaults as a consistency standard:

- Use `Times New Roman` throughout the manuscript, including body text, headings, references, tables, figure captions, and notes.
- Use body text size 12 pt (Chinese xiaosi / small-four body size) for the main text, abstract, references, table notes, and figure captions unless a template explicitly differs.
- Use major heading size 14 pt (Chinese sihao / fourth-size heading) for main headings such as Introduction, Methods, Results, Discussion, Limitations, Conclusion, and References; bold all main headings.
- Use 12 pt bold for subheadings unless the journal requires another hierarchy.
- Use double line spacing by default for journal submission manuscripts and references, unless the journal or user requests 1.5 spacing or another setting.
- Separate paragraphs clearly. Do not output dense, unbroken blocks of text.
- Use single-column, editable Word-compatible text, justified body alignment where appropriate, first-line body paragraph indentation, and standard 1-inch / 2.54 cm margins unless instructed otherwise.
- Use a consistent heading hierarchy and avoid decorative heading styles, colored fonts, unnecessary italics, or inconsistent spacing.
- Use italics only where required, such as statistical symbols, species names, or template conventions; remove leftover template instruction italics before submission.
- Ensure tables and figures use readable, consistent typography: usually 10-11 pt Times New Roman for table body text and 8-10 pt for figure panel labels or axis text, with no unnecessary styling.
- Keep table titles above tables and figure captions below figures, unless the user's target template requires another placement.
- Define all abbreviations used in tables or figures in table notes or figure captions.
- Check that table and figure numbering follows order of first citation in the text.
- For final polish, report any formatting deviations separately from language revision notes.

## Encoding, Citation, And File QA

Before final delivery, scan the entire output, including DOCX XML/text, Markdown, references, tables, captions, and exported reference files, for encoding or text-corruption artifacts. Fix broken accented names such as `P?rez-Esteve`, broken apostrophes such as `one?s` or `author?s`, Unicode replacement characters such as `U+FFFD`, garbled symbols, corrupted non-English names or journal titles, broken hyphens/dashes/minus signs, and question marks that are not real punctuation.

Run citation and reference QA before final delivery:

- Check that every in-text citation has a matching reference entry.
- Check that every reference entry is cited in the text, unless intentionally included as supplementary background.
- Verify DOI, PMID, PMCID, or publisher metadata when available.
- Ensure author names, years, article titles, journal names, volume, issue, pages/article numbers, and DOI links are consistent across text, tables, and References.
- Mark unresolved or uncertain references with `[REF-CHECK: issue]` rather than silently guessing.
- If the user requests EndNote compatibility, export references as `.ris`, `.nbib`, or another importable format.

Before telling the user the work is complete, verify the DOCX package opens structurally or passes validation, required formatting was actually written into the file XML/styles, no encoding artifacts remain, paragraphing is readable, and the writing respects the study design without overclaiming beyond the evidence.

## Output Format

Default output:

1. Polished text.
2. `Revision notes:` with 3-5 short bullets covering design-language fit, target-journal structure, causality restraint, statistical clarity, and style variation.
3. `Causality check:` one sentence stating whether causal language was allowed, restricted, or removed.

If an exemplar article scan was performed, add:

4. `Exemplar basis:` with the 2-3 full-text articles used, their DOI/URL when available, access source, and the section-level patterns that informed the revision. State if fewer than 2 full-text exemplars were available.

If formatting was requested or a manuscript file was provided, add:

5. `Formatting check:` with concise notes on font, size, line spacing, headings, paragraphing, tables, figures, captions, abbreviations, and unresolved items.
6. `Final QA:` when files or references were produced, report citation/reference consistency, encoding scan status, file integrity, and EndNote export status when relevant.

If the user asks for tracked reasoning or teaching feedback, provide:

- `Original`
- `Polished`
- `Why changed`

If the manuscript section is underdeveloped, first give a brief `Structural diagnosis`, then provide the polished version.

If the section was drafted from notes or partial materials, add:

- `Evidence used:` with the author-provided inputs that supported the draft.
- `Author input needed:` listing any placeholders or missing evidence.
