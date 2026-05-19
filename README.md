# nursing-paper-polishing

Author / 作者: Harston

`nursing-paper-polishing` is a Codex skill for polishing nursing, midwifery, digital health, health services, and medical manuscripts. Its core feature is **target-journal adaptation through full-text exemplar articles**: when a journal, study design, topic, and manuscript section are provided, the skill searches for 2-3 accessible full-text articles from the target journal with the same method design and the closest possible topic match, then uses their section-level writing logic to polish the user's text.

`nursing-paper-polishing` 是一个面向护理、助产、数字健康、健康服务和医学论文的 Codex skill。它的核心不是普通英文润色，而是 **基于目标期刊全文范文的期刊适应性润色**：当用户提供目标期刊、研究设计、主题和论文结构部分时，skill 会先检索目标期刊中 2-3 篇可获取全文、方法设计一致且主题尽量相近的文章，再根据这些文章对应章节的结构、句型和逻辑来润色用户文本。

## Core Workflow / 核心流程

1. Identify the target journal or publisher.
2. Identify the article type and study design.
3. Identify the manuscript section being polished, such as Abstract, Introduction, Methods, Results, Discussion, Limitations, Conclusion, Highlights, or title.
4. Retrieve or verify the target journal's official author guidelines.
5. Search for 2-3 accessible full-text exemplar articles from the target journal.
6. Prioritize exemplar articles with the same study design and maximum topic similarity.
7. Extract section-specific writing patterns from the exemplars.
8. Polish the user's text while preserving the original meaning, evidence, data, and study boundaries.
9. Apply nursing/medical language standards, including inclusive wording and non-causal language for non-causal designs.
10. Report the exemplar basis and any unresolved journal-formatting uncertainty.

1. 识别目标期刊或出版社。
2. 识别文章类型和研究设计。
3. 识别要润色的论文结构部分，例如 Abstract、Introduction、Methods、Results、Discussion、Limitations、Conclusion、Highlights 或标题。
4. 检索或核对目标期刊官方作者指南。
5. 检索目标期刊中 2-3 篇可获取全文的范文文章。
6. 优先选择同研究设计且主题相似度最高的范文。
7. 提取范文中对应章节的写作结构和逻辑。
8. 在不改变原意、证据、数据和研究边界的前提下润色用户文本。
9. 执行护理/医学英文统一标准，包括包容性表达和非因果研究的谨慎表述。
10. 输出范文依据，并说明仍不确定的期刊格式问题。

## Exemplar Search Rules / 范文检索规则

The skill must use **full-text exemplars only**. Abstract-only pages, PubMed records, Crossref records, DOI metadata pages, indexing pages, or citation database records can help identify candidate articles, but they do not count as exemplar articles.

该 skill 必须使用 **可获取全文的范文**。仅有摘要、PubMed 记录、Crossref 记录、DOI 元数据页、数据库索引页或引文数据库记录只能用于发现候选文献，不能计入范文。

Search priority:

1. Same target journal + same study design + all available topic components + full text.
2. Same target journal + same study design + population/condition + intervention/technology/method + full text.
3. Same target journal + same study design + population/condition + outcome + full text.
4. Same target journal + same study design + intervention/technology/method + outcome + full text.
5. Same target journal + same study design + one topic component + full text.
6. Same target journal + same study design only + full text.
7. Same publisher family + same study design + topic overlap + full text.
8. Same field + same study design + topic overlap + full text, only when target-journal evidence is insufficient.

检索优先级：

1. 同目标期刊 + 同研究设计 + 全部主题组件 + 可获取全文。
2. 同目标期刊 + 同研究设计 + 研究对象/疾病 + 干预/技术/方法 + 可获取全文。
3. 同目标期刊 + 同研究设计 + 研究对象/疾病 + 结局变量 + 可获取全文。
4. 同目标期刊 + 同研究设计 + 干预/技术/方法 + 结局变量 + 可获取全文。
5. 同目标期刊 + 同研究设计 + 任一主题组件 + 可获取全文。
6. 同目标期刊 + 同研究设计 + 可获取全文。
7. 同出版社 + 同研究设计 + 主题部分重合 + 可获取全文。
8. 同领域 + 同研究设计 + 主题部分重合 + 可获取全文，仅在目标期刊证据不足时使用。

For example, if the target is `JMIR Aging` and the study is a cross-sectional study on chatbot use for depression among older adults with Alzheimer's disease, the search should first prioritize:

`JMIR Aging + cross-sectional study + Alzheimer's disease/dementia + older adults + chatbot + depression + full text`

Then reduce topic similarity step by step. The weakest same-journal fallback is:

`JMIR Aging + cross-sectional study + full text`

例如，如果目标期刊是 `JMIR Aging`，研究是关于阿尔茨海默病老年人使用 chatbot 治疗或支持抑郁的横断面研究，应优先检索：

`JMIR Aging + cross-sectional study + Alzheimer's disease/dementia + older adults + chatbot + depression + full text`

如果没有，再逐步减少主题相似度。最弱的同刊兜底选择是：

`JMIR Aging + cross-sectional study + full text`

## Section-Aware Polishing / 分章节润色

The skill adapts only the section-relevant logic from exemplar articles:

