# Niuma Reviewer / 牛马审稿人

## 中文简介

**Niuma Reviewer（牛马审稿人）** 是一个面向护理科研工作者的 AI 初审辅助 skill，主要用于在正式投稿前模拟医学期刊审稿视角，帮助作者提前发现稿件中的期刊匹配、方法学、伦理透明度、统计报告、数据可复现性、结果解释和投稿格式问题。

本 skill 的目标不是替代真实同行评议，也不是直接给出录用保证，而是帮助护理、老年照护、数字健康、医学人工智能、量表开发、Delphi 研究、系统综述和临床护理研究作者，在投稿前进行一轮更接近期刊审稿标准的自查。

## 当前适配范围

目前主要适配：

- **JMIR 系列期刊**：重点支持 JMIR 正刊及 JMIR 系列期刊的作者指南、审稿人表单格式、数据共享、伦理声明、生成式 AI 使用披露和数字健康研究报告要求。
- **BMC 系列期刊**：面向 BMC Nursing、BMC Medical Informatics and Decision Making、BMC Geriatrics、BMC Health Services Research 等开放获取医学与护理期刊，按目标期刊的 aims and scope、submission guidelines、ethics policies 和 reporting guidelines 进行初审。

未来计划扩展：

- **Wiley** 护理与医学期刊
- **Elsevier** 护理、医学信息学与公共卫生期刊
- 其他 Springer Nature、SAGE、Taylor & Francis 等医学与护理方向期刊

## 核心功能

- 检索目标期刊的 aims and scope、author guidelines、article types 和 reporting requirements
- 判断稿件是否适合目标期刊和目标文章类型
- 识别可能导致 desk reject 的问题
- 检查伦理审批、知情同意、数据共享、利益冲突和 AI 使用声明
- 根据研究类型检查 CONSORT、STROBE、PRISMA、TRIPOD、STARD、COREQ、CHART 等报告规范
- 从编辑、方法学审稿人、临床/护理领域审稿人、完整性与报告规范审稿人的角度综合评价
- 按 JMIR 审稿人模板输出 confidential comments、general comments、major comments 和 minor comments
- 为作者生成投稿前修改优先级和关键修订建议

## 使用场景

适用于以下类型稿件的投稿前初审：

- 护理科研论文
- 医学人工智能和数字健康研究
- 老年照护、慢病管理、健康服务研究
- 量表开发与验证研究
- Delphi 或专家共识研究
- 系统综述、范围综述、Meta 分析
- 临床观察性研究、诊断/预测模型研究、混合方法研究

## 使用示例

```text
请调用 Niuma Reviewer，按照 JMIR 正刊的要求，帮我初审这篇护理人工智能论文。
```

```text
Use Niuma Reviewer to review this nursing manuscript for BMC Nursing before submission.
```

## English Overview

**Niuma Reviewer** is an AI-assisted preliminary peer-review skill for nursing and medical researchers. It helps authors evaluate manuscripts before submission by simulating journal-facing review perspectives and identifying issues related to journal fit, methodology, ethics, statistical reporting, reproducibility, claim-evidence alignment, and submission formatting.

The skill does not replace real peer review and does not predict acceptance. Its purpose is to help authors conduct a structured pre-submission audit that is closer to journal editorial and reviewer expectations.

## Current Journal Coverage

Currently focused on:

- **JMIR journals**: supports JMIR-style reviewer output, author instructions, reporting expectations, data-sharing requirements, ethics statements, and generative AI disclosure.
- **BMC journals**: supports preliminary review for journals such as BMC Nursing, BMC Medical Informatics and Decision Making, BMC Geriatrics, and BMC Health Services Research by checking journal scope, submission guidelines, ethics policies, and reporting requirements.

Planned expansion:

- **Wiley** nursing and medical journals
- **Elsevier** nursing, medical informatics, and public health journals
- Additional medical and nursing journals from Springer Nature, SAGE, Taylor & Francis, and other publishers

## Main Capabilities

- Search and summarize target-journal aims, scope, author instructions, article types, and reporting requirements
- Assess journal fit and article-type fit
- Identify potential desk-rejection risks
- Check ethics approval, consent, data availability, conflicts of interest, and AI-use disclosure
- Evaluate reporting standards such as CONSORT, STROBE, PRISMA, TRIPOD, STARD, COREQ, and CHART
- Review from multiple perspectives: handling editor, methods/statistics reviewer, clinical or nursing domain reviewer, and integrity/reporting reviewer
- Produce JMIR-style confidential comments, general comments, major comments, and minor comments
- Provide prioritized pre-submission revision advice

## Intended Users

Niuma Reviewer is designed for:

- nursing researchers
- graduate students and early-career researchers
- clinical nursing teams preparing manuscripts
- digital health and medical AI researchers
- authors preparing manuscripts for JMIR, BMC, and related medical journals

## Disclaimer

Niuma Reviewer is a pre-submission review aid. Authors should verify all journal requirements from official sources and should not treat the output as a substitute for professional editorial advice, institutional ethics review, statistical consultation, or formal peer review.
