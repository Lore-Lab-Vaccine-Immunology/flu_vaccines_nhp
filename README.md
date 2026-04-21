# Seasonal influenza mRNA vaccine induces stronger innate immunity and comparable or better adaptive responses than licensed inactivated vaccines in non-human primates

This repository contains source code and processed microarray input data for transcriptomic analysis of non-human primates vaccinated with **mRNA**, **Vaxigrip**, or **Fluad** influenza vaccines.

## Table of contents
* [General information](#general-information)
* [Repository structure](#repository-structure)
* [Reproducibility](#reproducibility)
* [License](#license)

## General information

The main analysis is implemented in `src/gene_array_analysis.qmd`. The workflow loads files from `data/`, performs preprocessing, PCA, differential expression analysis, and pathway-level summaries.

## Repository structure

- `src/`: analysis source files and rendered report.
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
