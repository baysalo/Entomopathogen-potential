# Universal Entomopathogenic Virulence Screening Pipeline

## Overview
This repository contains a versatile R-based pipeline designed for the **in silico screening of bacterial virulence factors**. It is optimized for analyzing entomopathogenic bacteria (e.g., *Bacillus*, *Serratia*, *Pseudomonas*) against insect host targets.

The tool processes BLAST homology data to identify, visualize, and statistically analyze potential insecticidal proteins, making it suitable for genomic mining projects.

## Key Features
* **Automated Visualization:** Generates publication-ready figures (Bar charts, Violin plots, Heatmaps).
* **Interaction Modeling:** Creates bipartite network graphs modeling Host-Pathogen interactions.
* **Deep Homology Scanning:** dedicated module for identifying distant homologs (15-45% identity) to find novel variant candidates.
* **Universal Compatibility:** Works with standard BLAST output formats (CSV).

## Repository Structure
* `data/`: Place your raw BLAST output files here (CSV format).
* `results/`: The pipeline automatically saves all figures and stats here.
* `Universal_Virulence_Pipeline.R`: The main analysis script.

## How to Use
1.  Clone this repository.
2.  Place your BLAST CSV files into the `data/` folder.
    * *Note: Update the filenames in the "Load Datasets" section of the script if they differ.*
3.  Open `Universal_Virulence_Pipeline.R` in RStudio.
4.  Run the script.
5.  Check the `results/` folder for your generated figures.

## Dependencies
The script automatically installs missing packages upon first run:
* R (>= 4.0.0)
* ggplot2
* dplyr
* igraph
* ggrepel
* viridis

## Author
Ömür BAYSAL Ph.D.
Professor in Molecular Biology and Genetics /Molecular Microbiology Unit 

[Mugla Sitki Kocman University, University of Worcester]
