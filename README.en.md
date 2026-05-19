<p align="right">
  <a href="README.md">中文</a> | <strong>English</strong>
</p>

# nursing-paper-polishing

Author: Harston

<p align="center">
  <img src="nursing-paper-polishing/assets/huyan-zhaji-qrcode.png" alt="Huyan Zhaji WeChat official account QR code" width="260">
</p>

> Search **护研札记** on WeChat official accounts (`wx`) for free updates on nursing research. We also provide 1-on-1 guidance on topic selection, statistics, polishing, and journal submission. The team includes multiple nursing PhDs from 985 universities and has published several Q1 and top-journal papers.

A Codex skill for nursing and medical manuscript polishing, journal adaptation, and evidence-constrained section completion.

Its core workflow is not generic editing. It adapts writing to a target journal by checking the journal guidelines and learning section-level writing patterns from 2-3 accessible full-text exemplar articles with the same study design and closest topic match.

## What It Does

- Polishes abstracts, introductions, methods, results, discussions, conclusions, titles, and highlights.
- Adapts manuscripts to target journals such as IJNS, JMIR journals, Elsevier journals, and Wiley journals.
- Searches full-text exemplar articles before journal-specific rewriting.
- Completes missing paragraphs or sections from user-provided notes, tables, figures, results, protocols, or partial drafts.
- Applies nursing and medical language guardrails, including non-causal wording for non-causal designs and inclusive terminology such as `older adults`.

## Core Workflow

1. Identify the target journal, article type, study design, topic, and manuscript section.
2. Check the target journal's current author guidelines.
3. Find 2-3 accessible full-text exemplar articles, prioritizing the same study design and highest topic similarity.
4. Extract section-specific patterns from those exemplars.
5. Polish or complete the user's text without inventing evidence.
6. Apply causality, inclusive-language, formatting, and target-journal checks.

## Exemplar Search Rule

Use full-text exemplars only. Abstract pages, PubMed records, Crossref records, DOI metadata pages, and indexing pages may identify candidates, but they do not count as exemplars.

Priority:

1. Same journal + same design + strongest topic match + full text.
2. Same journal + same design + partial topic match + full text.
3. Same journal + same design only + full text.
4. Same publisher or field + same design + topic overlap + full text, only if same-journal evidence is insufficient.

## Missing Section Completion

The skill can draft missing sections from partial materials, but the user's evidence is the ceiling for every claim.

If essential information is missing, it marks:

```text
AUTHOR_INPUT_NEEDED: [specific missing item]
```

It must not invent findings, sample sizes, eligibility criteria, search dates, databases, ethics details, registration numbers, citations, or implications.

## Example Prompts

```text
Use nursing-paper-polishing to polish the Eligibility section for a target nursing journal. The manuscript is a nursing-related scoping review.
```

```text
Use nursing-paper-polishing to complete the missing Discussion paragraph for IJNS using these results and Table 2.
```

```text
Use nursing-paper-polishing to revise this Abstract for JMIR Aging. This is a cross-sectional study about chatbot use for depression among older adults with Alzheimer's disease.
```

## Output

Typical output includes:

- Polished or completed text
- Revision notes
- Causality check
- Exemplar basis, when full-text exemplar scanning was used
- Evidence used and author input needed, when completing missing content
- Formatting check, when requested
