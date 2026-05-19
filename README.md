# nursing-paper-polishing 使用指南 / User Guide

Author / 作者: Harston

## 中文说明

`nursing-paper-polishing` 是一个面向护理、助产、数字健康、健康服务和医学论文的 Codex skill，用于根据目标期刊或出版社要求进行英文润色、结构调整、格式检查和投稿前语言风险审查。它保留 IJNS 作为内置 profile，但不再局限于 IJNS。

### 适用场景

- 润色护理 SCI 论文的摘要、引言、方法、结果、讨论、结论、标题或 highlights。
- 根据目标期刊适配稿件，例如 IJNS、JMIR、Elsevier 旗下期刊、Wiley 旗下期刊、Journal of Advanced Nursing 等。
- 检查非因果研究中的因果化表达，避免不恰当地使用 `enhance`、`improve`、`reduce`、`lead to` 等词。
- 检查医学与护理领域包容性表达，例如将 `elderly` 改为 `older adults`。
- 检查 Word 文档格式、表格、图题、图中文字、字体、字号、行距和编号一致性。

### 推荐使用方式

把目标期刊、稿件类型和研究设计告诉 Codex。例如：

```text
Use nursing-paper-polishing to polish this abstract for JMIR. This is a cross-sectional survey of nursing students.
```

```text
请用 nursing-paper-polishing 润色这段 Discussion，目标期刊是 International Journal of Nursing Studies，研究设计是 scoping review。
```

```text
请用 nursing-paper-polishing 检查这份 .docx 是否符合 Wiley 旗下 Journal of Advanced Nursing 的投稿格式。
```

### 工作逻辑

1. 先识别目标期刊或出版社。
2. 再识别文章类型和研究设计。
3. 查询或读取对应作者指南。
4. 按研究设计约束语言强度，尤其避免非因果研究写成因果结论。
5. 按目标期刊处理摘要结构、标题、关键词、highlights、impact statement、reference style、表图格式和匿名审稿要求。
6. 最后执行统一的护理/医学英文语言标准。

### 重要原则

- 不把 IJNS 的格式套用到 JMIR、Wiley 或其他期刊。
- 不把出版社级别规则当作具体期刊规则。
- Journal of Advanced Nursing 是 Wiley 旗下的一个具体期刊，应按它自己的 Author Guidelines 处理。
- 如果没有目标期刊，默认使用通用护理 SCI 英文标准。
- 如果需要最终投稿格式，最好上传目标期刊的 author guidelines 或 manuscript template。

## English Guide

`nursing-paper-polishing` is a Codex skill for polishing nursing, midwifery, digital health, health services, and medical manuscripts. It adapts English style, structure, formatting, and submission checks to the target journal or publisher. IJNS is retained as a built-in profile, but the skill is not limited to IJNS.

### Use Cases

- Polish abstracts, introductions, methods, results, discussions, conclusions, titles, or highlights for nursing SCI manuscripts.
- Adapt manuscripts for a target journal, such as IJNS, JMIR, Elsevier journals, Wiley journals, or Journal of Advanced Nursing.
- Check causal overclaiming in non-causal studies and revise verbs such as `enhance`, `improve`, `reduce`, or `lead to`.
- Apply inclusive medical and nursing language, such as replacing `elderly` with `older adults`.
- Audit Word formatting, tables, figure captions, figure text, fonts, sizes, line spacing, and numbering consistency.

### Recommended Prompts

```text
Use nursing-paper-polishing to polish this abstract for JMIR. This is a cross-sectional survey of nursing students.
```

```text
Use nursing-paper-polishing to revise this Discussion for International Journal of Nursing Studies. The study is a scoping review.
```

```text
Use nursing-paper-polishing to check whether this .docx follows the author guidelines for Journal of Advanced Nursing, a Wiley journal.
```

### Workflow

1. Identify the target journal or publisher.
2. Identify the article type and study design.
3. Read or retrieve the relevant author guidelines.
4. Match language strength to the study design, especially for non-causal evidence.
5. Adapt abstract headings, titles, keywords, highlights, impact statements, reference style, tables, figures, and anonymization to the target journal.
6. Apply a consistent nursing and medical English standard.

