
# Lysosomal Enzyme Analysis: NAGLU

**Bioinformatics Analysis of Human Alpha-N-Acetylglucosaminidase**

---

## 1. Student Information

- **Name:** Aurea, Gorgonio A.
- **Subject:** Cellular and Molecular Biology
- **Section:** B
- **Gene Symbol:** `NAGLU`
- **Enzyme Name:** Alpha-N-acetylglucosaminidase
- **NCBI Protein Accession:** `NP_000254.2`
- **NCBI Protein Record:** [NP_000254.2](https://www.ncbi.nlm.nih.gov/protein/NP_000254.2)
- **Repository Name:** `lysosomal-enzyme-NAGLU`
- **Date:** October 13, 2026

---

## 2. Introduction and Biological Function

NAGLU is the gene that encodes alpha-N-acetylglucosaminidase, a lysosomal enzyme involved in the degradation of heparan sulfate, a glycosaminoglycan found in the extracellular matrix and on cell surfaces.

The enzyme removes terminal alpha-N-acetylglucosamine residues during heparan sulfate degradation. Its proper function is important for lysosomal metabolism and cellular homeostasis.

Pathogenic variants in NAGLU can cause **mucopolysaccharidosis type IIIB (MPS IIIB), also known as Sanfilippo syndrome type B**. This lysosomal storage disorder results from impaired heparan sulfate degradation and its progressive accumulation.

This project uses R programming and NCBI protein sequence data to analyze the amino acid composition of NAGLU and identify potential N-linked glycosylation motifs.

## 3. Objectives

1. Retrieve the human NAGLU protein sequence from NCBI.
2. Determine the protein length and amino acid composition.
3. Identify potential N-linked glycosylation motifs using the N-X-S/T consensus sequence.
4. Generate figures showing amino acid composition and motif positions.
5. Interpret the findings in relation to protein characteristics and lysosomal function.
6. Document the analysis and results in a public GitHub repository.

---

## 4. Tools and Resources

- **NCBI Protein Database:** Protein sequence retrieval.
- **R and RStudio:** Sequence analysis and visualization.
- **rentrez:** Programmatic access to NCBI data, if used in the script.
- **ggplot2:** Data visualization, if used in the script.
- **GitHub:** Repository hosting and documentation.

---

## 5. R Script Workflow

### Step 1: Protein Sequence Retrieval

The human NAGLU protein sequence was obtained from the NCBI Protein database using accession `NP_000254.2`.

Reference: [NCBI Protein Record](https://www.ncbi.nlm.nih.gov/protein/NP_000254.2)

### Step 2: Sequence Processing

The protein sequence was loaded into R for analysis. The sequence was treated as a series of one-letter amino acid codes.

### Step 3: Amino Acid Composition

The sequence was analyzed to calculate the number of occurrences of each of the 20 standard amino acids. The results were used to determine the total protein length and the most abundant residues.

### Step 4: Potential N-Glycosylation Motif Detection

The sequence was scanned for the consensus pattern:

`N-X-S/T`

Where:
- **N** represents asparagine.
- **X** represents any amino acid except proline (`P`).
- **S/T** represents serine or threonine.

The positions of matching motifs were recorded for further analysis.

### Step 5: Data Visualization

Two figures were generated:

1. Amino acid composition bar plot.
2. Distribution of potential N-linked glycosylation motifs.

### Step 6: Results and Publication

The analysis outputs were organized into data, results, and figures folders. The R script and README were uploaded to GitHub to document the workflow and findings.

---

## 6. Results and Figure Interpretations

### Figure 1: Amino Acid Composition

<img width="2400" height="1350" alt="NAGLU_amino_acid_composition" src="https://github.com/user-attachments/assets/1f47d99b-7b15-48cf-9dcb-f22f9384d525" />


**Figure 1.** Distribution of amino acid residues in the NAGLU protein sequence.

#### Interpretation

The analysis reports a total protein length of **743 amino acids**.

The most abundant amino acid residues are:

| Amino Acid | One-Letter Code | Count | Percentage |
|---|---|---:|---:|
| Alanine | A | 95 | 12.79% |
| Leucine | L | 87 | 11.71% |
| Glycine | G | 60 | 8.08% |

Alanine is the most abundant residue, followed by leucine and glycine. Alanine and leucine can contribute to hydrophobic interactions and protein packing, while glycine can provide local flexibility because of its small side chain.

The graph illustrates the frequency of amino acid residues throughout the protein sequence. However, amino acid composition alone cannot establish the protein's three-dimensional structure or enzymatic activity.

### Figure 2: Potential N-Linked Glycosylation Motifs

<img width="2400" height="990" alt="NAGLU_potential_N_glycosylation" src="https://github.com/user-attachments/assets/1199f72a-49b8-4f94-b212-1b4791648ba7" />


**Figure 2.** Positions of potential N-linked glycosylation motifs along the NAGLU protein sequence.

#### Interpretation

The sequence analysis reports **seven potential N-linked glycosylation motifs**:

| Position | Motif Sequence |
|---:|---|
| 261 | NVT |
| 272 | NCS |
| 435 | NST |
| 503 | NCS |
| 513 | NRS |
| 526 | NTS |
| 532 | NRS |

These motifs occur at different positions along the protein sequence, with several located relatively close together in the middle and C-terminal regions.

N-linked glycosylation can contribute to protein folding, stability, quality control, and intracellular trafficking. Many lysosomal enzymes receive mannose-6-phosphate modifications on their N-linked oligosaccharides, helping direct them toward lysosomes.

**Important limitation:** N-X-S/T is a potential N-glycosylation motif, not confirmation of a glycan or a mannose-6-phosphate tag. Protein sequence analysis does not directly measure enzyme activity.

---

## 7. Review Questions and Answers

### Question 1: What does your enzyme normally break down inside lysosomes?

**Answer:**

NAGLU, or alpha-N-acetylglucosaminidase, participates in the degradation of heparan sulfate. It removes terminal alpha-N-acetylglucosamine residues during the lysosomal breakdown of this glycosaminoglycan.

### Question 2: What is the total length of your protein, and which amino acids are most common?

**Answer:**

The analyzed NAGLU precursor protein is reported to contain 743 amino acids. The most abundant residues are alanine (95 residues, 12.79%), leucine (87 residues, 11.71%), and glycine (60 residues, 8.08%).

### Question 3: How many potential N-glycosylation motifs did you find? Where are they located?

**Answer:**

Seven potential N-linked glycosylation motifs were identified at the following positions:

- Position 261: NVT
- Position 272: NCS
- Position 435: NST
- Position 503: NCS
- Position 513: NRS
- Position 526: NTS
- Position 532: NRS

These sequences match the N-X-S/T consensus pattern, where X is any amino acid except proline.

### Question 4: Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?

**Answer:**

Glycosylation can assist protein folding, stability, quality control, and intracellular trafficking. Many lysosomal enzymes receive mannose-6-phosphate modifications that help direct them to lysosomes.

However, identifying an N-X-S/T motif does not prove that glycosylation occurs at that site. Experimental evidence is required to confirm actual glycan attachment. The motif alone also does not establish whether a mannose-6-phosphate tag is present.

### Question 5: What could happen in the cell if your enzyme did not work properly?

**Answer:**

If NAGLU is deficient or nonfunctional, heparan sulfate cannot be degraded normally and progressively accumulates inside lysosomes. This disrupts cellular function and can cause mucopolysaccharidosis type IIIB (MPS IIIB), a lysosomal storage disorder associated with progressive neurological impairment and developmental regression.

---

## 9. Evidence Screenshots

Upload screenshots demonstrating your individual work into the `evidence/` folder.

### Evidence 1: R Script
<img width="720" height="1280" alt="Screenshot_20261015-094302" src="https://github.com/user-attachments/assets/b7f01e30-b405-4d36-8883-fe282020b22b" />


### Evidence 2: Sequence Analysis

<img width="720" height="1280" alt="Screenshot_20261015-225120" src="https://github.com/user-attachments/assets/0019b46a-c12d-4c54-955a-a26d3f934476" />


### Evidence 3: Generated Figures

<img width="2400" height="990" alt="NAGLU_potential_N_glycosylation" src="https://github.com/user-attachments/assets/e90b9efe-6c98-44bb-a156-d0634c6eaaff" />
<img width="2400" height="1350" alt="NAGLU_amino_acid_composition" src="https://github.com/user-attachments/assets/2f9b382a-9959-49a6-810d-c718c391fe36" />


---

## 10. References

1. **NCBI Protein Database:** Human NAGLU reference protein record.  
   https://www.ncbi.nlm.nih.gov/protein/NP_000254.2

2. **NCBI Gene:** NAGLU — N-acetyl-alpha-glucosaminidase.  
   https://www.ncbi.nlm.nih.gov/gene/?term=NAGLU%5BGene%5D+AND+Homo+sapiens%5BOrganism%5D

3. **NCBI Bookshelf:** Mucopolysaccharidosis type III.  
   https://www.ncbi.nlm.nih.gov/books/?term=Mucopolysaccharidosis+Type+III

---

## 11. Conclusion

This bioinformatics activity examined the human NAGLU protein sequence, characterized its amino acid composition, and identified potential N-linked glycosylation motifs.

The figures summarize amino acid distribution and the positions of predicted motifs. These findings provide a basis for discussing protein characteristics, lysosomal enzyme function, and the biological importance of glycosylation.

The project demonstrates how R programming, sequence databases, data visualization, and GitHub documentation can be combined to support a reproducible molecular biology investigation.
