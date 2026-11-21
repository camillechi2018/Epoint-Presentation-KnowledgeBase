# Epoint Presentation 知识库

这是供 [Epoint Presentation 技能](https://github.com/camillechi2018/Epoint-Presentation)调用的结构化 PPT 模板知识库。仓库保存可编辑来源页、组件字段与容量规则、主题资料和验收记录。普通正文组件优先按结构、字段与容量匹配；专用组件保留严格语义或数据契约检查。是否进入自动选稿，以当前记录的主题、页面职责、验收状态、项数及字段容量共同判断。

**当前知识库发布版本：v1.0.3；配套技能：v1.0.33。** [查看知识库 v1.0.3](https://github.com/camillechi2018/Epoint-Presentation-KnowledgeBase/releases/tag/v1.0.3) · [查看技能 v1.0.33](https://github.com/camillechi2018/Epoint-Presentation/releases/tag/v1.0.33)。发布标签是仓库快照，不改变下述组件验收状态或清单内部版本。

## v1.0.3 更新与使用

- 收录 v1.0.2 之后的蓝红正文长文案容量、可选副标题、科技风配色和可选摘要调整，并修复知识库文件清单与实际内容不一致的问题。
- 内容基线为已验证提交 `20e35aa6757d7cab1d65f9294c48b6c390684835`。本次发布准备仅更新 README 及对应清单哈希，不修改模板、绑定、目录或主题资源；清单包含 3,451 项文件。
- 技能 v1.0.33 默认从本仓库 `main` 获取更新。需要可复现快照或离线部署时，使用 `v1.0.3` 标签或发布页的知识库 ZIP；这是知识库，不是技能安装包。解压后按技能的本地知识库目录参数使用。
- 技能仓库负责安装和出稿，私有维护仓库负责知识库构建、清单及发布工具；普通用户不需要私有维护仓库访问权限。
- Mac 三色完整材料各 20 页的生成与内容保真已实测通过；后续应用打开、编辑性、逐页视觉及 DSL 项目由项目负责人接受为配套发布豁免，未记为已实测。组件草稿状态和每份成稿的验收要求仍保留。

> 资产状态：`draft_pending_review`。使用草稿组件须显式允许并进行人工审阅；预览图不代表该组件的所有能力均已验收。

科技风纯正文的 v3 契约声明 `background: skill_tech`，由支持 v3 契约的技能装配公共背景。原稿保留母版背景，供来源追溯和旧版本整页出稿使用。

## 三种风格预览

蓝色、红色、科技风格各展示一张封面和 16 个正文组件。图片中的文字和数字是版式示例，实际出稿以用户材料替换。

| 页面 | 蓝色系 · 蓝白简约 | 红色系 · 红白简约 | 科技风格 · 深蓝科技 |
| --- | --- | --- | --- |
| 封面 | ![蓝色系封面](review/style-galleries/blue-cover.png) | ![红色系封面](review/style-galleries/red-cover.png) | ![科技风格封面](review/style-galleries/tech-cover.png) |
| 正文组件 | ![蓝色系 16 个正文组件](review/style-galleries/blue-16.png) | ![红色系 16 个正文组件](review/style-galleries/red-16.png) | ![科技风格 16 个正文组件](review/style-galleries/tech-16.png) |

[蓝红封面及内容视觉索引](review/视觉索引.html) · [科技风 85 页索引](review/深蓝科技风85页索引.html)

蓝红组件按 `style_family=legacy-blue-red` 处理，以 `theme=blue/red` 区分色系；科技风使用独立的 `style_family=deep-blue-tech`。绿色实验主题不进入常规选择。

## 资产规模与统计口径

以下数字按本次整理时 `main` 分支文件统计。**来源页位、候选记录、已验证记录与主题版本不能相加，也不等于可直接调用的版式数量。** 运行时应以当前提交的目录与组件记录为准。

| 口径 | 数量 | 来源与含义 |
| --- | ---: | --- |
| 来源页位 | 770 | `source-pages.json`；早期 611 页位是扩充前口径。 |
| 可编辑来源稿 | 6 份 | `sources/` 中的蓝、红、封面、科技风和蓝红补充稿。 |
| 候选组件 | 461 条 | `catalog.json`，包含尚未验收的候选。 |
| 分类已验证 | 205 条 | `classification_status=verified`；仍需检查具体输出能力。 |
| 其中正文组件 | 141 条 | 上述记录中排除封面、目录、章节页和封底。 |

组件可按需从来源页提取；登记了 `ready_source_by_theme` 的组件应优先使用已修整的可编辑单页。`source`、`red_source` 用于原稿追溯。来源页的显式色与图片不自动成为自由绘制时可用的颜色素材。

正文资产改造分支中，`body_component_contract` v2 指向可直接打开的 `body-*.pptx` 及对应的 `body-*-bindings.json`。这些组件文件已移除页标题、Logo 和公共装饰，保留原生正文及内部标题。配套技能优先读取这些正文文件，在装配时另加公共页眉。旧整页路径保留用于旧技能兼容和原稿追溯。

### 字体与文件体积

`sources/cover.pptx` 已移除原稿附带的嵌入字体文件，20 页可编辑形状和文字保留；封面预览按清理后的源稿重新导出。原始文件哈希保存在 `source-manifest.json` 的 `original_sha256`，当前 `sha256` 对应仓库内的轻量文件。其他来源稿和组件本来就没有嵌入字体，无需批量改写。

模板不依赖 PowerPoint 自动猜测系统默认字体。配套技能在任务副本中按 Windows、macOS、Linux 选择已安装的明确字体，并在出稿前检查资源；某台设备没有指定字体时应停止或调整配置，不能让软件静默替换后声称版面一致。知识库源稿直接打开时，个别原版标题会因不再携带旧字体而呈现为本机可用字体；实际视觉以当前预览及目标应用复核为准。

## 内容如何匹配组件

1. 先选整套风格与页面职责。封面、目录、章节页、封底严格按角色匹配；普通正文按已验收的结构与信息关系检索，不以原稿的业务名称锁定用途。
2. 从 [`catalog.json`](catalog.json)、[`relation-taxonomy.json`](relation-taxonomy.json) 和组件规则检查主题、分类、PPTX 支持、媒体、原生项数与 `verified_counts`。`search_label` 只用于排序。
3. 按 `bindings.json` 检查字段路径、字数、行数、行宽并试填；严格语义和数据组件另检查专用契约。不能删空固定项数，也不能借模板示例内容补业务事实。
4. 在 PowerPoint 中检查文字边界、图片、Logo、颜色及整稿节奏。候选命中和程序试填成功仍需最终视觉复核。

正文无合适组件时，由[技能](https://github.com/camillechi2018/Epoint-Presentation)按同一风格使用内置排版规则或受约束的自由编排，并单独记录页面来源。

## 长文案与变项数

[正文长文案容量表](review/body-longcopy-capacity.json)覆盖 117 个正文组件、189 个蓝红科技主题版本。`physical_max_cjk_chars` 是单框实测极限，`recommended_max_cjk_chars` 是参考值；组稿优先使用更严格的 `use_for_planning_cjk_chars`，拥挤字段还须遵守 `visual_safe_max_cjk_chars`。117 个正文组件已按登记的可调用字数完成签收，见[视觉复核记录](review/body-longcopy-visual-review.md)。真实文案仍须通过行宽、行数和整页渲染。

变项数只按**具体组件**的 `verified_counts` 开放。蓝红目录、科技目录各有自己的已验收范围；其他流程或清单的变项数原型，不因目录可变而自动开放。固定项数组件只接受已登记的原生数量。

## 能力边界

| 能力 | 当前规则 |
| --- | --- |
| 静态可编辑 PPTX | 主题、字段、项数与 PPTX 验收状态均适配后使用；草稿还须人工审阅。 |
| 长文案 | 按逐字段安全容量试填；超容量压力样例失败，不代表所有长文案均不可用。 |
| 跨色系变量换色 | 蓝红双版本不等于任意来源页都能换色；按组件专项状态判断。 |
| 动效与 HTML | 有内部原型；静态 PPTX 验收不代表这些能力已验收。 |
| 目录及其他变项数 | 按该组件的 `verified_counts` 使用，不作整库统一承诺。 |

## 文件导航

| 路径 | 内容 |
| --- | --- |
| [`source-pages.json`](source-pages.json)、[`sources/`](sources/) | 来源页索引与可编辑原稿。 |
| [`catalog.json`](catalog.json)、[`layouts/`](layouts/) | 候选组件、绑定、规则与 ready 单页。 |
| [`relation-taxonomy.json`](relation-taxonomy.json) | 信息关系及同义词索引。 |
| [`themes/`](themes/)、[`brand/`](brand/) | 主题变量与品牌素材。 |
| [`source-previews/`](source-previews/)、[`cover-images/`](cover-images/) | 来源页预览与封面图库。 |
| [`review/`](review/) | 容量、静态 PPTX 和专项修整的验收证据。 |
| [`knowledge-manifest.json`](knowledge-manifest.json) | 供技能校验下载内容的文件哈希清单。 |

知识库模板和品牌素材仍处于 `draft_pending_review`。本仓库的授权范围见 [LICENSE](LICENSE)；公开可读不表示获得再分发或商用授权。配套技能另见[技能仓库的 LICENSE](https://github.com/camillechi2018/Epoint-Presentation/blob/main/LICENSE)。
