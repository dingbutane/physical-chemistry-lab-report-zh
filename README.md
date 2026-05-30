# physical-chemistry-lab-report-zh

中文物理化学实验报告写作与排版工作流的 Codex skill。

这个 skill 用于处理从实验讲义、模板报告、原始数据、图表、文献值到 Word 终稿的完整流程。它特别适合中文物化实验报告：需要模仿已有模板、整理实验数据、用 matplotlib 制图、写数据讨论、回答思考题，并在 Word 中处理公式、斜体物理量、上下标和参考文献。

## What It Does

- 学习实验讲义和既有模板报告，保持标题、字体、表格、公式和图注风格一致。
- 整理原始数据，保留原始读数、平均值和必要的校正计算。
- 用 `matplotlib` 生成实验报告图表，如工作曲线、相图和文献对比图。
- 在 `.docx` 中插入或替换表格、图片、讨论段落、思考题和参考文献。
- 规范物理量格式，例如斜体 *T*、*p*、*x*、*y*，以及 `n₂`、`ΔT`、`10⁻⁴ °C⁻¹` 等上下标。
- 将报告转成 PDF 后检查图表、公式、分页和排版效果。

## When To Use

Use this skill when a user asks Codex to write, revise, format, or finish a Chinese physical chemistry lab report, especially when the task involves:

- 实验讲义和模板报告；
- Word `.docx` 报告；
- 原始数据图片或实验表格；
- 折射率、沸点、相图、校正公式等数据处理；
- NIST、标准相图或其他文献数据对比；
- 中文实验报告中的误差分析和思考题。

## Installation

Clone this repository into your Codex skills directory:

```powershell
git clone git@github.com:dingbutane/physical-chemistry-lab-report-zh.git `
  "$env:USERPROFILE\.codex\skills\physical-chemistry-lab-report-zh"
```

Or copy the folder manually so that the skill file is located at:

```text
%USERPROFILE%\.codex\skills\physical-chemistry-lab-report-zh\SKILL.md
```

Restart Codex or start a new session if the skill list does not refresh immediately.

## Typical Workflow

1. Locate the handout, templates, raw data, current report, and figures.
2. Learn the style from previous reports in `Templates`.
3. Extract and verify raw data before committing it to the report.
4. Process data with reproducible calculations.
5. Generate high-resolution PNG figures with `matplotlib`.
6. Edit the Word report while preserving user-adjusted formatting.
7. Use proper italics, subscripts, superscripts, and inline equations for physical quantities.
8. Compare experimental results with literature values where appropriate.
9. Polish the discussion so the error analysis is tied to the actual data.
10. Convert to PDF and inspect key pages before final delivery.

## Notes

- The skill is intentionally workflow-focused. It does not bundle a fixed report template because lab requirements and local formatting habits vary.
- External data, such as NIST boiling points or standard VLE tables, should be checked from current or primary sources and cited in the final report.
- For Word formulas, `python-docx` handles basic formatting, while more complex equations may require direct OMML insertion.

## License

No license has been selected yet. Add one before broad redistribution if needed.
