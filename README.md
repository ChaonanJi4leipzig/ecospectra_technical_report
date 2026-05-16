# EcoSpectra RSE Methods Manuscript

Fast-deliverable manuscript version for a Remote Sensing of Environment methods paper on trait-centered Sentinel-2 learning from sparse hyperspectral labels.

The central claim is methodological: predicting forest functional traits from Sentinel-2 time series requires explicit treatment of temporal representation, auxiliary information, and temporal/spatial generalization. This version reports validated EnMAP-based model results and specifies PRISMA as the next label-source ablation.

Primary source files:

- `main.tex`
- `ecospectra_reference.bib`
- `Figure*_*.png`

Current figure set:

- `Figure1_pipeline_architecture.png`: trait-centered workflow
- `Figure2_data_distribution.png`: labeled-sample distribution
- `Figure3_reintegrated_performance_heatmap.png`: five-trait baseline accuracy
- `Figure4_reintegrated_scatter.png`: baseline observed-vs-predicted diagnostics
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
