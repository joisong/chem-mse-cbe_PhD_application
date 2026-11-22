# PhD application templates — Chemistry, MSE & CBE

Reusable LaTeX templates adapted from my Overleaf application layouts for chemistry, materials science and engineering, and chemical and biological engineering PhD applications.

| File | Purpose |
| --- | --- |
| `cv.tex` | Academic CV: education, research, publications, presentations, awards, teaching, and skills |
| `sop.tex` | Statement of purpose: preparation, research interests, program fit, and goals |
| `personal-statement.tex` | Personal or personal history statement: experiences, growth, and community contributions |
| `research-statement.tex` | Research statement or project summary: questions, methods, individual contributions, results, and future directions |

## Use in Overleaf

1. Download the desired `.tex` file and upload it into a blank Overleaf project.
2. Set that file as the Main document and select **pdfLaTeX** as the compiler.
3. Replace all bracketed writing prompts and generic header fields.
4. Compile, review the PDF, and tailor it to each program's current prompt and length requirements.

Each template is self-contained. You can also upload all four files into one project and switch the Main document before compiling. No images, custom class files, or bibliography files are required.

## Compile locally

With a TeX distribution and `latexmk` installed:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error cv.tex
latexmk -pdf -interaction=nonstopmode -halt-on-error sop.tex
latexmk -pdf -interaction=nonstopmode -halt-on-error personal-statement.tex
latexmk -pdf -interaction=nonstopmode -halt-on-error research-statement.tex
```

Clean generated files with `latexmk -c`. The included `.gitignore` excludes build products and a `private/` directory for personal drafts.

## Tailoring checklist

- Follow the exact institutional prompt: SOP, personal statement, and research statement have different purposes.
- Replace university, program, applicant, dates, and all placeholders.
- State your individual contribution and distinguish goals from achieved results.
- Keep publication status, quantitative claims, dates, and terminology consistent across documents.
- Check current faculty affiliations and program requirements.
- Review page breaks, header spacing, hyperlinks, symbols, and PDF text extraction.
- Keep personal drafts and confidential or unpublished material outside this public repository.

## Source and attribution

Adapted from four projects in my supplied Overleaf tag: `26fall_phdapplication_cv (Copy)`, `sop_ucb`, `phs_ucb`, and `research statement nw (Copy)`. The original research file is a project-summary layout; the reusable version adds an optional future-direction block.

These are placeholder templates, not copies of completed applications. Source drafts contained differing publication statuses and scientific details; those claims have not been carried into the templates. See `ATTRIBUTION.txt` for inherited CV credits. No repository-wide license is asserted here for third-party source material.
