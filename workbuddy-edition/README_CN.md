# Annual Report Forensic Analyst v2.2.4 WorkBuddy Marketplace Edition

[English](README.md) | 中文

这是 Annual Report Forensic Analyst v2.1.2 的 Apache License 2.0 WorkBuddy 适配版：一个基于证据的企业研究与管理层洞察框架，服务 CFO、战略、咨询和一般研究场景。它不是法律调查工具，也不是投资建议工具。

### 术语解释

- **Forensic Analysis（取证分析）**：指用证据验证主张的方法，不是法律调查、舞弊调查或审计意见。
- **Fact / Inference / Analyst View**：三层判断体系。Fact 是来源直接披露的事实；Inference 是基于事实的合理推断；Analyst View 是独立判断、局限性和不确定性。
- **PDF / Slides / Infographic**：输出转换层，用于把已完成研究转换为交付格式；正式或对外使用前需要人工复核，不代表自动形成获批的财务或管理决策。

## 支持能力

- Single Year Forensic Mode（单年度财报取证）
- Multi Year Forensic Mode（多年度财报取证）
- PDF Report Generation（PDF 研究报告）
- Executive Slide Generation（高管汇报幻灯片）
- Infographic Generation（企业研究信息图）

前两项用于研究，后三项用于将已完成研究转换为交付物；如用户已经提供研究结果，也可直接使用输出模式。

## Marketplace 快捷场景

- **三年年报分析**：默认比较三个可比年度，解释商业模式、叙事、财务和资本配置的变化。
- **CFO汇报材料**：生成面向 CFO 的证据驱动汇报结构，突出现金、资本配置、风险和监测指标。
- **PDF研究报告**：生成保留来源、局限性及 Fact / Inference / Analyst View 区分的 PDF-ready 报告。
- **企业研究信息图**：生成适合信息图制作的结论、证据、异议和视觉编码 brief。

## 快速开始

1. 按 [INSTALLATION.md](INSTALLATION.md) 安装。
2. 上传一份或多份年报文件。
3. 指定公司、期间、行业重点、受众和模式。
4. 要求每项重要结论区分事实、推断和分析师观点，并保留来源。
5. 对局限性和未解决问题进行复核，再对外使用输出。

### Quick Start Prompt / 快速启动 Prompt

```text
使用 Annual Report Forensic Analyst — WorkBuddy Edition。
公司：{{公司}}
模式：{{Single Year Forensic Mode 或 Multi Year Forensic Mode}}
分析期间：{{期间}}
行业重点：{{可选}}
年报文件：{{已上传文件}}
请将年报作为证据进行取证分析。每项重要结论必须区分 Fact、Inference、Analyst View，并列出支持证据、矛盾证据、来源位置、局限性和待调查问题。不得提供投资建议、评级、目标价、估值意见或缺乏证据支持的预测。
```

### 第一次使用流程

先上传年报并填写公司、期间和行业重点，再选择单年度或多年度研究模式。完成研究并复核证据、来源和不确定性后，再调用输出模式：

- **PDF 输出**：`请将已完成的取证研究转换为保留来源和局限性的 PDF-ready 研究报告，保留 Fact / Inference / Analyst View，并包含监测仪表板。`
- **Executive Slide 输出**：`请将已完成的取证研究转换为面向 {{受众}} 的 12 页高管汇报材料，每页只表达一个证据驱动的核心信息，并保留来源和不确定性。`
- **Infographic 输出**：`请将已完成的取证研究转换为企业研究信息图 brief，包含执行判断、价值创造链、主张、证据、矛盾、风险、监测信号和不确定性。`

## 推荐工作流

**Research Engine（研究引擎）**负责生成基于证据的取证研究：重建商业模式、验证管理层主张，并记录 Fact / Inference / Analyst View。**Output Layer（输出层）**再把已完成研究转换为 PDF 报告、Executive Slide brief 或信息图 brief。请保持顺序：**先研究，后输出**。正式或对外使用前，需要人工复核研究结果和转换后的交付物。

## Executive Slide 输出层

只有在已完成取证研究后，才使用 Executive Slide 输出层。它把研究转换为 CFO 汇报、CEO 讨论或战略复盘材料，不替代 Research Engine，也不强制固定页数。完整的输入、故事线、视觉、防退化和 QA 要求见 [中文提示词](prompts/executive-slide-generation-prompt_CN.md) 或 [English prompt](prompts/executive-slide-generation-prompt_EN.md)。

### 用户场景

- **CFO**：年度经营复盘、竞争分析、管理层汇报准备。
- **Strategy**：商业模式变化、竞争格局分析。
- **Consultant**：客户研究底稿、汇报材料准备。
- **General User**：上传年报即可开始企业研究。

## 边界与示例

管理层陈述必须作为待验证假设。该技能不提供投资建议、评级、目标价、估值意见或缺乏证据支持的预测。`examples/` 中的 SAP、Sandvik、Schneider、ABB 仅包含脱敏结构和占位符，不复制任何年报内容。

## 许可证

Apache License 2.0，见 [LICENSE](LICENSE)。
