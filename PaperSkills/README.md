# PaperSkills

学术论文写作辅助工具集 — 17 个 Claude Code Skill，覆盖翻译、润色、去 AI 味、图表生成、实验分析、审稿等全流程。

## 来源

本项目将 [Leey21/awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) 中的论文优化模板封装为 Claude Code Skill，原始核心内容归原作者 Leey21 所有，本人仅做封装适配。

## 使用方式

| 方式 | 操作 | 适用场景 |
|------|------|----------|
| **Claude Code Skill** | 输入 `/<skill-name>` 或自然描述自动触发 | Claude Code 内交互 |
| **Prompt 模板** | 复制 `00prompts/` 中的内容到任意 LLM | 独立使用，无需 Claude Code |

## Skill 列表

| 分类 | Skill | 功能 | Prompt |
|------|-------|------|--------|
| 翻译 | `/zh2en-latex` | 中文草稿 → 英文 LaTeX | [>>](00prompts/01-中转英-latex.md) |
| 翻译 | `/en2zh-latex` | 英文 LaTeX → 中文直译 | [>>](00prompts/02-英转中-latex.md) |
| 翻译 | `/zh2en-word` | 中文草稿 → 英文 Word | [>>](00prompts/03-中转英-word.md) |
| 润色 | `/polish-en` | 英文 LaTeX 深度润色 | [>>](00prompts/07-表达润色-英文.md) |
| 润色 | `/polish-zh` | 中文论文段落润色 | [>>](00prompts/08-表达润色-中文.md) |
| 润色 | `/zh2zh-word` | 口语 → 书面学术中文 | [>>](00prompts/04-中转中-word.md) |
| 编辑 | `/shorten` | 英文缩写（约 5-15 词） | [>>](00prompts/05-英文缩写.md) |
| 编辑 | `/expand` | 英文扩写（约 5-15 词） | [>>](00prompts/06-英文扩写.md) |
| 去AI味 | `/deai-en` | 机械化英文 → 自然学术表达 | [>>](00prompts/10-去AI味-latex英文.md) |
| 去AI味 | `/deai-zh` | 翻译腔中文 → 自然学术中文 | [>>](00prompts/11-去AI味-word中文.md) |
| 校对 | `/logic-check` | 终稿逻辑红线审查 | [>>](00prompts/09-逻辑检查英文.md) |
| 图表 | `/arch-diagram` | 生成顶会风格论文架构图 | [>>](00prompts/12-论文架构图.md) |
| 图表 | `/plot-recommend` | 实验数据 → 图表类型推荐 | [>>](00prompts/13-实验绘图推荐.md) |
| 图表 | `/fig-caption` | 中文描述 → 英文 Figure Caption | [>>](00prompts/14-生成图标题.md) |
| 图表 | `/tab-caption` | 中文描述 → 英文 Table Caption | [>>](00prompts/15-生成表标题.md) |
| 分析 | `/exp-analysis` | 实验数据 → LaTeX 分析段落 | [>>](00prompts/16-实验分析.md) |
| 审稿 | `/reviewer` | Reviewer 视角全面评估论文 | [>>](00prompts/17-reviewer审视.md) |

## 推荐工作流

| # | 链路 | 说明 |
|---|------|------|
| 1 | `/zh2en-latex` → `/polish-en` → `/reviewer` | 翻译 → 润色 → 审稿 |
| 2 | `/zh2en-latex` → `/deai-en` → `/reviewer` | 翻译 → 去AI味 → 审稿 |
| 3 | 写作 → `/logic-check` → `/reviewer` | 写作 → 逻辑检查 → 审稿 |
| 4 | `/exp-analysis` → `/plot-recommend` → `/fig-caption` + `/tab-caption` | 实验 → 分析 → 绘图 → 标题 |
| 5 | `/shorten` 或 `/expand` → `/logic-check` | 编辑 → 逻辑检查 |
| 6 | `/en2zh-latex` → `/zh2en-latex` | 英转中 → 反向核对 |
| 7 | `/zh2en-latex` → `/en2zh-latex` | 中转英 → 反向核对 |
| 8 | `/arch-diagram` → `/fig-caption` | 架构图 → 图标题 |

## 项目结构

```
├── CLAUDE.md              项目配置（自动触发 + 工作流）
├── README.md
├── 00prompts/              17 个 Prompt 模板（可复制到任意 LLM）
├── .claude/skills/         17 个 Skill 注册文件（Claude Code 自动发现）
├── zh2en-latex/            每个 Skill 一个目录（共 17 个）
│   ├── skill.md            完整定义（角色、约束、输出格式、自查）
│   ├── CLAUDE.md           上下文（触发场景、输入、后续建议）
│   └── README.md           人类可读文档
└── ...
```

## 致谢与免责

- 原始论文优化模板归 [Leey21](https://github.com/Leey21/awesome-ai-research-writing) 所有，原项目地址：https://github.com/Leey21/awesome-ai-research-writing
- 本项目仅为 Skill 封装，未做实质性内容修改
- 本项目仅供个人学习与技术实践，不作商业用途
- 封装未获原作者明示授权，如有异议请联系删除
- 使用本项目产生的任何后果由使用者自行承担
