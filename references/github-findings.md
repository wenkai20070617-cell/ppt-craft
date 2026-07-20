# GitHub PPT 项目调研｜GitHub PPT Project Review

本文件记录已读取的 GitHub 仓库内容及可供 `ppt-craft` 采用的工程做法。仓库之间没有已确认的继承、等价或官方认证关系。未复制仓库代码、模板和素材。

This file records verified public GitHub content and engineering practices considered for `ppt-craft`. No inheritance, equivalence, or official endorsement among the repositories has been confirmed. No repository code, templates, or assets were copied.

## 已核验项目｜Verified projects

| 项目 / Project | 已确认内容 / Confirmed content | 融入方式 / Adopted practice | 未自动采用 / Not adopted automatically |
| --- | --- | --- | --- |
| [anthropics/skills — pptx](https://github.com/anthropics/skills/blob/main/skills/pptx/SKILL.md) | 包含创建、模板编辑、提取、文件验证、渲染检查和 PptxGenJS 风险。Covers creation, template editing, extraction, file validation, rendered review, and PptxGenJS risks. | 模板先分析；分开执行内容、文件和渲染 QA。Analyse templates first; separate content, file, and rendered QA. | 许可证标注为专有；不复制代码和预设。The repository marks its licence as proprietary; no code or presets are copied. |
| [siril9/presentation-skill](https://github.com/siril9/presentation-skill) | 使用 design brief、content plan、evidence plan、asset plan、outline 和分层 QA。Uses design, content, evidence, asset, and outline records with layered QA. | 建立主张与来源对应，记录素材用途，采用分层 QA。Map claims to sources, record asset roles, and use layered QA. | 本地未运行其路由器、脚本和模板。Its router, scripts, and templates were not run locally. |
| [ningzimu/codex-ppt-skill](https://github.com/ningzimu/codex-ppt-skill) | 先确认大纲、视觉风格和样张，再批量生成整页图片；整页图片不可直接编辑。Confirms outline, visual style, and sample before batch full-slide images; full-slide images are not directly editable. | 生图前检查样张；排版前确定编辑性路线。Review a sample before batch generation and choose an editability route before layout. | 整页图片不设为默认。Full-slide imagery is not the default route. |
| [Noi1r/powerpoint-skill](https://github.com/Noi1r/powerpoint-skill) | 展示公式、图形、重叠检查、PDF 渲染和视觉 QA；记录 LibreOffice 对 OMML 的限制。Shows formula and diagram pipelines, overlap checks, PDF rendering, visual QA, and LibreOffice's OMML limitation. | 科技内容单独规划公式与图形，并记录渲染器差异。Plan formulas and diagrams as distinct content types and record renderer differences. | 未引入其脚本。Its scripts were not imported. |
| [slidevjs/slidev](https://github.com/slidevjs/slidev/blob/main/docs/guide/syntax.md) | 支持逐页布局、讲者备注、代码高亮、LaTeX 和图表语法。Supports per-slide layouts, speaker notes, code highlighting, LaTeX, and diagram syntax. | 技术演示把代码、公式、图表和备注作为独立内容类型。Treat code, formulas, diagrams, and notes as distinct content types. | 未核验其 `.pptx` 输出，不作为 PowerPoint 后端。Its `.pptx` output was not verified, so it is not a PowerPoint backend here. |
| [marp-team/marp](https://github.com/marp-team/marp) | 提供 Markdown 演示生态和主题机制。Provides a Markdown presentation ecosystem and themes. | 借鉴内容源与主题分离的工程思想。Use its separation of content source and theme as an engineering pattern. | 未确认导出结果符合当前编辑性要求。Its exports were not verified against current editability requirements. |

## 归纳的工程流程｜Derived engineering workflow

1. 先明确内容结构，再绑定版式和素材。Define content structure before binding layouts and assets.
2. 为事实、数据、图片和图表保留来源对应。Keep provenance for facts, data, images, and charts.
3. 批量生图前检查代表性样张。Review a representative sample before batch image generation.
4. 制作前确定编辑性路线。Choose the editability route before production.
5. 分别执行内容、文件结构、几何和渲染视觉检查。Run content, file-structure, geometry, and rendered visual checks separately.
6. 模板编辑先识别页面和布局，再调整结构与内容。Identify template slides and layouts before structural and content edits.
7. 公式、图表、图形和讲者备注按独立内容类型处理。Treat formulas, charts, diagrams, and speaker notes as distinct content types.

## 安全与范围｜Safety and scope

引用公开仓库只代表已读取其公开页面。Star 数、名称和功能相似不能证明质量、理论正确性、官方关系或环境兼容。未经用户授权，不克隆仓库、不安装依赖、不执行社区脚本、不复制受许可证约束的模板和素材。

Citing a public repository means only that its public page was read. Stars, names, and feature similarity do not establish quality, theoretical validity, official relationships, or environment compatibility. Do not clone repositories, install dependencies, run community scripts, or copy licence-restricted templates and assets without user authorisation.
