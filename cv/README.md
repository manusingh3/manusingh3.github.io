# CV Source

This directory contains the LaTeX source for Manu Singh Burson's CV.

## Workflow

1. **Edit** `cv.tex` with your latest updates.
2. **Compile** to PDF:
   ```bash
   cd cv
   pdflatex cv.tex
   pdflatex cv.tex   # run twice to resolve page references
   ```
3. **Copy** the compiled PDF to the site's files directory:
   ```bash
   cp cv.pdf ../files/cv.pdf
   ```
4. **Commit and push** — the site's CV page links to `/files/cv.pdf`.

## Requirements

The following LaTeX packages are required (all available in TeX Live / MiKTeX):

- `geometry`, `titlesec`, `tabularx`, `array`, `xcolor`
- `enumitem`, `fontawesome5`, `amsmath`, `hyperref`
- `eso-pic`, `calc`, `bookmark`, `lastpage`
- `changepage`, `paracol`, `ifthen`, `needspace`, `iftex`
- `sourcesanspro` (font)

Install on macOS with [MacTeX](https://www.tug.org/mactex/) or via Homebrew:
```bash
brew install --cask mactex
```
