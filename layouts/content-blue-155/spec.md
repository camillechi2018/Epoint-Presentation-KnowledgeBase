# content-blue-155

来源：blue P155。原生结构保留，可编辑。

## 结构复用契约

- 通用结构：`parallel-points`；已验证项数：`3`、`4`、`5`、`6`。
- 按结构、项数、字段容量和字段完整性选择；不要求匹配来源页的业务主题。
- `semantic_path` 仅作可编辑槽位地址，不代表业务语义约束；正文文字字段不设置 `semantic_role`。
- 页标题、Logo、下划线由技能处理，不计入本组件内容验收。
- 蓝红主题仅验证了短文案填充；资产仍为 `draft_pending_review`。

正文总宽保持原五项版的左右边界，按项数调整每列宽度。弧线段数和分隔线位置随列数变化。

各项数的实测容量如下。正文以一段输入，由 PowerPoint 按列宽换行。

### 3 项

- `title` 6 字
- `goal_label` 4 字
- `plan_label` 4 字
- `goal_body` 60 字
- `plan_body` 72 字

### 4 项

- `title` 6 字
- `goal_label` 4 字
- `plan_label` 4 字
- `goal_body` 44 字
- `plan_body` 52 字

### 5 项

- `title` 6 字
- `goal_label` 4 字
- `plan_label` 4 字
- `goal_body` 36 字
- `plan_body` 44 字

### 6 项

- `title` 6 字
- `goal_label` 4 字
- `plan_label` 4 字
- `goal_body` 32 字
- `plan_body` 40 字

技能根据已验收项数读取相应的纯正文绑定，并用原版重排规则装配正文。另一组原生字段见[固定结构](body-fixed-spec.md)。
