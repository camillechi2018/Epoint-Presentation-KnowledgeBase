# content-blue-233

来源：blue P233。原生结构保留，可编辑。

## 结构复用契约

- 通用结构：`process`；已验证项数：`3`、`4`、`5`、`6`。
- 按结构、项数、字段容量和字段完整性选择；不要求匹配来源页的业务主题。
- `semantic_path` 仅作可编辑槽位地址，不代表业务语义约束；正文文字字段不设置 `semantic_role`。
- 页标题、Logo、下划线由技能处理，不计入本组件内容验收。
- 蓝红主题仅验证了短文案填充；资产仍为 `draft_pending_review`。

正文总宽保持原五项版的左右边界，按项数调整每列宽度。保留原卡片间距，六项新增卡片位于收尾卡片之前。

各项数的实测容量如下。双段字段以换行分隔，每段独立校验。

### 3 项

- `title` 7 字
- `tag_a` 6 字
- `tag_b` 6 字
- `summary` 64 字
- `goal_label` 6 字
- `action_label` 6 字
- `goal` 2 段，每段 33 字

### 4 项

- `title` 7 字
- `tag_a` 6 字
- `tag_b` 6 字
- `summary` 52 字
- `goal_label` 6 字
- `action_label` 6 字
- `goal` 2 段，每段 26 字

### 5 项

- `title` 7 字
- `tag_a` 6 字
- `tag_b` 6 字
- `summary` 42 字
- `goal_label` 6 字
- `action_label` 6 字
- `goal` 2 段，每段 22 字

### 6 项

- `title` 6 字
- `tag_a` 5 字
- `tag_b` 5 字
- `summary` 36 字
- `goal_label` 5 字
- `action_label` 5 字
- `goal` 2 段，每段 18 字