### Key Principles

- Do not apply IJNS formatting to JMIR, Wiley, or other journals.
- Do not treat publisher-level rules as journal-specific rules.
- Journal of Advanced Nursing is a specific Wiley journal and should be handled through its own Author Guidelines.
- If no target journal is specified, use general nursing SCI English standards.
- For final submission formatting, provide the target journal's author guidelines or manuscript template whenever possible.

## 增强期刊适应模式 / Enhanced Journal Adaptation Mode

### 中文说明

当你同时提供目标期刊、研究设计和文章主题时，skill 会先进行联网检索，查找目标期刊中 2-3 篇使用相同或最相近方法设计、且可以获取全文的文章，再根据这些文章的结构和写作逻辑润色你的文本。

检索优先级为：

1. 相同研究设计，例如 cross-sectional study、scoping review、RCT、qualitative study。
2. 研究对象和疾病/状态，疾病优先于年龄段，例如 Alzheimer's disease/dementia 优先于 older adults。
3. 干预、暴露、技术或研究方法，例如 chatbot、digital intervention、AI-based tool。
4. 结局变量，例如 depression、quality of life、caregiver burden。

最低匹配标准是：相同研究设计 + 以上 2-4 点中的任意一点。也就是说，如果指定的是横断面研究，优先检索目标期刊中所有可获取全文的横断面研究，再逐步加入疾病、人群、chatbot、抑郁等关键词。

实际筛选时应先抓“同方法设计 + 主题最相似 + 可获取全文”的文章；如果没有，再逐步减少主题相似度。最次选择才是“同目标期刊 + 同方法设计 + 可获取全文，但主题相似度较低”的文章。

不能获取全文的文章不能作为范文。PubMed、Crossref、DOI 页面、数据库索引页或仅有摘要的页面只能用于发现候选文献，不能计入 2-3 篇范文。若出版社页面受限，应继续用 DOI、题名、PMCID、PMC、机构仓储或作者稿检索全文。

润色前还会判断文本属于论文哪个结构部分，例如 Abstract、Introduction、Methods、Results、Discussion、Limitations 或 Conclusion。随后只借鉴对应部分的写作逻辑，例如用 Abstract 范文改摘要结构，用 Methods 范文改方法顺序，用 Results 范文改统计报告方式。

示例：

```text
Use nursing-paper-polishing to polish this Abstract for JMIR Aging. This is a cross-sectional study about chatbot use for depression among older adults with Alzheimer's disease.
```

如果没有指定投稿期刊，则默认按 IJNS 风格和护理 SCI 严谨性要求约束语言和格式。

### English Guide

When you provide a target journal, study design, and manuscript topic, the skill first searches for 2-3 full-text published articles from the target journal that use the same or closest design. It then uses their section-level structure and writing logic to guide the revision.

Search priority:

1. Same study design, such as cross-sectional study, scoping review, RCT, or qualitative study.
2. Population and condition, with disease or condition prioritized before age group.
3. Intervention, exposure, technology, or method, such as chatbot or AI-based tool.
4. Outcome variable, such as depression, quality of life, or caregiver burden.

The minimum match is: same study design + at least one component from items 2-4.

In practice, the skill should first select full-text articles with the same design and the highest topic similarity. If none are available, it should reduce topic similarity step by step. The weakest acceptable same-journal fallback is a full-text article with the same design but low topic similarity.

Articles without accessible full text cannot be used as exemplars. PubMed, Crossref, DOI pages, indexing records, or abstract-only pages may help identify candidates, but they do not count toward the 2-3 exemplar articles. If a publisher page is restricted, the skill should search by DOI, title, PMCID, PMC, institutional repositories, or accepted manuscript copies.

Before polishing, the skill identifies the manuscript section, such as Abstract, Introduction, Methods, Results, Discussion, Limitations, or Conclusion. It then adapts only section-relevant patterns from the exemplar articles.

Example:

```text
Use nursing-paper-polishing to polish this Abstract for JMIR Aging. This is a cross-sectional study about chatbot use for depression among older adults with Alzheimer's disease.
```

If no target journal is specified, the skill defaults to IJNS-style nursing SCI constraints.
