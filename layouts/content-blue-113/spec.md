# content-blue-113

来源：blue P113。原生结构保留，可编辑。

## 结构复用契约

- 通用结构：`parallel-points`；已验证项数：`3`、`4`、`5`、`6`。
- 按结构、项数、字段容量和字段完整性选择；不要求匹配来源页的业务主题。
- `semantic_path` 仅作可编辑槽位地址，不代表业务语义约束；正文文字字段不设置 `semantic_role`。
- 页标题、Logo、下划线由技能处理，不计入本组件内容验收。
- 蓝红主题仅验证了短文案填充；资产仍为 `draft_pending_review`。

正文总宽保持原五项版的左右边界，按项数调整每列宽度。

各项数的实测容量如下。双段字段以换行分隔，每段独立校验。

### 3 项

- `footer_label` 8 字
- `circle_title` 6 字
- `first_title` 8 字
- `second_title` 8 字
- `first_body` 2 段，每段 24 字
- `second_body` 2 段，每段 24 字

### 4 项

- `footer_label` 8 字
- `circle_title` 6 字
- `first_title` 8 字
- `second_title` 8 字
- `first_body` 2 段，每段 18 字
- `second_body` 2 段，每段 18 字

### 5 项

- `footer_label` 8 字
- `circle_title` 6 字
- `first_title` 8 字
- `second_title` 8 字
- `first_body` 2 段，每段 14 字
- `second_body` 2 段，每段 14 字

### 6 项

- `circle_title` 5 字
- `footer_label` 7 字
- `first_title` 7 字
- `second_title` 7 字
- `first_body` 2 段，每段 12 字
- `second_body` 2 段，每段 12 字

技能根据已验收项数读取相应的纯正文绑定，并用原版重排规则装配正文。另一组原生字段见[固定结构](body-fixed-spec.md)。
