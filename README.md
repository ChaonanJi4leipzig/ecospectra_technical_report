# Sentinel-2 Trait-Centered RSE Methods Manuscript

Manuscript draft for a Remote Sensing of Environment methods paper on trait-centered Sentinel-2 time-series learning from sparse hyperspectral labels.

The central claim is methodological: predicting forest functional traits from Sentinel-2 time series requires explicit treatment of temporal representation, auxiliary information, and temporal/spatial generalization.

Primary source files:

- `main.tex`
- `ecospectra_reference.bib`
- `Figure*_*.png`

Current figure set:

- `Figure1_trait_centered_framework.pdf`: trait-centered methods schematic
- `Figure2_study_site_map.png`: European retained-site and filtered-cohort map
- `Figure3_reintegrated_performance_heatmap.png`: five-trait baseline accuracy
- `Figure5_sample_size_curve.png`: sample-size ablation
- `Figure6_temporal_window_curve.png`: temporal-window ablation
- `Figure5_era5_barplot.png`: ERA5 auxiliary-information ablation
- `Figure7_temporal_generalization_heatmap.png`: cross-year transfer
- `Figure8_spatial_generalization_heatmap.png`: cross-site transfer

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
