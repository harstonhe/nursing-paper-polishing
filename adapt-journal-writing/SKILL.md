---
name: adapt-journal-writing
description: Adapt manuscript writing, rewriting, polishing, reference formatting, or section planning to a specific target journal by first identifying the journal, searching current author guidelines and submission requirements, finding public exemplar articles of the same article type or method in that journal, verifying the selected exemplars through CrossRef or DOI metadata, extracting journal-specific writing logic, structure, formatting expectations, validating references against the journal style or APA fallback, and then applying nature-writing-style claim-evidence-boundary revision. Use when the user gives or asks for a target journal, journal-specific manuscript adaptation, author instructions, "按照目标期刊改写", "投稿期刊适配", "参考文献格式检查", "scoping review 写作逻辑", "根据某杂志已发表文章润色", or wants to rewrite an abstract, introduction, methods, results, discussion, title, references, cover-facing summary, or manuscript section for a named journal.
---

# Adapt Journal Writing

Use this skill to adapt scientific manuscript prose to a named target journal rather than applying a generic Nature-style rewrite.

The skill has four layers:

1. target journal requirements
2. same-journal exemplar articles
3. article-type or method conventions
4. reference-format validation
5. `nature-writing` style claim-evidence-boundary revision

The key behavior is: **research before rewriting**. Do not polish toward a journal until the current author instructions and suitable exemplar articles have been checked.

## Default Stance

- Treat journal adaptation as an evidence-grounded writing task, not a style imitation task.
- Use official journal pages first for requirements and article-type definitions.
- Use public, citable articles from the same journal as exemplars for writing logic, organization, headings, abstract structure, reporting depth, and tone.
- Prefer 2-3 highly relevant exemplars over many weak matches.
- Verify selected exemplar articles through CrossRef or DOI metadata before learning from them. If an article cannot be verified as real and accessible, replace it or label it as unverified and exclude it from pattern learning.
- Do not copy wording, sentences, paragraph templates, figures, titles, or unique phrasing from exemplar papers.
- Do not invent journal rules, word limits, article types, reporting checklist requirements, fees, or formatting constraints.
- If the target journal's policies may have changed, verify the current journal page before finalizing advice.
- Keep the author's actual evidence as the ceiling for every claim. If the evidence is missing, write a placeholder or flag `AUTHOR_INPUT_NEEDED`.
- Validate the reference list against the target journal's author guidelines. If no reference style is specified or the guideline is unavailable, use APA style as the fallback standard.
- If a reference has a formatting error, missing field, questionable DOI, unresolved metadata, duplicate record, or other uncertainty, mark it at the end of that reference entry instead of silently fixing or deleting it.

## Inputs To Collect

Before rewriting, identify or ask for the missing minimum inputs:

| Input | Required? | Notes |
|---|---:|---|
| Target journal name | Yes | Use the exact journal title when possible. |
| Manuscript type | Yes | Example: scoping review, systematic review, original article, methods paper, protocol, brief report. |
| Section to revise | Yes | Abstract, Introduction, Methods, Results, Discussion, title, full outline, or full manuscript. |
| Draft text or author notes | Yes | If absent, produce a structure or writing plan rather than final prose. |
| Field/topic | Strongly recommended | Needed to find same-journal exemplars. |
| Target constraints | Optional | Word limit, article type, reporting checklist, tables/figures, reference style. |

If the user only provides a journal and a broad intention, return a journal-adaptation plan and ask for the draft section before rewriting.

## Workflow

### 1. Resolve the Target Journal

Confirm the journal identity before searching deeply:

- official journal title
- publisher or society
- ISSN or homepage if ambiguity exists
- article type relevant to the user's manuscript

If multiple journals share similar names, ask a concise clarification question or state the assumption before proceeding.

### 2. Search Current Author Guidelines

Search the web for official sources. Prioritize:

1. journal "Instructions for Authors" or "Guide for Authors"
2. article type descriptions
3. editorial policies and reporting guidelines
4. submission system requirements
5. publisher-level policies only when journal-specific pages are silent

Extract only the requirements that affect writing:

- article type fit
- abstract format and word count
- main text word count
- required headings
- methods/reporting checklist requirements
- data/code availability requirements
- ethics/registration requirements
- tables/figures/supplement rules that affect prose
- reference style, DOI policy, citation style, and reference-list requirements

