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

Analysis was performed using R version 4.5.0 (2025-04-11), Platform: x86_64-apple-darwin20, Running under: macOS Sonoma 14.7.6. Attached package versions are described below:

```
attached packages:
 [1] dplyr_1.1.4            org.Mmu.eg.db_3.19.1   AnnotationDbi_1.66.0  
 [4] IRanges_2.38.1         S4Vectors_0.42.1       Biobase_2.64.0        
 [7] BiocGenerics_0.50.0    clusterProfiler_4.12.6 KEGGREST_1.44.1       
[10] pheatmap_1.0.12        eulerr_7.0.2           UpSetR_1.4.0          
[13] EnhancedVolcano_1.22.0 ggrepel_0.9.6          ggsci_3.2.0           
[16] gridExtra_2.3          limma_3.60.6           wesanderson_0.3.7     
[19] RColorBrewer_1.1-3     gplots_3.2.0           factoextra_1.0.7      
[22] ggplot2_3.5.2          matrixStats_1.5.0   
```

```bash
git clone https://github.com/Lore-Lab-Vaccine-Immunology/flu_vaccines_nhp
cd flu_vaccines_nhp
quarto render src/gene_array_analysis.qmd
```

## License

All code in this repository is distributed under the GNU General Public License v3.0.
