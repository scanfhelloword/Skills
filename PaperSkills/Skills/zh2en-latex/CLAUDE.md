# zh2en-latex — 中转英 LaTeX 翻译
## 功能
将用户提供的中文草稿翻译并润色为符合顶级会议标准的英文 LaTeX 学术论文片段。

## 自动触发场景
当用户出现以下行为时，应自动调用此 Skill：
- 提供中文文本并要求翻译成英文用于论文写作
- 提到"翻译成英文"、"translate to English for my paper"、"write this in English for my paper"、"中转英"、"LaTeX 翻译"
- 粘贴中文内容并要求 LaTeX 格式输出
- 说"帮我把这段中文写成英文论文"

## 需要收集的信息
- 用户的【中文草稿】

## 输出
- Part 1: 英文 LaTeX 代码（已转义特殊字符）
- Part 2: 中文直译（供核对）

## 后续建议
- 翻译完成后，可用 `/en2zh-latex` 反向翻译核对准确性
- 之后建议使用 `/polish-en` 进行深度润色
- 如果内容涉及 Word 排版，建议用户使用 `/zh2en-word`
- 翻译后可用 `/logic-check` 检查逻辑一致性
- 如果翻译结果有 AI 味，建议使用 `/deai-en`
- 终稿前建议使用 `/reviewer` 进行模拟审稿