Use `references/journal-requirements.md` when turning sources into a requirements matrix.

### 3. Find Same-Journal Exemplar Articles

Search public articles in the target journal using the user's article type and topic.

For example, if the manuscript is a scoping review:

- search the target journal for `"scoping review"`
- add topic terms when needed
- prefer recent articles from the last 3-5 years unless the journal has few examples
- keep 2-3 articles that are article-type matches and preferably topic-adjacent

### 3b. Verify Exemplar Articles With CrossRef

Before learning writing patterns from the selected 2-3 exemplar articles, verify each article through CrossRef or DOI metadata.

For each candidate, check:

- DOI exists and resolves through CrossRef or official DOI metadata
- title substantially matches the candidate article
- journal/container title matches the target journal or an accepted journal-title variant
- publication year matches or is within one year of the candidate record
- article URL, DOI landing page, abstract page, or full text is accessible enough to inspect structure

Use this decision rule:

| Verification status | Rule |
|---|---|
| `verified` | DOI/title/journal/year match and a landing page or abstract/full text is accessible. Use as an exemplar. |
| `partial` | DOI metadata exists but one non-critical field differs, or access is limited. Use only with a note and prefer replacing it if better candidates exist. |
| `unverified` | No CrossRef/DOI match, wrong journal, wrong title, fabricated-looking record, or inaccessible source. Do not use for pattern learning. |

If fewer than two exemplars pass verification, broaden the search by topic, date range, or article-type synonyms. If still fewer than two pass, continue only with a clearly labeled limited-exemplar profile.

For each exemplar, capture:

- title, year, DOI or URL
- CrossRef or DOI verification status
- article type
- abstract structure
- section heading pattern
- Introduction logic
- Methods reporting depth
- Results organization
- Discussion and limitations pattern
- tone and claim strength

Use `references/exemplar-learning.md` for the extraction checklist.

### 4. Build A Journal Adaptation Profile

Create a compact profile before rewriting:

| Dimension | Journal-specific observation | Implication for this manuscript |
|---|---|---|
| Article type |  |  |
| Abstract |  |  |
| Section structure |  |  |
| Methods/reporting |  |  |
| Claim strength |  |  |
| Discussion style |  |  |
| Required statements |  |  |

If journal requirements conflict with exemplar habits, follow the official journal requirements and note the conflict.

### 5. Apply Nature-Writing Logic

After the journal profile is built, use the core `nature-writing` logic:

1. Build a one-sentence argument: `In [system/problem], we show [advance] using [approach], supported by [evidence], with [boundary].`
2. Map each paragraph to one job: context, gap, approach, result, comparison, implication, limitation, or reporting detail.
3. Keep claims near the evidence that supports them.
4. Calibrate verbs: `show`, `demonstrate`, `suggest`, `indicate`, `may`, `could`, `is associated with`, `maps`, `summarizes`.
5. Remove unsupported novelty, causality, certainty, and universal claims.
6. Adapt structure, headings, and emphasis to the target journal profile.

For scoping reviews, default to:

- map the evidence landscape, not prove intervention efficacy
- state eligibility, sources, charting process, synthesis approach, and reporting checklist
- avoid causal or clinical recommendation claims unless the review design supports them
- separate `what was mapped`, `what patterns emerged`, and `what gaps remain`

Use `references/writing-adaptation.md` for article-type adaptation patterns.

### 6. Validate Reference Style And Metadata

Before finalizing a manuscript or DOCX, inspect the References section.

Use the target journal's author guidelines first. If the journal gives a reference style, follow it. If the guideline is unavailable, unclear, or silent about reference style, use APA as the fallback standard.

Check each reference for:

- author order and initials
- publication year placement
- article title capitalization
- journal title formatting
- volume, issue, page range, and article number
- DOI or stable URL formatting
- duplicate entries
- obvious encoding problems
- mismatch between DOI metadata and the written reference
- incomplete, preprint, conference, or in-press records needing author confirmation

When CrossRef or DOI metadata is available, use it to verify DOI, title, journal/container title, and publication year. Do not invent missing fields.

If a reference is wrong or uncertain, append a compact marker at the end of that same reference entry:

```text
[REF-CHECK: issue]
```

Examples:

- `[REF-CHECK: DOI not verified]`
- `[REF-CHECK: possible duplicate]`
- `[REF-CHECK: missing volume/issue/pages]`
- `[REF-CHECK: title/year differs from DOI metadata]`
- `[REF-CHECK: encoding problem in author names]`
- `[REF-CHECK: APA formatting needs manual confirmation]`

