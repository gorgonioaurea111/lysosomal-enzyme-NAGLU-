# Lysosomal Enzyme Analysis: NAGLU

## Student Information
* **Name:** Aurea, Gorgonio A.
* **Subject & Section:** Cellular and Molecular Biology, Section-B
* **Gene Symbol:** NAGLU
* **NCBI Protein Accession:** NP_000254 (alpha-N-acetylglucosaminidase precursor)
* **Date:** October 13, 2026

---

## Overview
This repository contains reproducible bioinformatics results analyzing the human **NAGLU** gene and its corresponding lysosomal enzyme using R and NCBI data.

* **NCBI Protein Record:** [NP_000254](https://www.ncbi.nlm.nih.gov/protein/NP_000254)
* **Normal Function:** NAGLU (alpha-N-acetylglucosaminidase) normally breaks down heparan sulfate inside lysosomes by hydrolyzing terminal N-acetyl-D-glucosamine residues.

---

## Figures

### Figure 1: Amino Acid Composition
<img width="2400" height="1350" alt="file_show" src="https://github.com/user-attachments/assets/9c923ef6-efac-4fcc-a49a-d5d4a56f35de" />

### Figure 2: Potential N-Glycosylation Motifs
<img width="2400" height="990" alt="file_show (1)" src="https://github.com/user-attachments/assets/8a9e9c03-698a-4b77-875c-2bc94d5bb5ad" />


---

## Review Questions & Answers

1. **What does your enzyme normally break down inside lysosomes?**
   * NAGLU normally breaks down **heparan sulfate** inside lysosomes by hydrolyzing terminal N-acetyl-D-glucosamine residues.

2. **What is the total length of your protein, and which amino acids are most common?**
   * The total length of the NAGLU protein is **743 amino acids**. 
   * The five most common amino acids are **Alanine (A)** (95 counts, 12.79%), **Leucine (L)** (87 counts, 11.71%), **Glycine (G)** (60 counts, 8.08%), **Valine (V)** (52 counts, 7.00%), and **Arginine (R)** (49 counts, 6.59%).

3. **How many potential N-glycosylation motifs did you find? Where are they located?**
   * We found **7 potential N-glycosylation motifs** ($N-X-S/T$ pattern where $X$ is not Proline).
   * They are located at positions: **261 (NVT)**, **272 (NCS)**, **435 (NST)**, **503 (NCS)**, **513 (NRS)**, **526 (NTS)**, and **532 (NRS)**.

4. **Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?**
   * Glycosylation is crucial for lysosomal enzymes because specific sugar tags (like mannose-6-phosphate) direct the enzymes safely to the lysosome. 
   * **No**, finding a sequence motif ($N-X-S/T$) only indicates a *potential* site and does not prove the protein is actually glycosylated in vivo.

5. **What could happen in the cell if your enzyme did not work properly?**
   * If NAGLU fails to work properly, heparan sulfate accumulates progressively inside the cell's lysosomes, leading to **Mucopolysaccharidosis type IIIB (MPS-IIIB)**, also known as **Sanfilippo syndrome B**, a severe lysosomal storage disorder.
