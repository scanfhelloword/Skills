# tab-caption — 生成表的标题
## 功能
将中文描述转化为符合顶级会议规范的英文表标题（Table Caption）。

## 自动触发场景
- 用户要求写表标题
- 提到"表标题"、"table caption"、"表格标题"、"写表注"

## 需要收集的信息
- 用户的【中文描述】

## 输出
- 英文表标题文本（无 Table 1: 前缀）

## 后续建议
- 推荐使用 Comparison with / Ablation study on / Results on 等句式
- 表标题完成后，如需图标题使用 `/fig-caption`
- 论文图表标题完成后，使用 `/reviewer` 进行终稿审稿
