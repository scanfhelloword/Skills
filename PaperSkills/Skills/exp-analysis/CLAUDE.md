# exp-analysis — 实验分析
## 功能
从实验数据中挖掘关键趋势和对比结论，整理为 LaTeX 分析段落。

## 自动触发场景
- 用户提供实验数据并要求分析
- 提到"实验分析"、"分析实验数据"、"写实验段落"、"analyze results"、"experiment analysis"、"write up the results"

## 需要收集的信息
- 用户的【实验数据】

## 输出
- Part 1: LaTeX 分析段落（`\paragraph{}` 结构）
- Part 2: 中文直译

## 后续建议
- 分析完成后可用 `/polish-en` 润色
- 如需推荐图表类型，使用 `/plot-recommend`
- 分析中涉及的图表标题，使用 `/fig-caption` 或 `/tab-caption`
