# Seasonal influenza mRNA vaccine induces stronger innate immunity and comparable or better adaptive responses than licensed inactivated vaccines in non-human primates

This repository contains source code and processed microarray input data for transcriptomic analysis of non-human primates vaccinated with **mRNA**, **Vaxigrip**, or **Fluad** influenza vaccines.

DOI: [10.1038/s41541-026-01492-y](www.doi.org/10.1038/s41541-026-01492-y)
## Table of contents
* [General information](#general-information)
* [How to view the analysis](#how-to-view-the-analysis)
* [Repository structure](#repository-structure)
* [Reproducibility](#reproducibility)
* [License](#license)

## General information

The main analysis is implemented in `src/gene_array_analysis.qmd`. The workflow loads files from `data/`, performs preprocessing, PCA, differential expression analysis, and pathway-level summaries.

## How to view the analysis

The rendered HTML report is not versioned in this repository. To view the full analysis, render it locally from the Quarto source:

```bash
quarto render src/gene_array_analysis.qmd
```

Then open `src/gene_array_analysis.html` in your browser.

## Repository structure

- `src/`: analysis source files.
- `data/`: processed expression and annotation input files.
- `influenza_vaccine.Rproj`: RStudio project file.

## Reproducibility

Analysis was performed using R version 4.5.3 (2026-03-11), Platform: x86_64-apple-darwin20, Running under: macOS Sonoma 14.8.5.

[Click here to check the rendered analysis and R package versions](https://lore-lab-vaccine-immunology.github.io/flu_vaccines_nhp/src/gene_array_analysis.html).

```bash
git clone https://github.com/Lore-Lab-Vaccine-Immunology/flu_vaccines_nhp
cd flu_vaccines_nhp
quarto render src/gene_array_analysis.qmd
```

## License

All code in this repository is distributed under the GNU General Public License v3.0.
