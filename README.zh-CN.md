# 博士申请文书模板：化学、材料与化工方向

根据我在 Overleaf 中的申请文书排版整理，提供英文和中文两套可复用 LaTeX 模板。所有正文均为写作提示与占位内容，需要替换成申请人自己的真实经历。

| 文书 | 英文模板 | 中文模板 | 内容重点 |
| --- | --- | --- | --- |
| 学术简历 CV | `cv.tex` | `cv-zh.tex` | 教育、研究、论文、会议、奖励及技能 |
| 研究目的陈述 SOP | `sop.tex` | `sop-zh.tex` | 科研准备、研究方向、项目契合与职业目标 |
| 个人陈述 PS／PHS | `personal-statement.tex` | `personal-statement-zh.tex` | 成长经历、个人选择、合作与社区贡献 |
| 研究陈述 | `research-statement.tex` | `research-statement-zh.tex` | 研究问题、方法、个人贡献、成果与未来方向 |

## 在 Overleaf 中使用

1. 下载所需的 `.tex` 文件，上传至一个空白 Overleaf 项目。
2. 在项目设置中将该文件设为 Main document（主文档）。
3. **中文模板选择 XeLaTeX；英文模板选择 pdfLaTeX。** 中文使用 TeX 发行版中的 Fandol 字体，不依赖本机中文字体。
4. 替换页眉中的姓名、院校、专业、入学年份及正文中的全部占位内容。
5. 编译后逐页检查排版，遵守目标院校的题目、页数和字数要求。

每个模板均可独立使用，无需额外图片、类文件或参考文献文件。中文版本用于中文申请或构思；如果项目要求英文提交，请使用相应语言完成最终文书。

## 本地编译

安装包含中文支持及 Fandol 字体的 TeX 发行版和 latexmk 后运行：

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error cv-zh.tex
latexmk -xelatex -interaction=nonstopmode -halt-on-error sop-zh.tex
latexmk -xelatex -interaction=nonstopmode -halt-on-error personal-statement-zh.tex
latexmk -xelatex -interaction=nonstopmode -halt-on-error research-statement-zh.tex
```

用 `latexmk -c` 清理中间文件。`.gitignore` 已排除编译产物及 `private/` 私人草稿目录。

## 写作与提交检查

- 以学校的具体题目为准；PS、PHS、SOP 的名称和用途并非各校完全一致。
- 明确写出自己的工作，区分个人贡献、团队成果、研究目标与已实现结果。
- 核对所有材料中的时间、数字、术语、作者顺序和论文发表状态。
- 针对每个项目重写契合段落，核实导师信息与招生要求。
- 检查页眉是否重叠、跨页是否自然、链接与数学符号是否正常。
- 本仓库为公开模板；私人文书、个人联系方式和未公开研究内容请单独保存。

## 来源与说明

英文版排版来自所提供 Overleaf 标签中的 CV、SOP、PHS 与研究项目总结；中文版沿用其内容结构，并采用支持中文的 `ctexart` 排版。原始研究文件属于项目总结，因此模板另加了可选的未来研究方向。

原始完整申请中的个人经历、具体数值与发表状态未写入这些通用模板。CV 的来源署名见 `ATTRIBUTION.txt`。本仓库未为第三方来源材料统一声明许可证。

验证范围：已检查 LaTeX 环境与花括号配对；当前环境未安装编译器，尚未完成 PDF 编译与视觉校验。