Use `references/reference-validation.md` for the detailed checklist and marker rules.

### 7. Apply Formatting And Final QA

When producing a manuscript-ready DOCX or revised manuscript section, apply the target journal's explicit formatting rules first. If the journal is silent and the user gives formatting instructions, follow the user. If neither is available, use these submission-ready defaults:

- use `Times New Roman` throughout the manuscript, including body text, headings, references, tables, figure captions, and notes
- use body text size 12 pt (Chinese xiaosi / small-four body size) for main text, abstract, references, table notes, and figure captions
- use major heading size 14 pt (Chinese sihao / fourth-size heading) for main section headings such as Introduction, Methods, Results, Discussion, Limitations, Conclusion, and References
- bold all main section headings; use 12 pt bold for subheadings unless the target journal specifies otherwise
- use double line spacing by default for journal submission manuscripts, unless the journal or user requests 1.5 spacing or another setting
- separate paragraphs clearly; do not output dense, unbroken blocks of text
- use justified body text, first-line paragraph indentation, single-column layout, editable Word-compatible text, and standard 1-inch / 2.54 cm margins unless instructed otherwise
- keep table titles above tables and figure captions below figures unless the journal specifies otherwise
- keep references in the same font, size, and line spacing as the body text unless the journal specifies otherwise

Before final delivery, scan the entire output, including DOCX XML/text, Markdown, references, tables, captions, and exported reference files, for text-corruption artifacts. Fix broken accented names such as `P?rez-Esteve`, broken apostrophes such as `one?s` or `author?s`, Unicode replacement characters such as `U+FFFD`, garbled symbols, corrupted non-English names or journal titles, broken hyphens/dashes/minus signs, and question marks that are not real punctuation.

Run a final QA pass before telling the user the work is complete:

1. Formatting QA: verify the required font, size, line spacing, headings, margins, paragraphing, and table/figure caption placement were actually written into the file.
2. Citation/reference QA: check every in-text citation has a matching reference entry, every reference is cited unless intentionally supplementary, and DOI/PMID/PMCID/publisher metadata are verified when available.
3. Encoding QA: confirm no suspicious question marks, `U+FFFD`, broken apostrophes, or corrupted author/place/journal names remain.
4. Claim-evidence-boundary QA: confirm the writing respects article type, study design, author results, and verified sources without overclaiming.
5. File integrity QA: verify DOCX package validity or structural opening, and export `.ris`, `.nbib`, or another importable format when the user requests EndNote compatibility.

### 8. Produce The Adapted Output

Unless the user asks for a different format, return:

```text
Journal adaptation evidence
| Source | What was checked | Verification | Key writing implication |
|---|---|---|---|

Journal writing profile
| Dimension | Observation | How I applied it |
|---|---|---|

Adapted draft
[rewritten prose]

Revision notes
- [3-6 concise notes]

Reference validation
| Reference | Status | Marker added |
|---|---|---|

Formatting and final QA
- [font, line spacing, headings, paragraphing, encoding scan, citation/reference consistency, file integrity, and EndNote export status when relevant]

Author input needed
- [only real missing fields, or "None"]
```

For long manuscripts, revise section by section. Do not attempt a whole-manuscript rewrite if the source text is too long to verify and adapt reliably in one pass.

## Source And Citation Rules

- Provide links to the official author guidelines and exemplar articles used.
- Distinguish official requirements from inferred exemplar patterns.
- When using exemplar articles, paraphrase structural observations only.
- Do not quote large portions of publisher text or published papers.
- If web access is unavailable, produce a provisional adaptation checklist and clearly mark it as not journal-verified.

## Related Files

| File | Open when |
|---|---|
| [references/journal-requirements.md](references/journal-requirements.md) | Converting author guidelines into a writing-relevant requirements matrix |
| [references/exemplar-learning.md](references/exemplar-learning.md) | Extracting reusable structure and logic from same-journal public articles |
| [references/writing-adaptation.md](references/writing-adaptation.md) | Applying article-type-specific adaptation, especially scoping reviews and reviews |
| [references/reference-validation.md](references/reference-validation.md) | Checking and marking reference-list format, DOI metadata, APA fallback, duplicates, and uncertain records |
