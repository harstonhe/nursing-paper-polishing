# Medical Review Framework

Use this framework after journal requirements have been collected.

## Universal Medical Manuscript Checks

| Dimension | Review questions |
|---|---|
| Research question | Is the clinical/public health/biomedical question explicit, important, and answerable by the design? |
| Journal fit | Does the topic, method, article type, and implication match the target journal's readership? |
| Novelty | Is the gap real, current, and not just a restatement of common knowledge? |
| Design validity | Can the chosen design answer the question without fatal bias? |
| Population and setting | Are eligibility criteria, recruitment, setting, and representativeness clear? |
| Measures/outcomes | Are primary outcomes, exposures, comparators, endpoints, instruments, and timing defined? |
| Analysis | Are statistics or qualitative analyses appropriate, reproducible, and complete? |
| Results | Are results aligned with prespecified questions and methods, not selectively reported? |
| Interpretation | Do claims stay within the design, sample, uncertainty, and limitations? |
| Ethics and transparency | Are ethics approval, consent, registration, data availability, funding, conflicts, and AI use reported as required? |
| Reporting completeness | Does the paper follow the right reporting guideline and journal checklist? |

## Study-Design-Specific Checks

### Randomized or Interventional Trial

- CONSORT/SPIRIT as applicable; CONSORT-AI/SPIRIT-AI for AI interventions.
- Trial registration, protocol availability, primary outcome, allocation, concealment, blinding, sample size, harms, attrition, intention-to-treat.
- Reject or major-revision risk: no registration when required, unclear primary endpoint, post hoc endpoint switching, serious imbalance without explanation.

### Observational Study

- STROBE alignment.
- Cohort/case-control/cross-sectional design correctly named; exposure/outcome windows clear; confounding strategy justified; missing data handled; sensitivity analyses considered.
- Beware causal language from cross-sectional or uncontrolled retrospective data.

### Diagnostic, Prognostic, or Prediction Model Study

- STARD for diagnostic accuracy; TRIPOD/TRIPOD-AI for prediction models.
- Index test, reference standard, participant flow, calibration/discrimination, internal/external validation, decision thresholds, clinical utility.
- Fatal risks: no independent validation for a model claiming deployment readiness; unclear reference standard; data leakage.

### Systematic Review or Meta-analysis

- PRISMA 2020; protocol registration such as PROSPERO when appropriate.
- Search strategy, databases, date ranges, eligibility, screening process, risk-of-bias tool, synthesis plan, heterogeneity, certainty of evidence.
- Fatal risks: non-reproducible search, no risk-of-bias assessment, narrative claims unsupported by included studies.

### Qualitative or Mixed-Methods Study

- COREQ/SRQR for qualitative components; GRAMMS or journal-specific guidance for mixed methods.
- Sampling rationale, reflexivity, coding process, saturation/information power, triangulation, integration of qualitative and quantitative strands.

### Case Report, Case Series, or Quality Improvement

- CARE for case reports; SQUIRE for quality improvement.
- Patient consent/privacy, timeline, intervention detail, alternative explanations, generalization boundaries.
- Check whether the target journal accepts this article type.

### Digital Health, AI, or Clinical Decision Support

- Match checklist to design: CONSORT-AI, SPIRIT-AI, DECIDE-AI, TRIPOD-AI, STARD-AI where applicable.
- Data provenance, train/validation/test separation, missingness, bias/fairness, external validation, usability, clinical workflow, safety, model availability.
- Watch for leakage, inflated performance, lack of clinically meaningful comparator, and overclaiming real-world effectiveness from development-only studies.

## Severity Guide

- **Critical**: invalidates the main conclusion, violates ethics/transparency requirements, or makes journal fit untenable.
- **Major**: materially weakens credibility but could be fixed with substantial analysis, reporting, or reframing.
- **Minor**: clarity, completeness, formatting, or limited interpretation issue that does not change the main judgment.

## Review Bias Control

- Do not demand a different design merely because it would be ideal; ask whether the chosen design can support the stated claim.
- Do not penalize non-native English more than the science warrants.
- Give credit for strengths, but only when tied to concrete manuscript content.
- State uncertainty when the manuscript lacks enough information to judge.
