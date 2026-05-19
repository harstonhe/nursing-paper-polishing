# Missing Section Completion

Use this reference when the user asks to write, complete, reconstruct, or fill in a missing manuscript paragraph or section from uploaded files, notes, tables, figures, results, protocols, reviewer comments, or partial drafts.

This mode composes `nursing-paper-polishing` with the evidence discipline of `adapt-journal-writing`: research the target journal and exemplars first, then draft only what the user's materials can support.

## Trigger

Run this mode when the user says or implies:

- "补全这一段"
- "只上传了缺失段落/材料，请帮我写"
- "write the missing paragraph"
- "complete the Discussion/Introduction/Methods"
- "draft based on these notes/tables/results"
- "按照目标期刊补写"
- "根据这几个结果写 Discussion"

## Minimum Inputs

Identify these before drafting:

- target journal or default profile;
- manuscript type and study design;
- target section or paragraph role;
- author-provided evidence or notes;
- existing surrounding text, if available;
- tables, figures, results, protocol, or search strategy when relevant.

If the target journal is not specified, default to IJNS-style nursing SCI rigor.

If the target section is not specified, infer it from headings and content only when safe. Otherwise ask for the section before drafting.

## Evidence Boundary

The user's materials set the ceiling for every claim.

Allowed evidence sources:

- uploaded manuscript paragraphs;
- author notes, bullet points, outlines, and tables;
- figures and captions;
- extracted results or statistical outputs;
- search strategy, protocol, registration, eligibility criteria, and screening records;
- cited references already provided by the user;
- target journal official guidelines;
- accessible full-text exemplar articles for structure only.

Exemplar articles can inform structure, tone, heading logic, and section-specific sentence moves. They cannot supply claims, findings, limitations, study details, or citations for the user's manuscript.

## AUTHOR_INPUT_NEEDED Rule

Use `AUTHOR_INPUT_NEEDED: [specific missing item]` when essential content is absent.

Examples:

- `AUTHOR_INPUT_NEEDED: exact database search dates`
- `AUTHOR_INPUT_NEEDED: number of records screened at full text`
- `AUTHOR_INPUT_NEEDED: main finding from Table 2`
- `AUTHOR_INPUT_NEEDED: ethics approval details`
- `AUTHOR_INPUT_NEEDED: citation supporting this background claim`

Do not hide missing information behind vague prose.

## Section-Specific Completion Rules

### Abstract

Draft only after Methods and Results are clear. Do not invent results. Match the target journal's abstract headings and word limit.

### Introduction or Background

Use the target journal's exemplar pattern for problem framing, population framing, gap, and objective. Claims about prevalence, burden, or prior work need user-provided citations or placeholders.

### Methods

Methods may be completed from a protocol, search strategy, eligibility criteria, screening plan, data extraction form, appraisal tool, ethics statement, or registration record. Do not invent dates, databases, reviewers, software, tools, checklists, or criteria.

### Results

Results can only be drafted from tables, figures, screening numbers, extracted findings, or author notes. Do not interpret beyond the data. Use placeholders for missing counts, estimates, themes, or subgroup details.

### Discussion

Use author-provided findings as the anchor. Structure usually follows: principal findings, comparison with prior work, interpretation, implications, limitations, and future research. Match the study design: trials may discuss effect evidence, qualitative studies may discuss meanings and context, psychometric studies may discuss validity evidence, and reviews may discuss mapped or synthesized evidence and gaps.

### Limitations

Name limitations supported by the study design and conduct. Do not add generic limitations unless they actually apply.

### Conclusion

Keep conclusions close to the findings and design. For non-causal studies, use cautious language such as `may inform`, `could guide`, or `warrants further evaluation`.

## Workflow

1. Build a compact evidence inventory from the user's materials.
2. Identify the missing section's rhetorical job.
3. Retrieve target journal requirements and full-text exemplar patterns if a target journal is specified.
4. Map evidence to paragraph moves.
5. Draft only supported prose; insert `AUTHOR_INPUT_NEEDED` placeholders where needed.
6. Polish for target-journal structure, causal restraint, inclusive language, sentence variety, and formatting expectations.
7. Output the draft with evidence notes and missing-input notes.

## Output

For missing-section completion, return:

```text
Completed draft
[draft prose]

Evidence used
- [author-provided material used]

Author input needed
- [specific missing item, or None]

Revision notes
- [3-5 concise notes]

Exemplar basis
- [only if full-text exemplar scan was performed]
```

For direct-output requests, keep notes brief and prioritize the completed prose.
