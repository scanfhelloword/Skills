# PaperSkills — 学术论文写作 Prompt 集合

学术论文写作辅助 Prompt 合集，涵盖翻译、润色、去 AI 味、图表生成、实验分析、审稿等场景。

## 📑 Part I: 写作 Prompt 集合

| 编号 | 名称 | 说明 |
|------|------|------|
| 01 | [中转英-latex](01-中转英-latex.md) | 中文草稿 → 英文 LaTeX 学术片段 |
| 02 | [英转中-latex](02-英转中-latex.md) | 英文 LaTeX → 中文直译（快速理解论文） |
| 03 | [中转英-word](03-中转英-word.md) | 中文草稿 → 英文 Word 学术片段 |
| 04 | [中转中-word](04-中转中-word.md) | 中文草稿 → 中文 Word 学术段落（口语转书面语） |
| 05 | [英文缩写](05-英文缩写.md) | 英文 LaTeX 文本微幅缩减（约 5-15 词） |
| 06 | [英文扩写](06-英文扩写.md) | 英文 LaTeX 文本微幅扩写（约 5-15 词） |
| 07 | [表达润色-英文](07-表达润色-英文.md) | 英文 LaTeX 深度润色与重写 |
| 08 | [表达润色-中文](08-表达润色-中文.md) | 中文论文段落专业审视与润色 |
| 09 | [逻辑检查](09-逻辑检查英文.md) | 论文终稿红线审查（仅报致命错误） |
| 10 | [去AI味-latex](10-去AI味-latex英文.md) | 机械化英文 → 自然学术表达（附 AI 词汇黑名单） |
| 11 | [去AI味-word](11-去AI味-word中文.md) | 翻译腔中文 → 自然学术中文 |
| 12 | [论文架构图](12-论文架构图.md) | 根据方法描述生成顶会风格架构图（中英文双版） |
| 13 | [实验绘图推荐](13-实验绘图推荐.md) | 根据实验数据推荐最佳图表类型 |
| 14 | [生成图标题](14-生成图标题.md) | 中文描述 → 英文 Figure Caption |
| 15 | [生成表标题](15-生成表标题.md) | 中文描述 → 英文 Table Caption |
| 16 | [实验分析](16-实验分析.md) | 实验数据 → LaTeX 分析段落 |
| 17 | [Reviewer 审视](17-reviewer审视.md) | Reviewer 视角全面评估论文，含改稿策略建议 |

## 📑 Part II: Claude Code Skills

以上 17 个功能已封装为 Claude Code Skills，可通过 `/skill-name` 直接调用：

| 分类 | Skill |
|------|-------|
| 翻译 | `/zh2en-latex` `/en2zh-latex` `/zh2en-word` |
| 润色 | `/zh2zh-word` `/polish-en` `/polish-zh` |
| 编辑 | `/shorten` `/expand` |
| 去AI味 | `/deai-en` `/deai-zh` |
| 校对 | `/logic-check` |
| 图表 | `/arch-diagram` `/plot-recommend` `/fig-caption` `/tab-caption` |
| 分析 | `/exp-analysis` |
| 审稿 | `/reviewer` |

## 使用说明

- **Prompt 方式**：点击上方链接进入文件，复制完整 Prompt，粘贴到聊天框填入内容后发送
- **Skill 方式**：直接在 Claude Code 中输入 `/<skill-name>`，按提示提供输入内容
