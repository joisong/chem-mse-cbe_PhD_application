# 博士申请文书模板

面向化学、材料科学与工程、化学与生物工程方向的 LaTeX 博士申请模板，包含学术简历、SOP、个人陈述和研究陈述，文书模板为英文，使用说明提供中英文版本。

[English](README.md)

### 为什么整理这些模板

把申请材料集中管理，复用统一的排版，并方便针对不同院校修改。模板正文采用写作提示与占位内容，需要替换为自己的真实经历。

### 快速开始

1. 点击仓库的 **Code → Download ZIP** 下载文件。
2. 在 [Overleaf](https://www.overleaf.com/project) 中新建空白项目，上传所需 `.tex` 文件，并设为 **Main document**。
3. 将编译器设为 **pdfLaTeX**。
4. 替换占位内容后编译，按学校要求调整语言、题目和篇幅。

| 文书 | 英文模板 |
| --- | --- |
| 学术简历 CV | [cv.tex](cv.tex) |
| 研究目的陈述 SOP | [sop.tex](sop.tex) |
| 个人／个人经历陈述 PS、PHS | [personal-statement.tex](personal-statement.tex) |
| 研究陈述 | [research-statement.tex](research-statement.tex) |

### 本地编译

安装 TeX 发行版和 `latexmk` 后运行：

```sh
latexmk -pdf cv.tex
```

更换文件名即可编译其他文书。每个模板均可独立使用。

### 效果预览

暂未附上 PDF 预览，可在 Overleaf 中编译查看。当前已完成静态结构检查，尚未完成 PDF 编译和视觉校验。

### 来源与许可

README 的组织方式参考 [sb2nov/resume](https://github.com/sb2nov/resume)。文书排版来自我的 Overleaf 项目；CV 的原始署名见 [ATTRIBUTION.txt](ATTRIBUTION.txt)，上游 MIT 许可原文见 [LICENSE-sb2nov.txt](LICENSE-sb2nov.txt)。其余材料未统一声明仓库级许可证。

私人草稿请放入 Git 忽略的 `private/` 目录，或另行保存在公开仓库之外。
