# PhD Application Templates

A collection of LaTeX templates for PhD applications in chemistry, materials science and engineering, and chemical and biological engineering. Includes an academic CV, statement of purpose, personal statement, and research statement, with English document templates and documentation in English and Chinese.

[中文说明](README.zh-CN.md)

### Motivation

Keep application documents in one place, reuse consistent layouts, and make it easier to tailor each document to a different program. The templates contain writing prompts and placeholders for your own experience.

### Quick start

1. Download this repository using **Code → Download ZIP**.
2. Upload a `.tex` file to a blank [Overleaf](https://www.overleaf.com/project) project and set it as the **Main document**.
3. Select **pdfLaTeX** as the compiler.
4. Replace the placeholders and compile. Follow the program's required language, prompt, and length limit.

| Document | Template |
| --- | --- |
| Academic CV | [cv.tex](cv.tex) |
| Statement of purpose | [sop.tex](sop.tex) |
| Personal / personal history statement | [personal-statement.tex](personal-statement.tex) |
| Research statement | [research-statement.tex](research-statement.tex) |

### Build locally

With a TeX distribution and `latexmk` installed:

```sh
latexmk -pdf cv.tex
```

Substitute the filename to build another document. Each file is self-contained.

### Preview

PDF previews are not included yet. Compile the selected file in Overleaf to preview it. The templates have passed static structure checks; PDF compilation and visual review remain unverified.

### Credits and license

README organization inspired by [sb2nov/resume](https://github.com/sb2nov/resume). Document layouts are adapted from my Overleaf projects; inherited CV credits are recorded in [ATTRIBUTION.txt](ATTRIBUTION.txt), with the upstream MIT notice in [LICENSE-sb2nov.txt](LICENSE-sb2nov.txt). No repository-wide license is declared for the remaining materials.

Keep personal drafts in `private/` (ignored by Git) or outside this public repository.
