# LIFR_Skin

Single-cell RNA-seq analysis of skin samples from systemic sclerosis (SSc) and healthy control patients. This repository includes preprocessing, quality control, metadata annotation, normalization, clustering, and differential gene expression analysis.

---

## 📁 Project Structure

```text
.
├── data/                        # Raw metadata tables (ignored by git)
├── figures/                    # Generated plots and figures
├── results/                    # Saved Seurat objects and intermediate files
├── scripts/                    # R scripts and RMarkdowns for each step
├── LIFR_Skin.Rproj             # R project file
├── README.md                   # Project README (this file)
└── step1_LIFR.Rmd              # RMarkdown pipeline for preprocessing and QC
```

---

## 🧪 Requirements

- R version ≥ 4.2
- Key packages: `Seurat`, `data.table`, `dplyr`, `future`, `ggplot2`

Install dependencies (if not already):

```r
install.packages(c("Seurat", "data.table", "dplyr", "future", "ggplot2"))
```

---

## 📊 Data Files and Their Purpose

| File                                  | Description                                                                 |
|---------------------------------------|-----------------------------------------------------------------------------|
| `results/combined_seurat.rds`         | Initial merged Seurat object (all cells, all conditions)                    |
| `results/combined_annotated_seurat.rds` | Merged Seurat object with metadata annotations added                       |
| `results/combined_qc_seurat.rds`      | After QC, normalization, PCA, UMAP                                          |
| `results/combined_control_ssc_only.rds`| Subset of only Control and SSc cells (filtered object)                      |
| `results/staged_merge/group_0X.rds`   | Intermediate files from stepwise merging of subsets                         |
| `results/markers_allclusters.csv`     | Output of `FindAllMarkers` on clusters from final UMAP                      |

---

## 🧬 How to Run

Open R or RStudio, load the R project, and run:

```r
rmarkdown::render("step1_LIFR.Rmd")
```

This will:
- Load and merge raw count files
- Annotate metadata
- Filter low-quality cells
- Normalize and scale data
- Run PCA, clustering, and UMAP
- Save intermediate `.rds` files for later use

---

## 📂 Git Ignore

The following folders are ignored via `.gitignore`:
```
GSE195452_RAW/
```
To keep the repo lightweight.

---

## 📬 Questions?
Contact [Sergio Poli De Frias, MD](https://github.com/sergiopolid) or open an issue on this repo.
