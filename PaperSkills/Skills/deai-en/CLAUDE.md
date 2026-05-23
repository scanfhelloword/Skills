# deai-en — 去 AI 味（LaTeX 英文）
## 功能
将 AI 生成的机械化英文文本重写为符合顶会标准的自然学术表达。

## 自动触发场景
- 用户说文本听起来像 AI 写的、太机械
- 提到"去AI味"、"去 AI 味"、"de-AI"、"humanize"、"machine-like"、"too robotic"、"doesn't sound human"、"rewrite to sound natural"

## 需要收集的信息
- 用户的【英文 LaTeX 代码片段】

## 输出
- Part 1: 重写后 LaTeX（或原文）
- Part 2: 中文直译
- Part 3: 修改日志或通过检测

## 后续建议
- 若原文已自然，会直接通过检测
- 之后可用 `/polish-en` 进一步润色
- 如果是中文文本需要去 AI 味，使用 `/deai-zh`
