---
name: ppt-craft
description: Create, revise, or audit audience-ready PowerPoint presentations (.pptx) through a gated workflow covering outline, evidence, images, layout, production, and rendered quality assurance. The skill instructions are available in Chinese and English. Produce slides in the user's requested language, and use bilingual slide content only when explicitly requested. Use when Codex must turn a brief, source material, or data into a professional deck, improve an existing presentation, or evaluate its content and design. 本技能提供中英文说明，并按用户指定语言制作演示文稿；仅在用户明确要求时制作双语页面。
---

# PPT Craft｜PPT 制作（中英双语技能说明）

## Confirm the task｜确认任务

确认受众、目标、场景、时长、语言、必用资料、品牌或模板限制、输出格式，以及成品是否需要可编辑。缺失信息会实质改变内容或路线时，只问一个具体问题。

Confirm the audience, objective, setting, duration, language, required sources, brand or template constraints, output format, and editability requirements. Ask one focused question only when missing information would materially change the result.

区分已确认事实、建议、推断和待确认信息。数据、引文、机构立场、品牌素材、图片来源和对象关系必须有证据。重要事实保留逐页来源或来源页。

Separate confirmed facts, recommendations, inferences, and unconfirmed information. Require evidence for data, quotations, institutional positions, brand assets, image provenance, and object relationships. Keep slide-level citations or a sources slide for material claims.

阅读 [references/presentation-principles.md](references/presentation-principles.md) 获取理论依据。需要选择生成路线、项目记录或 QA 方法时，阅读 [references/github-findings.md](references/github-findings.md)。GitHub 项目属于实现案例，不承担学术理论证明。

Read [references/presentation-principles.md](references/presentation-principles.md) for research-grounded design guidance. Read [references/github-findings.md](references/github-findings.md) when choosing an implementation route, working records, or QA method. Treat GitHub repositories as implementation examples, not academic evidence.

## Language policy｜语言策略

- 本 skill 的说明同时提供中文和英文；这不表示成品 PPT 默认使用两种语言。This skill is documented in Chinese and English; that does not make the output deck bilingual by default.
- 按用户明确指定的语言制作页面与演讲者备注。未指定时，采用用户请求和主要资料所使用的语言。Produce slides and speaker notes in the language explicitly requested. If none is specified, use the language of the request and primary source material.
- 不自动添加译文、双语副标题或第二语言正文。仅在用户明确要求双语演示时，才在每页建立主次语言层级并保持语义对应。Do not add translations, bilingual subtitles, or secondary-language body copy by default. Create bilingual slides only when the user explicitly requests them, then establish a clear primary/secondary hierarchy and preserve semantic equivalence.
- 标题保持简短完整；专有名词、数字、来源和行动要求在选定语言中保持一致。Keep titles concise and complete; preserve terminology, numbers, citations, and requested actions in the selected language.

## Gated workflow｜固定制作顺序

按以下顺序推进。每一步检查上一轮结果；发现问题时回到对应步骤修正。用户已经授权连续执行时，内部完成各检查点并继续；缺少关键选择时再请求确认。

Follow the sequence below. Check each result before continuing and return to the relevant step when a defect is found. Continue through internal gates when the user has authorized end-to-end execution; request input only for a material missing choice.

1. **写大纲｜Draft the outline**
   - 写出受众需求、中心结论、核心论点、证据链、行动或结语。Define the audience need, central takeaway, supporting claims, evidence chain, and action or conclusion.
   - 为每页记录页码、结论式标题、页面任务、所需证据和预计视觉形式。Record each slide's number, takeaway title, narrative job, evidence need, and intended visual form.
2. **优化大纲｜Refine the outline**
   - 检查语境、论证顺序、受众理解路径和结尾行动。Check context, argumentative sequence, audience comprehension path, and closing action.
   - 删除重复与无关页面，补齐证据缺口和过渡；页数由内容与时长共同决定。Remove repetition, close evidence gaps, add transitions, and let content plus duration determine slide count.
3. **丰富大纲｜Enrich the outline**
   - 补齐经核验的事实、数据、案例、定义、讲述重点和来源。Add verified facts, data, cases, definitions, talking points, and sources.
   - 建立“主张—证据—来源—页面”对应关系；资料不足时标注待确认。Map claim to evidence, source, and slide; mark missing material as unconfirmed.
   - 将长段文字转换成比较、流程、因果模型、时间线、图表、示意图或短列表。Convert long prose into comparisons, processes, causal models, timelines, charts, diagrams, or short lists.
4. **配图｜Source visuals**
   - 先定义每页视觉任务，再搜索照片、插图、图标、图表或原始示意图。Define each visual's job before searching for photos, illustrations, icons, charts, or source diagrams.
   - 记录来源、许可状态、原图链接、建议裁切、页面用途和替代文本需求。Record provenance, license status, source URL, crop, slide purpose, and alt-text needs.
