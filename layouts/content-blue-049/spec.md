# content-blue-049

来源：blue P049。原生结构保留，可编辑。

通用结构为 `comparison`。左右两侧逐行成对，项数按左右合计。4 项为左右各 2 项，6 项为左右各 3 项。四项版重新分配行距，两侧和中间图形的横向位置固定。

蓝红已验收 4、6 项。基于结构、项数和槽位容量自动选版。

固定正文槽位的实测容量

- `center.left` 4 字
- `center.right` 4 字
- `center.marker` 2 字
- `center.top` 8 字
- `center.bottom` 8 字
- `body.summary` 95 字

### 4 项

- `left_title` 7 字
- `left_body` 40 字
- `right_title` 7 字
- `right_body` 40 字

### 6 项

- `left_title` 7 字
- `left_body` 40 字
- `right_title` 7 字
- `right_body` 40 字

PowerPoint 蓝红容量稿和常规稿通过。资产状态为 `draft_pending_review`。

技能根据已验收项数读取相应的纯正文绑定，并用原版重排规则装配正文。另一组原生字段见[固定结构](body-fixed-spec.md)。
