# GitHub PPT 项目调研

本文件记录已读取的 GitHub 仓库内容，以及可供 `ppt-craft` 采用的工程做法。仓库之间没有已确认的继承、等价或官方认证关系。未复制仓库代码、模板和素材。

## 已核验项目

| GitHub 项目 | 已确认内容 | 融入本 skill 的做法 | 未自动采用的内容 |
| --- | --- | --- | --- |
| [anthropics/skills — pptx](https://github.com/anthropics/skills/blob/main/skills/pptx/SKILL.md) | 包含 PPTX 创建、模板编辑、内容提取、文件验证、渲染检查与常见 PptxGenJS 风险说明。 | 模板先分析；制作后分别进行内容、文件结构和逐页渲染检查；修改后重新渲染受影响页面。 | 仓库许可证标注为专有；不复制脚本、代码和具体设计预设。 |
| [siril9/presentation-skill](https://github.com/siril9/presentation-skill) | 使用 design brief、content plan、evidence plan、asset plan、outline 等项目记录；采用几何、渲染视觉、占位文字三类 QA。 | 在丰富大纲时建立主张与来源对应；在配图阶段记录素材用途；使用分层 QA。 | 其布局语料、路由器、脚本和模板没有在本地核验运行，尚未确认与当前环境兼容。 |
| [ningzimu/codex-ppt-skill](https://github.com/ningzimu/codex-ppt-skill) | 先确认大纲、视觉风格和样张，再批量生成整页图片并组装 PPTX；仓库说明整页图片元素不可直接编辑。 | 在生图阶段先做代表性样张；在排版前明确可编辑、整页图片或混合路线。 | 整页图片路线不作为默认方式；用户需要编辑或数据精度时优先使用原生元素。 |
| [Noi1r/powerpoint-skill](https://github.com/Noi1r/powerpoint-skill) | 展示了公式、Graphviz/Mermaid/TikZ 图形、重叠检查、PDF 渲染与视觉检查流程；说明 LibreOffice 对 OMML 的渲染有限制。 | 科研与技术演示按内容需要单独准备公式和结构图；区分 PowerPoint 实际显示与 QA 渲染器差异。 | 未引入公式与图形脚本；使用前需要用户任务确有需要并完成本地兼容验证。 |
| [slidevjs/slidev](https://github.com/slidevjs/slidev/blob/main/docs/guide/syntax.md) | 支持逐页布局、演讲者备注、代码高亮、LaTeX 与图表语法。 | 技术演示可把代码、公式、图表与讲者备注作为独立内容类型规划。 | Slidev 输出与 `.pptx` 的关系未在本任务中核验，不作为 PowerPoint 制作后端。 |
| [marp-team/marp](https://github.com/marp-team/marp) | 提供 Markdown 幻灯片生态和主题机制。 | 证明“内容源与主题分离”是一种已存在的工程实现；用于启发内容计划和视觉系统分离。 | 未确认其导出结果满足当前 PowerPoint 编辑性要求，不替换 `presentations` skill。 |

## 由仓库案例归纳的工程流程

以下内容是跨项目归纳，属于工程建议：

1. 先保存或明确内容结构，再绑定版式和素材。
2. 为事实、数据、图片和图表保留来源对应关系。
3. 批量生图前检查一页代表性样张。
4. 制作前确定编辑性路线；整页图片适合强视觉输出，原生对象方便后续编辑和数据核对。
5. QA 分成内容、文件结构、几何与渲染视觉检查；单一检查无法覆盖全部问题。
6. 模板编辑先识别现有页面与布局，再进行结构调整和内容替换。
7. 公式、图表、图形和讲者备注按独立内容类型处理，避免在普通文本框中降级表达。

## 安全与范围

引用 GitHub 仓库只代表已读取其公开页面。Star 数、仓库名称或相似功能不能证明质量、理论正确性、官方关系或适合当前环境。未经用户授权，不克隆仓库、不安装依赖、不执行社区脚本、不复制受许可证约束的模板与素材。