5. **优化配图方案｜Refine the visual plan**
   - 检查图片是否支持页面结论，以及风格、视角、光线、色彩和抽象程度是否协调。Check whether each image supports the claim and whether style, viewpoint, lighting, colour, and abstraction are coherent.
   - 检查裁切、分辨率、留白和文字覆盖区域；明确直接使用、编辑或生成的素材。Check crop, resolution, negative space, and copy placement; classify assets as use, edit, or generate.
6. **生图｜Generate images**
   - 只为缺少合适素材且确有表达价值的页面生成图片。Generate only when suitable source material is unavailable and a new image adds explanatory value.
   - 提示词包含主题、主体、构图、风格、色彩、画幅、留白和禁止元素。Include subject, composition, style, colour, aspect ratio, negative space, and exclusions in the prompt.
   - 先检查代表性样张，再生成其余图片；核对文字、人物、标识、事实暗示、版权风险和跨页一致性。Approve a representative sample before the remaining images; check text, people, marks, factual implications, copyright risk, and consistency.
   - 精确数据图、结构图和需编辑文字优先使用原生对象。Prefer native objects for precise data, structured diagrams, and editable text.
7. **生成 PPT 排版方案｜Plan slide layouts**
   - 明确每页布局、标题层级、正文与视觉位置、图表、标注、对齐、色彩和留白。Specify layout, hierarchy, copy and visual placement, charts, labels, alignment, colour, and whitespace.
   - 选择可编辑、整页图片或混合路线，并记录选择依据。Choose an editable, image-based, or hybrid route and record the rationale.
   - 使用母版或复用布局维护视觉系统，让页面结构服务内容。Use masters or reusable layouts for consistency while adapting each slide to its content.
8. **优化排版方案｜Refine layouts**
   - 按目标尺寸检查阅读顺序、对比度、字号、密度、对齐、图表可读性、视觉重心和跨页节奏。Check reading order, contrast, type size, density, alignment, chart readability, visual balance, and pacing at the target size.
   - 检查页面边界、文本容器、图片裁切和来源区域，预留渲染差异空间。Check canvas bounds, text containers, image crops, and citation areas; leave room for rendering variance.
   - 对代表性页面进行样张检查后再进入制作。Review representative slide proofs before production.
9. **开始制作 PPT｜Produce the PPT**
   - 使用 `presentations` skill 生成或编辑 `.pptx`，落实已确认内容、素材和版式。Use the `presentations` skill to create or edit the `.pptx` from the approved content, assets, and layouts.
   - 编辑模板时先查看缩略图与文本，完成页面增删和排序后再替换内容。When editing a template, inspect thumbnails and text, finish structural changes, then replace slide content.
   - 保持图表、表格、文字和基础图形可编辑；复杂视觉按已确认路线处理。Keep charts, tables, text, and basic shapes editable; handle complex visuals according to the chosen route.

## Content and visual rules｜内容与视觉准则

每页承担一个明确任务，标题表达结论或问题。用层级、位置和标注引导阅读，将标签放在对应图形或数据旁边。

Give each slide one narrative job. Write titles as conclusions or questions. Use hierarchy, position, and annotation to guide reading, and place labels beside the graphics or data they explain.

图表从问题出发选择编码：精确比较用条形图或点图，趋势用折线图，构成用合适的部分—整体图，分布用直方图或点图，关系用散点图，地理分布用地图。标注单位、期间、定义、分母、不确定性和来源；坐标轴、排序和截断不得改变数据含义。

Choose chart encodings from the question: bars or dots for precise comparison, lines for trends, appropriate part-to-whole forms for composition, histograms or dots for distributions, scatterplots for relationships, and maps for geographic patterns. Label units, periods, definitions, denominators, uncertainty, and sources. Do not distort meaning through axes, ordering, or truncation.

颜色以外增加标签、形状、纹理、线型或位置线索。为有意义的视觉元素提供替代文本，使用唯一且描述明确的标题。

Add labels, shapes, textures, line styles, or position cues in addition to colour. Provide alt text for meaningful visuals and use unique, descriptive slide titles.

## Acceptance checks｜成品验收

1. **内容检查｜Content**：核对页序、事实、数字、来源、术语、拼写、备注和占位文字。Check order, facts, numbers, citations, terminology, spelling, notes, and placeholders.
2. **文件检查｜File**：确认 `.pptx` 可以打开，页面关系、媒体、图表和模板关联完整。Confirm that the file opens and that slide relationships, media, charts, and template links remain intact.
3. **几何检查｜Geometry**：检查越界、重叠、过密、间距、对齐、文本溢出和图片拉伸。Check bounds, overlap, density, spacing, alignment, text overflow, and image distortion.
4. **渲染检查｜Rendered review**：渲染全部页面并逐页查看；修正后重新渲染受影响页面。Render and inspect every slide; re-render affected slides after fixes.
5. **交付检查｜Delivery**：确认成品符合大纲、视觉路线、语言、编辑性、尺寸和路径要求。Confirm the deck matches the outline, visual route, language, editability, dimensions, and output path.

报告实际输出路径、已完成检查、已修复问题和未验证项目。编辑现有演示文稿时，保留用户确认的内容与风格限制。

Report the actual output path, completed checks, fixed defects, and any unverified items. Preserve confirmed content and style constraints when editing an existing deck.
