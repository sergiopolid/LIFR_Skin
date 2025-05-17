
# Restoring R Environment for LIFR_Skin Project

This file describes how to restore the R session used for analyzing LIFR/LIF expression.

---
  
  ## 📦 Required Libraries
  
  Make sure these libraries are installed:
  
  ```r
library(Seurat)
library(dplyr)
library(data.table)
library(ggplot2)
library(patchwork)
library(Cairo)
library(ggrepel)


setwd("/n/data1/bwh/medicine/rosas/Projects/LIFRSkin")
load("results/LIFR_Skin_environment.RData")

   ##🗂 File Reference

results/LIFR_Skin_environment.RData: The full saved R session
scripts/Step3_LIF_LIFR_expression.Rmd: Contains all commands for expression and visualization
figures/: Directory where all final .pdf visualizations are saved

