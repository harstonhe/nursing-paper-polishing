<p align="right">
  <a href="README.md">English</a> | <strong>中文</strong>
</p>

# nursing-paper-polishing

作者：Harston

这是一个面向护理和医学论文的 Codex skill，用于英文润色、目标期刊适配，以及基于证据的缺失段落补写。

它的核心不是普通润色，而是先核对目标期刊作者指南，再检索 2-3 篇可获取全文、研究设计一致且主题最相近的范文文章，最后根据对应章节的写作逻辑来润色或补写。

## 主要功能

- 润色摘要、引言、方法、结果、讨论、结论、标题、highlights 和回复信。
- 适配 IJNS、JMIR、Elsevier 期刊、Wiley 期刊、Journal of Advanced Nursing 等目标期刊。
- 在期刊适配润色前检索可获取全文的同类范文。
- 根据用户提供的提纲、表格、图片、结果、protocol 或局部草稿补写缺失段落。
- 执行护理和医学语言约束，包括非因果研究避免因果表达，以及使用 `older adults` 等包容性术语。

## 核心流程

1. 识别目标期刊、文章类型、研究设计、主题和论文结构部分。
2. 核对目标期刊最新作者指南。
3. 检索 2-3 篇可获取全文的范文，优先同研究设计和最高主题相似度。
4. 提取范文中对应章节的写作结构。
5. 在不编造证据的前提下润色或补写文本。
6. 执行因果表达、包容性语言、格式和目标期刊检查。

## 范文检索规则

只使用可获取全文的范文。摘要页、PubMed 记录、Crossref 记录、DOI 元数据页和数据库索引页只能用于发现候选文章，不能计入范文。

优先级：

1. 同期刊 + 同研究设计 + 主题最相似 + 可获取全文。
2. 同期刊 + 同研究设计 + 部分主题相似 + 可获取全文。
3. 同期刊 + 同研究设计 + 可获取全文。
4. 同出版社或同领域 + 同研究设计 + 主题部分相似 + 可获取全文，仅在同期刊证据不足时使用。

## 缺失段落补写

skill 可以根据局部材料补写缺失段落，但用户提供的证据是所有结论的上限。

缺少关键信息时，会标注：

```text
AUTHOR_INPUT_NEEDED: [具体缺失项]
```

不得编造研究结果、样本量、纳入排除标准、检索日期、数据库、伦理信息、注册号、引用或实践意义。

## 示例提示词

```text
请调用 nursing-paper-polishing。目标期刊是 Journal of Nursing Scholarship，文章是关于 AI-chatbots 在痴呆症照护者中的使用情况的 scoping review。请润色 Methods 里的 Eligibility。
```

```text
请调用 nursing-paper-polishing，根据这些结果和 Table 2 补写 IJNS 投稿论文的 Discussion 缺失段落。
```

```text
Use nursing-paper-polishing to revise this Abstract for JMIR Aging. This is a cross-sectional study about chatbot use for depression among older adults with Alzheimer's disease.
```

## 输出内容

通常包括：

- 润色或补写后的文本
- 修改说明
- 因果表达检查
- 使用全文范文时的范文依据
- 补写内容时的证据来源和仍需作者补充的信息
- 用户要求时的格式检查
