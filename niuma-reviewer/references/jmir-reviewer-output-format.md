# JMIR Reviewer Output Format

Use this format when the target journal is JMIR or when the user asks for reviewer-style comments based on the JMIR peer-review form. This reference was derived from the user's JMIR reviewer template file.

## Output Contract

Produce review comments in this order:

1. `II.1. Confidential comments for editors`
2. `II.2. Potential conflicts of interest`
3. `II.3. Use of generative artificial intelligence tools in preparing this peer review`
4. `II.4. Parts of the manuscript outside reviewer expertise / suggested external reviewers`
5. `II.5. Interest in writing an editorial or commentary`
6. `General comments`
7. `Specific comments`
8. `Major comments`
9. `Minor comments`

Keep the JMIR section headings in English unless the user explicitly asks for Chinese-only output. The explanatory text under each heading may be in the user's language.

## Section Requirements

### II.1. Confidential comments for editors

Give the editor a direct, candid assessment that is not intended for authors. Address whether the manuscript meets JMIR acceptance criteria:

- ethical conduct
- originality
- adequate discussion and citation of prior/related work
- clear writing
- appropriate study methods
- valid data
- conclusions that are reasonable and supported by the data
- importance of the information
- interest and fit for JMIR readership

Include an explicit editorial recommendation such as `Reject`, `Major Revision`, `Minor Revision`, `Proceed to External Review`, or `Likely Suitable After Pre-submission Revision`.

### II.2. Potential conflicts of interest

State whether any potential conflicts of interest are known. If none are known from the reviewer's perspective, write a concise declaration such as: `No known conflicts of interest.`

### II.3. Use of generative artificial intelligence tools

Disclose AI use in preparing the review. When Codex generates the review, state that generative AI assistance was used to structure and draft the review, and that conclusions are based on the provided manuscript and verified journal requirements. Do not falsely claim no AI was used.

### II.4. Parts outside expertise / suggested external reviewers

State any areas that require specialist review. Examples:

- advanced statistics or psychometrics
- clinical nursing domain expertise
- AI/LLM benchmarking and reproducibility
- ethics, privacy, or data governance
- English language editing

Suggest reviewer expertise types, not real named reviewers, unless the user explicitly asks for names and has provided a safe source.

### II.5. Interest in writing an editorial or commentary

State whether an editorial/commentary would be appropriate and outline a possible angle only if useful. Otherwise write `Not applicable` or `No`.

### General comments

Summarize the manuscript in 1 short paragraph, then give the overall assessment. Mention the core contribution, fit with JMIR, and the main reason for the recommendation.

### Specific comments

Give section-by-section comments in manuscript order: Title/Abstract, Introduction, Methods, Results, Discussion/Conclusion, References/Statements/Supplementary Materials. Keep comments specific and grounded in manuscript content.

### Major comments

Numbered items. Each major comment must include:

- manuscript location
- problem
- why it matters for JMIR review
- required revision or evidence needed

Use major comments for issues affecting validity, transparency, reproducibility, ethics, journal fit, interpretation, or editorial decision.

### Minor comments

Continue numbering after major comments if following the JMIR template style, or restart at 1 if the user prefers. Use minor comments for wording, formatting, citation style, table/figure clarity, grammar, and small reporting improvements.

## Tone and Detail

- Be direct but constructive.
- Do not overpraise.
- Do not rewrite the manuscript inside the review unless asked.
- Do not include a long separate scoring table unless the user requests scores.
- If a finding is based on a journal rule, cite the source URL in the comment.
