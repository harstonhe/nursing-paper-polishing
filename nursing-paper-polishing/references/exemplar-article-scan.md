# Exemplar Article Scan

Use this reference when the user specifies a target journal and enough article content to identify study design, population, condition, method/intervention/exposure, and outcome. The purpose is to adapt the manuscript to the target journal's published writing logic from accessible full-text articles, not to copy text.

## Trigger

Run this scan when the user provides:

- a target journal, such as `JMIR Aging`, `International Journal of Nursing Studies`, or `Journal of Advanced Nursing`;
- a study design, such as cross-sectional study, scoping review, randomized trial, qualitative study, or mixed-methods study;
- topic details, such as population, disease/condition, intervention/exposure/method, or outcome.

If no target journal is specified, default to IJNS constraints and do not perform a target-journal exemplar scan unless the user asks for one.

## Full-Text Requirement

Use only articles for which the full text, PDF, PMC version, institutional repository copy, author manuscript, or user-provided copy is accessible. For section-specific polishing, the relevant section must be accessible. For example, Methods polishing requires access to the Methods, Eligibility, Inclusion and exclusion criteria, or Study selection text.

Exclude as exemplars:

- abstract-only pages;
- PubMed, Crossref, Scopus, Web of Science, OUCI, ResearchGate, or DOI metadata records without full text;
- paywalled publisher pages when no accessible full text is available;
- article titles found only in reference lists;
- PDF request pages without readable article text.

Metadata-only sources may be used to discover candidate articles or verify citation details, but they cannot be counted among the 2-3 exemplar articles.

When a publisher DOI page is blocked or paywalled, search exact DOI and title variants for accessible full text:

- `"10.xxxx/xxxxx"`;
- `"article title" "PMC"`;
- `"article title" pdf`;
- `site:pmc.ncbi.nlm.nih.gov "article title"`;
- `site:pubmed.ncbi.nlm.nih.gov "article title"` to find PMCID;
- institutional repository or accepted manuscript copies.

If fewer than two full-text exemplars are available after reasonable searching, state this limitation and use only the accessible full-text article(s). Do not fill the exemplar list with abstract-only records.

## Search Priority

Always prioritize the same study design. The minimum acceptable match is:

`same study design + at least one topic component`

Topic components should be ranked:

1. Population and condition, with disease/condition before age group when both are available.
2. Intervention, exposure, technology, method, or phenomenon.
3. Outcome variable.

Example topic:

`cross-sectional study` + `older adults with Alzheimer's disease` + `chatbot` + `depression` + target journal `JMIR Aging`

Search order:

1. Same journal + same design + all available topic components, with full text available.
2. Same journal + same design + condition/population + technology/intervention/method, with full text available.
3. Same journal + same design + condition/population + outcome, with full text available.
4. Same journal + same design + technology/intervention/method + outcome, with full text available.
5. Same journal + same design + condition or population, with full text available.
6. Same journal + same design + technology/intervention/method, with full text available.
7. Same journal + same design + outcome, with full text available.
8. Same journal + same design only, with full text available.
9. Same publisher family + same design + two or more topic components, with full text available.
10. Same publisher family + same design + one topic component, with full text available.
11. Same field + same design + two or more topic components, only if same-journal and same-publisher full-text evidence is insufficient.

Do not choose articles without the same study design unless no design-matched papers can be found. If design-matched articles are unavailable, state the limitation and use the closest available design only for broad journal style, not design-specific reporting.

Do not jump directly to `same journal + same design only` before trying reasonable combinations of topic similarity. For Method, Eligibility, Search strategy, and Study selection polishing, design match remains mandatory, but topic similarity should be maximized first and relaxed stepwise.

## Query Construction

Build several query combinations rather than relying on one search. Include the journal name and method terms first, then add topic terms.

For the example above, use combinations such as:

- `"JMIR Aging" cross-sectional older adults Alzheimer's chatbot depression`
- `"JMIR Aging" cross-sectional dementia chatbot`
- `"JMIR Aging" cross-sectional older adults depression`
- `"JMIR Aging" cross-sectional digital health depression`
- `site:jmir.org "JMIR Aging" "cross-sectional" dementia`
- `site:jmir.org "JMIR Aging" "cross-sectional" chatbot`

Prefer official journal pages, PubMed, Crossref, DOI pages, publisher pages, or article HTML/PDF. Avoid relying on general summaries when article abstracts or full text are available.

For a Journal of Nursing Scholarship scoping review, begin with broad method-first queries such as:

- `"Journal of Nursing Scholarship" "scoping review" "Eligibility criteria"`
- `"Journal of Nursing Scholarship" "scoping review" "Methods"`
- `"Journal of Nursing Scholarship" "scoping review" "study selection"`
- `site:pmc.ncbi.nlm.nih.gov "Journal of Nursing Scholarship" "scoping review"`
- `"Journal of Nursing Scholarship" "scoping review" DOI`

Then add topic terms such as `AI`, `chatbot`, `caregiver`, `dementia`, or `digital health`.

## Article Selection

Select 2-3 full-text exemplar articles.

For each selected article, record:

- title
- journal
- year
- DOI or URL
- full-text access source, such as publisher full text, PMC, institutional repository, accepted manuscript, or user-provided PDF
- study design
- matched components
- sections available for comparison

Prefer articles that share the section being polished. If polishing a Methods paragraph, a full-text Methods section is more useful than an abstract-only match.

## Section-Aware Extraction

Before polishing, identify the manuscript section:

- `Abstract`: compare abstract heading sequence, objective sentence, methods compression, result reporting, conclusion strength, registration wording.
- `Introduction` or `Background`: compare problem opening, population framing, disease/condition framing, gap statement, objective placement.
- `Methods`: compare design declaration, setting, participants, measures, data collection, analysis, ethics, and registration order.
- `Results`: compare descriptive statistics, effect estimates, confidence intervals, p-value restraint, table callouts, and no-overinterpretation.
- `Discussion`: compare principal findings opening, relation to prior work, implications, limitations, and future research.
- `Limitations`: compare specificity, likely direction of bias, and boundary language.
- `Conclusion`: compare restrained implication language and study-design boundaries.
- `Title`, `Keywords`, `Highlights`, `Impact statement`, or `Social media abstract`: compare only target-journal items that the journal actually uses.

Use exemplars to infer:

- paragraph move order;
- sentence types and tense;
- level of methodological detail;
- hedging and causality strength;
- transition density;
- result-reporting compactness;
- section-specific opening and closing patterns.

Do not:

- copy article wording;
- import claims, citations, findings, or limitations from exemplar papers;
- overfit to a single exemplar;
- quote long passages;
- use exemplar text as a substitute for the user's evidence.

## Synthesis for Revision

After scanning, create a brief internal synthesis before rewriting:

1. Target journal section pattern.
2. Design-specific reporting pattern.
3. Content-specific vocabulary and inclusive language.
4. Causality and implication limits.
5. Formatting or article-type requirements.

Then revise the user's text according to the target section.

## Output

When internet search was used, include an `Exemplar basis:` note after the polished text:

- list the 2-3 full-text articles used with DOI/URL and access source when available;
- state which parts informed the revision, such as Abstract structure, Methods sequence, or Discussion implication language;
- state if fewer than two same-journal, design-matched full-text articles were found.

Keep exemplar notes concise. The main deliverable remains the polished manuscript text.
