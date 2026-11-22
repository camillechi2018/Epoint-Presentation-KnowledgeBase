# content-blue-046

来源：blue P046。原生结构保留，可编辑。

## 结构复用契约

- 通用结构：`comparison`；已验证项数：`3`、`4`。
- 按结构、项数、字段容量和字段完整性选择；不要求匹配来源页的业务主题。
- `semantic_path` 仅作可编辑槽位地址，不代表业务语义约束；正文文字字段不设置 `semantic_role`。
- 页标题、Logo、下划线由技能处理，不计入本组件内容验收。
- 蓝红主题仅验证了短文案填充；资产仍为 `draft_pending_review`。

正文维持原四项版的总宽和列间距，三项版拉宽各列并重排分隔线。

各项数的实测容量如下。双段字段以换行分隔，每段独立校验。

### 3 项

- `category` 12 字
- `challenge_title` 12 字
- `solution_title` 12 字
- `challenge_body` 2 段，每段 35 字
- `solution_body` 2 段，每段 35 字

### 4 项

- `category` 8 字
- `challenge_title` 9 字
- `solution_title` 9 字
- `challenge_body` 2 段，每段 23 字
- `solution_body` 2 段，每段 23 字

技能根据已验收项数读取相应的纯正文绑定，并用原版重排规则装配正文。另一组原生字段见[固定结构](body-fixed-spec.md)。
