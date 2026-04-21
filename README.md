# Seasonal influenza mRNA vaccine induces stronger innate immunity and comparable or better adaptive responses than licensed inactivated vaccines in non-human primates

This repository contains source code and processed microarray input data for transcriptomic analysis of non-human primates vaccinated with **mRNA**, **Vaxigrip**, or **Fluad** influenza vaccines.

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

```bash
git clone https://github.com/Lore-Lab-Vaccine-Immunology/flu_vaccines_nhp
cd flu_vaccines_nhp
quarto render src/gene_array_analysis.qmd
```

## License

All code in this repository is distributed under the GNU General Public License v3.0.