- Abstract: heading order, objective sentence, methods compression, result reporting, and conclusion strength.
- Introduction/Background: problem opening, population framing, gap statement, and objective placement.
- Methods: design declaration, eligibility criteria, search strategy, screening, extraction, appraisal, ethics, and registration.
- Results: study selection, descriptive reporting, tables, effect estimates, confidence intervals, and no overinterpretation.
- Discussion: principal findings, relation to prior work, implications, limitations, and future research.
- Conclusion: restrained implication language and study-design boundaries.

skill 只借鉴范文中对应章节的写作逻辑：

- Abstract：标题顺序、目标句、方法压缩方式、结果报告和结论强度。
- Introduction/Background：问题引入、研究对象框定、研究空白和目标位置。
- Methods：设计声明、Eligibility、检索策略、筛选、资料提取、质量评价、伦理和注册。
- Results：文献筛选结果、描述性报告、表格引用、效应量/置信区间和避免过度解释。
- Discussion：主要发现、与既有研究关系、意义、局限和未来研究。
- Conclusion：克制的实践意义和研究设计边界。

The skill must not copy exemplar wording, import exemplar claims, or overfit to one article.

skill 不应复制范文原句，不应引入范文中的结论或数据，也不应过度模仿单篇文章。

## Language Guardrails / 语言约束

Across all target journals, the skill applies a consistent nursing and medical English standard:

- Preserve the author's meaning, data, citations, and study boundaries.
- Do not invent evidence, mechanisms, references, novelty claims, or clinical implications.
- Avoid causal language in non-causal designs such as scoping reviews, cross-sectional studies, qualitative studies, psychometric studies, and descriptive reviews.
- Replace unsupported causal verbs such as `enhance`, `improve`, `reduce`, `lead to`, `result in`, and `impact` with cautious alternatives such as `may inform`, `could support`, `has the potential to`, `is associated with`, or `may provide a basis for`.
- Use inclusive medical language, such as `older adults` instead of `elderly`, `people with dementia` instead of `demented patients`, and `people with disabilities` instead of `the disabled`.
- Avoid repeatedly using the same transition or sentence frame more than twice in nearby paragraphs.
- Avoid frequent em dashes and overly mechanical parallel sentences.

所有目标期刊均执行统一的护理/医学英文标准：

- 保留作者原意、数据、引用和研究边界。
- 不编造证据、机制、参考文献、创新性或临床意义。
- 非因果研究避免因果化表达，例如 scoping review、横断面研究、质性研究、量表研究和描述性综述。
- 将缺乏因果依据的 `enhance`、`improve`、`reduce`、`lead to`、`result in`、`impact` 等词改为 `may inform`、`could support`、`has the potential to`、`is associated with` 或 `may provide a basis for` 等谨慎表达。
- 使用包容性医学表达，例如用 `older adults` 替代 `elderly`，用 `people with dementia` 替代 `demented patients`，用 `people with disabilities` 替代 `the disabled`。
- 避免相邻段落中同一连接词或句式重复超过两次。
- 避免频繁使用破折号和过于机械的排比句。

## Journal Defaults / 期刊默认规则

- If a target journal is specified, use that journal's current official author guidelines.
- If the journal belongs to Wiley, Elsevier, JMIR, Sage, Springer Nature, or another publisher, do not rely on publisher-level rules alone; verify the specific journal.
- `Journal of Advanced Nursing` is a specific Wiley journal, not a publisher category.
- If no target journal is specified, default to IJNS-style nursing SCI rigor.
- Do not apply IJNS highlights to JMIR or Wiley journals unless the target journal explicitly requires them.
- Do not apply JMIR/AMA style to IJNS unless requested by the target journal.

- 如果指定了目标期刊，优先使用该期刊最新官方作者指南。
- 如果期刊属于 Wiley、Elsevier、JMIR、Sage、Springer Nature 或其他出版社，不应只使用出版社通用规则，而要核对具体期刊。
- `Journal of Advanced Nursing` 是 Wiley 旗下具体期刊，不是出版社类别。
- 如果没有指定目标期刊，默认使用 IJNS 风格和护理 SCI 严谨性要求。
- 不要把 IJNS highlights 套用到 JMIR 或 Wiley 期刊，除非目标期刊明确要求。
- 不要把 JMIR/AMA 格式套用到 IJNS，除非目标期刊要求。

## Expected Output / 输出格式

Default output:

1. Polished text.
2. Revision notes.
3. Causality check.
4. Exemplar basis, if a full-text exemplar scan was performed.
5. Formatting check, if manuscript formatting was requested.

默认输出：

1. 润色后的文本。
2. 修改说明。
3. 因果表达检查。
4. 如果进行了全文范文检索，列出范文依据。
5. 如果用户要求格式检查，列出格式检查结果。

## Example Prompts / 示例提示词

```text
Use nursing-paper-polishing to polish the Eligibility section for Journal of Nursing Scholarship. The manuscript is a scoping review on AI chatbots among informal caregivers of people with dementia.
```

```text
请调用 nursing-paper-polishing。目标期刊是 Journal of Nursing Scholarship，文章是关于 AI-chatbots 在痴呆症照护者中的使用情况的 scoping review。请润色 Methods 里的 Eligibility。
```

```text
Use nursing-paper-polishing to revise this Abstract for JMIR Aging. This is a cross-sectional study about chatbot use for depression among older adults with Alzheimer's disease.
```

```text
请用 nursing-paper-polishing 检查这份 .docx 是否符合 Wiley 旗下 Journal of Advanced Nursing 的投稿格式，并指出需要按作者指南核实的项目。
```
