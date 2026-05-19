# Protein Language Model–Guided Variant Design of GAPDH

## Overview

This project explores the application of pretrained protein language models (ESM-2) for computational protein analysis and conservative enzyme variant generation.

The study focuses on the GAPDH enzyme across bacterial, yeast, and human homologs to investigate whether protein language models can capture evolutionary structure and generate biologically plausible sequence variants entirely in silico.

The project combines:
- Bioinformatics
- Protein sequence analysis
- Evolutionary analysis
- Representation learning
- AI-guided protein engineering

---

# Objectives

- Curate homologous GAPDH protein sequences across species
- Validate structural and evolutionary conservation
- Learn protein representations using pretrained protein language models
- Analyze embedding-based evolutionary relationships
- Generate conservative protein sequence variants computationally

---

# Dataset

The dataset consists of GAPDH homologous protein sequences from:

- *Escherichia coli* O157:H7
- *Escherichia coli* K12
- *Homo sapiens*
- *Saccharomyces cerevisiae*

These homologs were selected to ensure:
- Evolutionary diversity
- Conserved enzymatic function
- Biologically meaningful representation learning

---

# Methodology

## 1. Multiple Sequence Alignment (MSA)

Homologous sequences were aligned using **Clustal Omega** to verify conserved motifs and structural consistency across species.

### Key Steps
- FASTA sequence preparation
- Multiple sequence alignment
- Alignment visualization
- Pairwise evolutionary distance analysis

### Findings
- Strong conservation of catalytic motifs across homologs
- High-quality alignment with low gap percentages
- Clear evolutionary relationships between bacterial and eukaryotic proteins

---

## 2. Feature Extraction

Several sequence-based features were extracted for comparative analysis.

### Amino-Acid Composition
- Amino-acid frequency analysis
- Comparison of residue distributions across homologs

### Gap Statistics
- Alignment gap analysis
- Alignment quality validation

### Conservation Analysis
- Per-position conservation scoring
- Identification of highly conserved residues

### Findings
- Strong residue conservation across homologs
- Conserved catalytic and structural regions
- Similar amino-acid composition profiles among species

---

## 3. Protein Language Modeling (ESM-2)

The pretrained **ESM-2 transformer model** from Meta AI was used to learn protein representations.

### Workflow
- Sequence tokenization
- Embedding extraction
- Mean pooling of embeddings
- PCA-based visualization of embedding space

### Findings
- ESM-2 embeddings captured evolutionary relationships
- PCA clearly separated bacterial and eukaryotic sequences
- Biological structure emerged without task-specific training

---

## 4. AI-Guided Protein Variant Generation

A masked language modeling strategy was applied to generate conservative variants of human GAPDH.

### Workflow
- Masked a small region of the human GAPDH sequence
- Used ESM-2 masked language modeling predictions
- Predicted biologically plausible amino-acid substitutions
- Evaluated sequence similarity and conservation

### Findings
- Generated variants preserved structural context
- Predicted substitutions remained evolutionarily conservative
- Demonstrated feasibility of AI-guided protein design

---

# Technologies & Tools

## Bioinformatics
- Clustal Omega
- Biopython

## Machine Learning & AI
- ESM-2 Protein Language Model
- Transformers (Hugging Face)
- PyTorch
- PCA

## Data Science
- Python
- Pandas
- NumPy
- Scikit-learn

## Visualization
- Matplotlib

---

# Key Results

- Verified strong evolutionary conservation among GAPDH homologs
- Identified highly conserved catalytic regions
- Demonstrated that ESM-2 embeddings capture biological relationships
- Successfully generated conservative enzyme variants using masked language modeling
- Showed the potential of pretrained protein language models for computational protein engineering

---

# Biological Significance

This project demonstrates how modern AI models can learn biologically meaningful protein representations directly from sequence data.

The workflow provides a foundation for:
- AI-assisted protein engineering
- Functional variant generation
- Computational enzyme design
- Representation learning in molecular biology

---

# Future Directions

Potential future extensions include:

- Structural validation using AlphaFold
- Functional stability prediction
- Larger-scale protein family analysis
- Directed evolution simulation
- Protein fitness prediction
- Drug-target interaction modeling

---

# Repository Contents

- Protein sequence preprocessing
- Multiple sequence alignment workflows
- Evolutionary distance analysis
- Conservation scoring
- ESM-2 embedding extraction
- PCA visualization
- AI-guided variant generation

---

# Notebook

📓 **Google Colab / Notebook:**  
[https://github.com/raja016956/My_Projects/blob/main/Protein%20Language%20Model%E2%80%93Guided%20Variant%20Design%20of%20GAPDH.md
](https://colab.research.google.com/drive/1O0aT-27ApNn11J4Q0u8ypHosfemDnNfE?usp=sharing)
---

# Notes

- This project is intended for educational, research, and portfolio purposes
- All analyses were performed computationally
- Focus was placed on reproducibility, interpretability, and biological relevance

---

# Author

**Ghulam Fatima Memon**  
Computer Science Student | Computational Biology & AI Research Enthusiast

:contentReference[oaicite:0]{index=0}
