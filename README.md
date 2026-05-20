# Algorithmic-Foundations-Of-Computational-Genomics
<div align="center">

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Scientific_Computing-orange?style=for-the-badge&logo=numpy)
![Algorithms](https://img.shields.io/badge/Algorithms-Computational_Genomics-darkred?style=for-the-badge)
![Motif Search](https://img.shields.io/badge/Motif-Discovery-purple?style=for-the-badge)
![Genome Analysis](https://img.shields.io/badge/Genome-Analytics-darkgreen?style=for-the-badge)
![Status](https://img.shields.io/badge/Build-Stable-success?style=for-the-badge)

</div>

---

<div align="center">

## DNA Sequence Analysis • Motif Discovery • Probabilistic Genomics

</div>

# Algorithmic Foundations of Computational Genomics

A structured implementation of classical bioinformatics algorithms for DNA sequence analysis, motif discovery, genomic signal detection, and probabilistic motif optimization using Python.

This repository progressively builds computational genomics concepts from fundamental sequence processing to advanced stochastic motif search algorithms commonly used in modern bioinformatics pipelines.

---

# Repository Overview

This project was developed as part of an Advanced Computational Biology assignment focused on algorithmic bioinformatics and genome-scale sequence analysis.

The repository demonstrates:

* Exact and approximate DNA pattern matching
* k-mer frequency analysis
* Genome skew analysis
* Replication origin detection
* Hamming distance computation
* Motif matrix construction
* Consensus sequence extraction
* Greedy motif search
* Pseudocount stabilization
* Randomized motif optimization

The implementations are intentionally written from scratch without relying on high-level BioPython abstractions in order to understand the underlying computational logic of genomic algorithms.

---

# Repository Structure

```text
algorithmic-foundations-of-computational-genomics/
│
├── sequence-analysis/
│   ├── Phase1.1_PatternCount.py
│   ├── Phase1.2_FrequencyMap.py
│   ├── Phase1.3_MostFrequentKmers.py
│   ├── Phase1.4_ComplementaryDNA.py
│   ├── Phase1.5_PatternMatching.py
│   └── README_Module1.md
│
├── genome-skew-analysis/
│   ├── Phase2.1_SymbolArray.py
│   ├── Phase2.1.2_FasterSymbolArray.py
│   ├── Phase2.2_SkewArray.py
│   ├── Phase2.3_MinimumSkew.py
│   ├── Phase2.4_HammingDistance.py
│   ├── Phase2.5_ApproximatePatternMatching.py
│   └── README_Module2.md
│
├── motif-discovery/
│   ├── Phase3.0_NumPyFoundations.py
│   ├── Phase3.1_CountNucleotideMotif.py
│   ├── Phase3.2_ProfileMatrix.py
│   ├── Phase3.3_ConsensusSequence.py
│   ├── Phase3.4_ScoreDNAMotif.py
│   ├── Phase3.5_ProfileMostProbableKmer.py
│   ├── Phase3.6_GreedyMotifSearch.py
│   ├── Extended_PatternWithMismatch.py
│   └── README_Module3.md
│
├── probabilistic-motif-search/
│   ├── Phase4.1_GreedyMotifSearchWithPseudocounts.py
│   ├── Phase4.2_RandomizedMotifSearch.py
│   └── README_Module4.md
│
├── requirements.txt
└── README.md
```

---

# Computational Workflow

```text
DNA Sequence Processing
        ↓
Pattern Detection
        ↓
k-mer Frequency Analysis
        ↓
Genome Skew Analysis
        ↓
Mutation Distance Calculation
        ↓
Motif Matrix Construction
        ↓
Consensus & Profile Generation
        ↓
Greedy Motif Discovery
        ↓
Probabilistic Optimization
        ↓
Randomized Motif Search
```

---

# Algorithm Summary

| Phase | Algorithm                    | Objective                       | Biological Relevance       | Complexity |
| ----- | ---------------------------- | ------------------------------- | -------------------------- | ---------- |
| 1.1   | Pattern Count                | Count motif occurrences         | Motif enrichment           | O(nm)      |
| 1.2   | Frequency Map                | Generate k-mer frequencies      | Sequence composition       | O(nk)      |
| 1.3   | Frequent k-mers              | Detect dominant motifs          | Regulatory motifs          | O(nk)      |
| 1.4   | DNA Complement               | Generate complementary strand   | DNA replication            | O(n)       |
| 1.5   | Pattern Matching             | Exact motif localization        | Binding site mapping       | O(nm)      |
| 2.1   | Symbol Array                 | Sliding nucleotide analysis     | Circular genomes           | O(n²)      |
| 2.1.2 | Faster Symbol Array          | Optimized window computation    | Genome efficiency          | O(n)       |
| 2.2   | Skew Array                   | Compute G-C imbalance           | Replication direction      | O(n)       |
| 2.3   | Minimum Skew                 | Detect oriC candidates          | Replication origin         | O(n)       |
| 2.4   | Hamming Distance             | Mutation quantification         | Evolutionary divergence    | O(n)       |
| 2.5   | Approximate Matching         | Mutation-tolerant motif search  | Functional motif discovery | O(nm)      |
| 3.1   | Nucleotide Count Matrix      | Motif conservation analysis     | PWM generation             | O(tk)      |
| 3.2   | Profile Matrix               | Probability matrix generation   | Statistical motif modeling | O(tk)      |
| 3.3   | Consensus Sequence           | Representative motif extraction | Conserved regions          | O(tk)      |
| 3.4   | Motif Scoring                | Measure motif divergence        | Conservation analysis      | O(tk)      |
| 3.5   | Profile-Most Probable k-mer  | Probabilistic motif matching    | Motif prediction           | O(nk)      |
| 3.6   | Greedy Motif Search          | Deterministic motif discovery   | Regulatory site detection  | O(tn²k)    |
| 4.1   | Greedy Search + Pseudocounts | Stabilized motif discovery      | Noise handling             | O(tn²k)    |
| 4.2   | Randomized Motif Search      | Stochastic optimization         | Global motif discovery     | Iterative  |

---

# Core Concepts Implemented

## Fundamental Sequence Algorithms

* Sliding window pattern matching
* Exact motif localization
* k-mer decomposition
* DNA complement generation

## Genome Signal Analysis

* Circular genome handling
* Genome skew computation
* Replication origin prediction
* Approximate sequence matching

## Motif Discovery Framework

* Motif matrices
* Position frequency matrices
* Position probability matrices
* Consensus sequence generation
* Greedy motif optimization

## Probabilistic Optimization

* Laplace pseudocount correction
* Zero-probability prevention
* Randomized search heuristics
* Local minima avoidance

---

# Biological Applications

These algorithms are foundational in:

* Regulatory motif discovery
* Transcription factor binding analysis
* Comparative genomics
* Mutation analysis
* Genome annotation
* Replication origin prediction
* Evolutionary sequence comparison
* Computational molecular biology

---

# Technologies Used

| Technology                | Purpose                 |
| ------------------------- | ----------------------- |
| Python                    | Core implementation     |
| NumPy                     | Matrix manipulation     |
| Dictionaries              | Frequency mapping       |
| Sliding Window Algorithms | Sequence traversal      |
| Probability Models        | Motif scoring           |
| Randomization             | Stochastic optimization |

---

# Installation

Clone the repository:

```bash
git clone https://github.com/your-username/algorithmic-foundations-of-computational-genomics.git
```

Move into the repository:

```bash
cd algorithmic-foundations-of-computational-genomics
```

Install dependencies:

```bash
pip install numpy
```

---

# Running the Algorithms

Example:

```bash
python sequence-analysis/Phase1.1_PatternCount.py
```

or

```bash
python probabilistic-motif-search/Phase4.2_RandomizedMotifSearch.py
```

---

# Example Outputs

## Pattern Matching

```python
Pattern: CGCG
Positions: [0, 26, 30, 42]
```

## Minimum Skew Detection

```python
Minimum Skew Positions: [12]
```

## Greedy Motif Search

```python
Best Motifs:
['CAG', 'CAG', 'CAA', 'CAA', 'CAA']
```

## Randomized Motif Search

```python
Optimized Motifs:
['TCTCGGGG', 'CCAAGGTG', 'TACAGGCG', 'TTCAGGTG', 'TCCACGTG']
```

---

# Scientific Significance

This repository demonstrates how classical computational biology algorithms are constructed from first principles.

Rather than relying on high-level bioinformatics libraries, the implementations explicitly demonstrate:

* algorithmic genome traversal
* motif scoring logic
* probability-based sequence modeling
* deterministic and stochastic optimization techniques

The progression mirrors foundational computational genomics curricula and motif discovery frameworks used in modern bioinformatics education.

---
