# Cell Type Annotation - LIFR Skin Seurat Object

This README lists the assigned cell types for each cluster in the Seurat object, along with representative marker genes used for the annotation.

---
  
  ### Cluster-to-Cell Type Mapping and Marker Genes
  
  **Cluster 0: Naive CD4+ T cells**
  *Markers:* IL7R, TRAC, TRBC2, SELL, TCF7, LTB, LEF1, CD3E

**Cluster 1: Resting Dermal Fibroblasts**
  *Markers:* SFRP2, FBN1, WISP2, ELN, PI16, SLPI, PRG4

**Cluster 2: Adventitial Fibroblasts**
  *Markers:* APOD, C3, CFH, CXCL12, GPC3, EFEMP1, ADH1B

**Cluster 3: Myofibroblasts**
  *Markers:* POSTN, EDNRA, COL11A1, ASPN, F2RL2, CDH11

**Cluster 4: Cytotoxic NK/CD8+ T cells**
  *Markers:* PRF1, GNLY, GZMA, GZMB, NKG7, KLRD1, CX3CR1

**Cluster 5: Activated CD4+ T cells**
  *Markers:* CXCR4, CD69, IL32, CCL4, TNFAIP3, SLC2A3

**Cluster 6: Pericytes / SMCs**
  *Markers:* RGS5, STEAP4, NOTCH3, SYNPO2, MRVI1

**Cluster 7: Endothelial Cells**
  *Markers:* VWF, PLVAP, ADGRL4, CLDN5, ACKR1, SELE

**Cluster 8: Basal Keratinocytes**
  *Markers:* KRT14, KRT5, DSC3, KRT1, CASP14, LGALS7B

**Cluster 9: M2 Macrophages**
  *Markers:* C1QA, CD163, FOLR2, VSIG4, MRC1, LYVE1

**Cluster 10: Conventional Dendritic Cells (cDC2)**
  *Markers:* CD1C, FCER1A, CLEC10A, HLA-DQA1, HLA-DPB1

**Cluster 11: M1 Monocytes / Macrophages**
  *Markers:* S100A8, S100A9, FCN1, LILRA1, SERPINA1, HCK

**Cluster 12: Naive B cells**
  *Markers:* MS4A1, CD79A, IGHM, TCL1A, IGHD, CD37

**Cluster 13: Mast Cells**
  *Markers:* CPA3, TPSAB1, TPSB2, KIT, MS4A2, CMA1, HDC

**Cluster 14: Smooth Muscle Cells**
  *Markers:* MYH11, TAGLN, ACTA2, CNN1, PLN, RBPMS2

**Cluster 15: Peripheral Glial Cells**
  *Markers:* SOX10, CDH19, PCSK2, NRXN1, ERBB3, GFRA3

**Cluster 16: Cycling Cells**
  *Markers:* MKI67, TOP2A, TYMS, RRM2, TPX2, CCNB1

**Cluster 17: Plasma Cells**
  *Markers:* IGHG1, IGHG4, IGHA1, IGLC2, JCHAIN, IGKC

**Cluster 18: Naive CD8+ T cells**
  *Markers:* CD8B, LEF1, CCR7, TCF7, IL7R, CD3E

**Cluster 19: Low-quality / Debris**
  *Markers:* Metazoa-SRP, snoU13, U1, RD3L, pseudogenes

---
  
  Annotations were made using canonical markers and observed gene expression patterns within each cluster. This metadata column is stored as `celltype` in the Seurat object.
