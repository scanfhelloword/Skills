# zh2en-word — 中转英 Word 翻译
## 功能
将中文草稿翻译并润色为适合 Word 编辑的英文学术论文片段。输出纯文本，不含任何 Markdown 格式，可直接粘贴到 Word。

## 自动触发场景
- 用户提供中文并要求翻译成英文用于 Word
- 提到"Word 翻译"、"翻译成英文（Word）"、"translate for Word"
- 用户明确说输出要用于 Word、不要 Markdown 格式

## 需要收集的信息
- 用户的【中文草稿】

## 输出
- Part 1: 纯文本英文（无 Markdown，无 LaTeX 转义）
- Part 2: 中文直译

## 后续建议
- 如需 LaTeX 格式，使用 `/zh2en-latex`
- 翻译后可用 `/polish-en` 深度润色
