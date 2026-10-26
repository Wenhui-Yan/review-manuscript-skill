# 论文审稿技能 · Manuscript Review Skill

为科研论文生成精炼、可定位的审稿意见。兼顾需要展开的核心科学问题、简短的方法建议和具体小错误，尤其适用于遥感与生态学稿件。

## 审稿方式

- 核实每条意见的页码和印刷行号；没有行号时使用图表编号或文字锚点。
- 少量核心问题展开，其余建议简短直接，不为凑条数制造问题。
- 明确指出变量误写、图号重复、公式符号和表格编号等实际错误。
- 检查正文是否已经回应疑问，区分确定错误与需要澄清的问题。
- 可参考用户提供的旧审稿意见，但不套用旧稿件的结论。
- 根据当前论文证据形成建议，不预设“大修”或“拒稿”。

## 安装

将本仓库下载或克隆到个人技能目录下的 `review-manuscript` 文件夹，使 `SKILL.md` 位于该文件夹根目录。

默认个人技能目录为 `~/.codex/skills`；如果设置了 `CODEX_HOME`，则使用其下的 `skills` 目录。

```text
skills/
└── review-manuscript/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

## 使用

附上论文，以及可选的补充材料和审稿风格示例，然后输入：

```text
请用 $review-manuscript 审稿，定位到页码和行号。
核心建议适当展开，也指出具体小错误，整体不要冗长。
如果提供了审稿示例，请参考其风格。
```

通常使用少量展开的核心意见，搭配简短问题和具体更正；意见条数与篇幅按稿件调整。语言、推荐结论和交付格式均可在请求中指定。

## 内容与边界

本仓库包含技能指令和调用元数据，不包含论文、审稿实例或账户凭据。技能本身不提交审稿意见，也不上传未发表的稿件。使用者应遵守适用的期刊保密要求及 AI 使用政策，并核查最终意见。

## English

A reusable manuscript-review skill that produces concise, evidence-based peer-review reports with verified page and line references. It combines a few developed scientific concerns with short methodological questions and specific minor corrections. Prior review examples can guide tone and layout without carrying over their findings or recommendations.

The review workflow is defined in [SKILL.md](SKILL.md). UI metadata is in [agents/openai.yaml](agents/openai.yaml).
