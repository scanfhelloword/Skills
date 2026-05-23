# arch-diagram — 论文架构图
## 功能
根据论文方法描述生成顶会风格学术架构图。含中英文双版 Prompt，建议都尝试取最优。

## 自动触发场景
- 用户要求生成论文架构图
- 提到"画架构图"、"架构图"、"architecture diagram"、"paper figure"、"illustration for my method"

## 需要收集的信息
- 用户的【论文摘要 + 方法部分描述】

## 输出
- 架构图生成 Prompt（含完整视觉约束）

## 特别提示
- 使用 nano banana 等图像模型时，英文版 Prompt 效果更佳

## 后续建议
- 生成架构图后，用 `/fig-caption` 为图写标题
- 如需为实验数据选择图表类型，使用 `/plot-recommend`
