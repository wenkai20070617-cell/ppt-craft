# PPT 设计理论与证据

本文件用于支持 `ppt-craft` 的设计判断。每条内容只在其证据覆盖的条件下使用；它们不替代用户材料、受众研究、行业规范或品牌要求。

## 已确认的理论与研究

| 理论或研究 | 来源支持的内容 | 对 PPT 的可执行用法 | 适用边界 |
| --- | --- | --- | --- |
| 多媒体学习：连贯原则 | Mayer 说明，排除无关素材可减少外在加工并促进学习。 | 删除与页面目标无关的文字、装饰、动画和数据。 | 主要针对多媒体教学与学习；用于汇报或提案时属于设计判断。 |
| 多媒体学习：提示与邻近原则 | Mayer 将突出关键信息的线索，以及相关文字和图形的空间或时间邻近，列为降低外在加工的方法。 | 用标题、颜色、标注或渐进显示指出重点；将说明贴近对应图形或数据。 | 复杂材料仍需结合受众先验知识与讲述方式。 |
| 多媒体学习：分段、预训练与个性化 | Mayer 的多媒体原则包含按学习者节奏分段、先说明关键概念、使用对话式表达等方法；PPT 应用研究将这些原则用于幻灯片设计。 | 将复杂过程拆成可理解的页或步骤；首次出现的术语先定义；面向教学或培训时优先使用清晰自然的讲述语言。 | 适用于教学、培训与知识传递；高层决策汇报可能需要更紧凑的表达。 |
| 认知负荷理论 | Sweller 将工作记忆容量视为有限，并讨论降低不必要负荷、促进图式构建的教学设计。 | 避免让观众同时在多处寻找彼此关联的信息；将复杂因果关系分层呈现。 | 该理论源于教学设计，无法单独确定商业演示的说服效果。 |
| PowerPoint 的多媒体学习应用 | Grech 的同行评议论文将 Mayer 的十二项多媒体设计原则应用于医学 PowerPoint，并指出幻灯片用于补充演讲。 | 将演讲与页面分工：页面保留可视证据、结构和关键提示；讲者提供解释与过渡。 | 研究情境为医学教育，迁移到其他场景时需要结合实际目的。 |
| 图形感知 | Cleveland 与 McGill 的实验研究比较了位置、长度、角度、面积、颜色等基础视觉任务，并主张在图表中优先采用更易准确判断的任务。 | 精确比较优先采用共用基线上的位置或长度编码，如点图或条形图；面积、角度和颜色饱和度用于精确比较时要谨慎。 | 数据类型、受众熟悉度和展示时间仍会影响效果。 |
| 可访问性：文字对比度 | W3C WCAG 2.2 的理解文件规定：普通文字与背景至少 4.5:1；大号文字至少 3:1。 | 在图片底图、渐变和投影环境中实际测量文字与背景的对比度；用遮罩或纯色区域保证可读性。 | WCAG 是网页可访问性标准；将其用于 PPT 是明确的可访问性设计基线，不自动等同于某个组织的合规要求。 |
| PowerPoint 可访问性 | Microsoft 建议使用唯一且描述性的幻灯片标题、足够对比度、替代文本、内置布局，并避免单独依赖颜色传递信息。 | 对有意义的视觉内容写替代文本；为图表提供颜色以外的标签、形状、线型或位置线索；运行 PowerPoint Accessibility Checker。 | 检查器只能发现部分问题，仍需在实际展示与阅读环境中人工检查。 |

## 用法

1. 先确认页面任务：解释、比较、证明、决策、教学、过程说明或行动请求。
2. 选择与任务匹配的表达：
   - 精确比较：条形图、点图、直接数值标注。
   - 时间变化：折线图或带明确时间轴的时间线。
   - 因果或流程：步骤图、因果图、前后对比。
   - 概念关系：带清晰连接与标签的关系图。
3. 再用理论检查：是否有无关负荷、重点提示、图文邻近、可读性、数据含义和替代线索。
4. 生成 `.pptx` 后，渲染并逐页检查；记录无法验证的项目。

## 来源链接

- Richard E. Mayer, [Principles for Reducing Extraneous Processing in Multimedia Learning](https://www.cambridge.org/core/books/abs/cambridge-handbook-of-multimedia-learning/principles-for-reducing-extraneous-processing-in-multimedia-learning-coherence-signaling-redundancy-spatial-contiguity-and-temporal-contiguity-principles/C98AB3A6CE760DD63C048936EA0B3B44).
- John Sweller, [Cognitive Architecture and Instructional Design](https://research.utwente.nl/en/publications/cognitive-architecture-and-instructional-design/).
- Victor Grech, [The application of the Mayer multimedia learning theory to medical PowerPoint slide show presentations](https://pubmed.ncbi.nlm.nih.gov/29381105/).
- Gharabegian et al., [Presentation design and delivery to improve knowledge translation in a remote world](https://pubmed.ncbi.nlm.nih.gov/36202597/).
- William S. Cleveland and Robert McGill, [Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods](https://lenagroeger.s3.amazonaws.com/newschool/ClevelandMcGill.pdf).
- W3C, [Understanding SC 1.4.3: Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum).
- Microsoft Support, [Make your PowerPoint presentations accessible to people with disabilities](https://support.microsoft.com/en-us/accessibility/powerpoint/make-your-powerpoint-presentations-accessible-to-people-with-disabilities).

## 结论边界

这些资料支持“减少无关负荷、突出关键信息、让关联内容相邻、选择可准确解读的图表编码、保障可读性”的设计方向。它们不能证明某一种版式、页数、配色或动画会对所有主题、受众和场景产生同样的效果。最终页面应以用户确认的目标、事实和约束为准。
