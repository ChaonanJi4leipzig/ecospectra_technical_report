# EcoSpectra Technical Report

First technical-report draft for the EcoSpectra traits-model reintegrated-data gate and active experiments.

The LaTeX structure was initialized from `ecospectra_model_technical_report.zip` and the scientific content was replaced with the current EcoSpectra model-report content.

Primary source files:

- `main.tex`
- `ecospectra_reference.bib`
- `Figure*_*.png`
- `main.html` as a Pandoc parser/preview artifact when no local LaTeX engine is available

Build with a local LaTeX installation:

```bash
latexmk -pdf main.tex
```

If `latexmk` is unavailable:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```
