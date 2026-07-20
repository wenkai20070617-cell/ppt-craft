# PPT 设计理论与证据｜Presentation Design Theory and Evidence

本文件支持 `ppt-craft` 的设计判断。每条内容只在其证据覆盖的条件下使用。它们不替代用户材料、受众研究、行业规范或品牌要求。

This file supports design decisions in `ppt-craft`. Apply each principle only within the scope supported by its evidence. These sources do not replace user material, audience research, industry rules, or brand requirements.

## 已确认理论与研究｜Confirmed theories and research

| 理论 / Theory | 来源支持的内容 / Evidence supported by the source | PPT 用法 / Application | 边界 / Boundary |
| --- | --- | --- | --- |
| 多媒体学习：连贯 / Multimedia learning: coherence | 排除无关素材可减少外在加工并促进学习。Excluding extraneous material can reduce extraneous processing and support learning. | 删除与页面任务无关的文字、装饰、动画和数据。Remove copy, decoration, animation, and data that do not support the slide's job. | 主要针对学习材料；用于其他演示时属于设计推断。Primarily studied in learning materials; transfer to other presentation settings is a design inference. |
| 提示与邻近 / Signalling and contiguity | 视觉线索突出结构；相关文字和图形靠近可降低外在加工。Cues reveal structure, while proximity between related words and graphics can reduce extraneous processing. | 用层级和标注指出重点，将说明贴近对应图形。Use hierarchy and annotations to signal focus; place explanations beside their referents. | 仍需结合受众知识和讲述方式。Audience knowledge and delivery still matter. |
| 分段、预训练与个性化 / Segmenting, pre-training, personalisation | Mayer 的原则包含分段、预先说明关键概念和对话式表达。Mayer's principles include segmentation, advance explanation of key concepts, and conversational language. | 拆分复杂过程，先定义术语，教学场景使用自然清晰的语言。Break down complex processes, define terms early, and use clear natural language in teaching contexts. | 决策汇报可能需要更紧凑表达。Decision decks may require tighter copy. |
| 认知负荷 / Cognitive load | 工作记忆容量有限，教学设计应减少不必要负荷并促进图式构建。Working memory is limited; instructional design should reduce unnecessary load and support schema construction. | 减少分散搜索，将复杂关系分层呈现。Reduce split attention and reveal complex relationships in layers. | 不能单独预测商业说服效果。It does not by itself predict persuasive success. |
| PowerPoint 应用研究 / PowerPoint application research | Grech 将 Mayer 的十二项原则应用于医学 PowerPoint，并提出幻灯片用于补充演讲。Grech applies Mayer's twelve principles to medical PowerPoint and frames slides as support for the talk. | 页面保留可视证据、结构和提示，讲者负责解释与过渡。Let slides carry visual evidence, structure, and cues while the speaker supplies explanation and transitions. | 研究情境为医学教育。The context is medical education. |
| 图形感知 / Graphical perception | Cleveland 与 McGill 比较位置、长度、角度、面积和颜色等视觉任务的判断准确性。Cleveland and McGill compare perceptual accuracy for position, length, angle, area, colour, and related encodings. | 精确比较优先用共用基线上的位置或长度；谨慎使用面积、角度和颜色饱和度。Prefer common-position or length encodings for precise comparisons; use area, angle, and colour saturation carefully. | 效果还受数据、受众和展示时间影响。Data, audience familiarity, and viewing time also affect performance. |
| 文字对比度 / Text contrast | WCAG 2.2 规定普通文字至少 4.5:1，大号文字至少 3:1。WCAG 2.2 specifies at least 4.5:1 for normal text and 3:1 for large text. | 测量文字与背景对比度，必要时使用遮罩或纯色区域。Measure text/background contrast and use masks or solid fields when needed. | WCAG 是网页标准；用于 PPT 是设计基线，不自动构成组织合规。WCAG is a web standard; using it for slides is a design baseline, not automatic organisational compliance. |
| PowerPoint 无障碍 / PowerPoint accessibility | Microsoft 建议唯一标题、足够对比度、替代文本、内置布局和非颜色单一编码。Microsoft recommends unique titles, sufficient contrast, alt text, built-in layouts, and cues beyond colour. | 添加替代文本和非颜色线索，运行 Accessibility Checker。Add alt text and non-colour cues, and run Accessibility Checker. | 自动检查只能发现部分问题。Automated checks cover only part of accessibility. |

## 使用方法｜How to apply

1. 确认页面任务：解释、比较、证明、决策、教学、过程或行动。Identify the slide's job: explain, compare, prove, decide, teach, show a process, or request action.
2. 选择匹配的表达：精确比较用条形图或点图，趋势用折线图，因果或流程用步骤图，概念关系用清晰连接图。Choose a matching form: bars or dots for exact comparison, lines for trends, step diagrams for processes or causes, and clearly connected diagrams for concepts.
3. 检查无关负荷、重点提示、图文邻近、可读性、数据含义和替代线索。Check extraneous load, signalling, contiguity, readability, data meaning, and redundant cues.
4. 生成后渲染并逐页检查，记录未验证项目。Render and inspect every slide after generation, and record anything unverified.

## 来源｜Sources

- Richard E. Mayer, [Principles for Reducing Extraneous Processing in Multimedia Learning](https://www.cambridge.org/core/books/abs/cambridge-handbook-of-multimedia-learning/principles-for-reducing-extraneous-processing-in-multimedia-learning-coherence-signaling-redundancy-spatial-contiguity-and-temporal-contiguity-principles/C98AB3A6CE760DD63C048936EA0B3B44).
- John Sweller, [Cognitive Architecture and Instructional Design](https://research.utwente.nl/en/publications/cognitive-architecture-and-instructional-design/).
- Victor Grech, [The application of the Mayer multimedia learning theory to medical PowerPoint slide show presentations](https://pubmed.ncbi.nlm.nih.gov/29381105/).
- Gharabegian et al., [Presentation design and delivery to improve knowledge translation in a remote world](https://pubmed.ncbi.nlm.nih.gov/36202597/).
- William S. Cleveland and Robert McGill, [Graphical Perception](https://lenagroeger.s3.amazonaws.com/newschool/ClevelandMcGill.pdf).
- W3C, [Understanding SC 1.4.3: Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum).
- Microsoft Support, [Make your PowerPoint presentations accessible](https://support.microsoft.com/en-us/accessibility/powerpoint/make-your-powerpoint-presentations-accessible-to-people-with-disabilities).

## 结论边界｜Conclusion boundary

这些资料支持减少无关负荷、突出关键信息、让关联内容相邻、选择可准确解读的图表编码和保障可读性的方向。它们不能证明某一种版式、页数、配色或动画适合所有场景。

The sources support reducing extraneous load, signalling essential material, placing related content together, choosing accurately decoded chart encodings, and protecting readability. They do not prove that one layout, slide count, palette, or animation works for every topic, audience, and setting.
