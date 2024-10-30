# **Analysis-COVID-19**
> *Phylogenetic analysis and nucleotide sequence comparison of SARS-CoV-2 and related coronaviruses.*

## **Introduction**
This project conducts a comparative phylogenetic analysis of SARS-CoV-2 alongside other human coronaviruses. It examines nucleotide sequence patterns and evolutionary relationships, aiming to provide insights into genetic similarities and variations among these viruses. By understanding these relationships, the project seeks to highlight characteristics potentially associated with virus transmission and infection in humans.

## **Project Description**
- **Main functionality:** 
   - Comparative analysis of nucleotide sequences from SARS-CoV-2 and similar viruses.
   - Phylogenetic tree generation to illustrate evolutionary relationships among different coronaviruses.
- **Technologies used:** 
   - R programming language, `Biostrings`, `ggtree`, `DECIPHER`, `adegenet`, `seqinr` libraries for sequence alignment and analysis.
- **Challenges faced:** 
   - Handling and aligning diverse viral genome sequences with varying lengths and mutations.
- **Future improvements:** 
   - Incorporate additional virus samples for a broader phylogenetic comparison.
   - Automate sequence updates as new virus strains are identified.

## **Table of Contents**
1. [Introduction](#introduction)
2. [Project Description](#project-description)
3. [Installation](#installation)
4. [Usage](#usage)
5. [License](#license)

## **Installation**
1. **Prerequisites**:
   - **R** - [Download and install R](https://cran.r-project.org/)
   - **RStudio** (optional, recommended for an enhanced R experience) - [Download and install RStudio](https://rstudio.com/)
   - **BiocManager** for managing Bioconductor packages.
   
2. **Clone the repository**:
   ```bash
   git clone https://github.com/ivmg5/Analysis-COVID-19.git
   cd Analysis-COVID-19
   ```

3. **Install dependencies**:
   Open R and install the required libraries with the following code:
   ```r
   if (!require("BiocManager", quietly = TRUE)) install.packages("BiocManager")
   BiocManager::install(c("Biostrings", "ggtree", "DECIPHER", "ggmsa"))
   install.packages(c("seqinr", "ape", "phytools", "viridis", "ggplot2", "adegenet"))
   ```

4. **Set working directory**:
   - Ensure that the working directory is set to the project folder:
   ```r
   setwd("/path/to/Analysis-COVID-19")
   ```

### **Configuration Options**
- For further customization, modify environment variables within the `.Rmd` file, such as file paths and specific sequences to analyze.

## **Usage**
1. **Run the main analysis script (`main.Rmd`)**:
   - Open `main.Rmd` in RStudio or your preferred R environment.
   - Execute each code chunk to perform nucleotide sequence analysis, alignment, and generate visualizations.

2. **Example usage**:
   - Reading sequences:
     ```r
     virus_sequences <- read.GenBank(c("JX869059", "AY508724", "MN908947", ...))
     ```
   - Generating a phylogenetic tree:
     ```r
     distance_matrix <- dist.alignment(virus_aligned, matrix = "similarity")
     phylo_tree <- nj(distance_matrix)
     ladderized_tree <- ladderize(phylo_tree)
     phylo_plot <- ggtree(ladderized_tree) + geom_tiplab()
     phylo_plot
     ```

3. **Interpret results**:
   - The project outputs include nucleotide sequence comparisons and a phylogenetic tree. Interpret these visuals to assess genetic similarity and evolutionary proximity among viruses.

## **License**
This project is licensed under the MIT License.

[![Build Status](https://img.shields.io/badge/status-active-brightgreen)](#)
[![Code Coverage](https://img.shields.io/badge/coverage-80%25-yellowgreen)](#)
