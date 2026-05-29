# Reference Validation

Use this reference after manuscript adaptation and before final delivery.

## Source Priority

| Priority | Source | Use for |
|---:|---|---|
| 1 | Target journal author guidelines | Required reference style, citation rules, DOI policy |
| 2 | Publisher style guide linked by the journal | Detailed formatting rules |
| 3 | APA style | Fallback when journal guidance is unavailable, unclear, or silent |
| 4 | CrossRef or DOI metadata | Verify DOI, title, journal, year, volume, issue, pages, article number |
| 5 | PubMed or publisher page | Biomedical metadata verification when DOI metadata is incomplete |

Do not invent missing bibliographic fields. Mark uncertainty instead.

## Validation Checklist

Check each reference for:

| Field | Check |
|---|---|
| Authors | Surname and initials, order, spelling, group authors, use of ampersand or "and" according to style |
| Year | Year is present and matches DOI/publisher metadata |
| Title | Article title is present, capitalization follows journal style or APA fallback, no encoding artifacts |
| Source | Journal title or proceedings/book title is complete and formatted consistently |
| Volume/issue/pages | Present when available; article numbers are not mistaken for page ranges |
| DOI/URL | DOI is formatted consistently and resolves or appears in DOI metadata |
| Record type | Journal article, preprint, conference paper, report, software, guideline, or web source is formatted appropriately |
| Duplicates | Same DOI, title, or article appears more than once |
| In-text consistency | Key cited studies in the manuscript appear in References and obvious uncited duplicates are flagged |

## APA Fallback Rules

When the journal does not specify a reference style, apply APA-like consistency:

- Author, A. A., Author, B. B., & Author, C. C. (Year). Article title in sentence case. *Journal Title*, *volume*(issue), page range or article number. https://doi.org/xxxxx
- Use sentence case for article titles.
- Use title case for journal titles.
- Include DOI as a URL when available.
- Do not add periods after DOI URLs.
- Keep article numbers when no page range exists.

## CrossRef Verification

When possible, verify each DOI or likely DOI with CrossRef:

| Status | Meaning |
|---|---|
| `verified` | DOI exists and title, journal, and year substantially match |
| `partial` | DOI exists but one field is missing, access is limited, or online-first year differs |
| `unverified` | DOI does not resolve, title/journal/year conflicts, or no reliable metadata found |

Use CrossRef verification to identify errors, not to overwrite author-supplied citations without checking the manuscript context.

## Marker Rules

If a reference has an error or uncertainty, append a compact marker at the end of that reference entry:

```text
[REF-CHECK: issue]
```

Use one or more semicolon-separated issues when needed:

```text
[REF-CHECK: DOI not verified; possible duplicate]
```

Common markers:

| Marker | Use when |
|---|---|
| `[REF-CHECK: DOI not verified]` | DOI is absent, malformed, or not found in DOI metadata |
| `[REF-CHECK: title/year differs from DOI metadata]` | DOI metadata conflicts with the written reference |
| `[REF-CHECK: journal differs from DOI metadata]` | Container title does not match the written journal |
| `[REF-CHECK: missing volume/issue/pages]` | Required bibliographic fields appear incomplete |
| `[REF-CHECK: possible duplicate]` | Same DOI/title appears more than once |
| `[REF-CHECK: encoding problem in author names]` | Names or titles contain corrupted characters |
| `[REF-CHECK: incomplete conference/preprint details]` | Non-journal item lacks venue, date, preprint server, or stable URL |
| `[REF-CHECK: APA formatting needs manual confirmation]` | Fallback formatting was applied but metadata remains uncertain |

Do not mark every stylistic difference if the reference is already consistent with the target journal style. Reserve markers for items the author should inspect before submission.

## Output Summary

After validating references, include a concise report:

```text
Reference validation
| Reference | Status | Marker added |
|---|---|---|
| Author year short title | verified / partial / unverified | [REF-CHECK: ...] or None |
```

