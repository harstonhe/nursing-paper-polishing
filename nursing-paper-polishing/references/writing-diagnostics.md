# Writing Diagnostics

Use this file before substantial polishing, reviewer-comment revision, paragraph rebuilding, or full-section rewriting. The goal is to diagnose the writing problem before improving the English.

## Core Rule

Do not polish sentences while leaving the reasoning broken. A paragraph that sounds fluent but performs the wrong rhetorical job is still a failed revision.

## Failure-Mode Diagnosis

Identify the main problem before editing:

- `wrong paper-type logic`: the section uses a logic that does not fit the study design or article type;
- `wrong section job`: the paragraph belongs in another section, such as interpretation in Results or new evidence in Conclusion;
- `missing gap or positioning`: the Background or Introduction does not explain what remains uncertain and why it matters;
- `claim without evidence`: an assertion is not supported by data, a method detail, a table, a figure, a participant quote, or a verified source;
- `evidence without a claim`: data are listed but the reader is not told what point they support;
- `missing boundary`: the implication exceeds the design, sample, setting, evidence type, or journal/reviewer constraint;
- `Results and Discussion mixed`: observations, interpretation, and implications are not separated;
- `citation-positioning problem`: prior work is misrepresented, uncited, over-flattened, or used to manufacture novelty;
- `sentence-level clutter only`: the logic is sound, but grammar, transitions, concision, or mechanics need repair.

Prioritize fixes in this order:

`paper type -> section job -> paragraph logic -> claim/evidence/boundary -> citation positioning -> sentence polish`

## Claim-Evidence-Boundary

Every important scientific statement should have three components.

### Claim

Ask:

- What exactly is being said?
- Is it descriptive, comparative, interpretive, causal, methodological, clinical, or policy-facing?
- Does the sentence use a verb that is stronger than the design can support?

### Evidence

Ask:

- Which result, table, figure, statistic, quote, coding output, protocol item, appraisal result, or verified citation supports the claim?
- Is the evidence from the user's manuscript, the user's notes, or a full-text exemplar used only for structure?
- Does the claim need a citation, a data value, a table reference, or `AUTHOR_INPUT_NEEDED`?

### Boundary

Ask:

- What population, setting, method, sample, follow-up period, measurement, language, country, or evidence type limits the claim?
- Is the manuscript a causal design, non-causal design, review, validation study, qualitative study, or exploratory study?
- Should the sentence use `may`, `could`, `appears to`, `was associated with`, `mapped`, `identified`, `described`, or `warrants further evaluation`?

## Common Repairs

- Claim too broad: narrow it by population, setting, time, method, or evidence type.
- Causal verb in non-causal work: replace with descriptive or cautious wording.
- Missing evidence: insert `AUTHOR_INPUT_NEEDED: [specific evidence]`.
- Unclear contribution: state what uncertainty was reduced, not that the study is simply important.
- Overlong paragraph: split by controlling idea.
- Repetitive transition chain: remove decorative transitions and rely on thematic linking.

## Design-Aware Examples

- Randomized trials may support intervention effects when allocation, measurement, attrition, and analysis are adequate.
- Quasi-experimental studies require careful wording about design assumptions and residual confounding.
- Cross-sectional studies describe prevalence, distributions, associations, or perceptions, not change over time.
- Qualitative studies describe experiences, meanings, processes, and contexts, not frequencies as population estimates.
- Psychometric studies support claims about reliability, validity evidence, measurement structure, and intended use, not clinical effectiveness.
- Scoping reviews map evidence and identify gaps, not pooled effects or intervention effectiveness unless explicitly supported.
- Systematic reviews synthesize evidence according to the included study designs and certainty of evidence.

## Output Use

When the user asks for direct polishing, silently apply this diagnostic process. When the section is underdeveloped, briefly report the diagnosis before the polished text unless the user asks for output only.
