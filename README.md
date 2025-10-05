## Overview
This project was completed as part of the Computational Biology (CSE 6411) course at BUET in the October 2024 semester. NGS technologies produce short reads that are aligned to a reference genome for downstream analysis. In paired-end mode, some reads map to multiple loci, introducing ambiguity. Aligner-specific resolution schemes can yield incorrect mappings, degrading analysis quality. This project minimizes that issue with an MLP-based filter that predicts and discards incorrect alignments of multi-mapping reads reported by the aligner. The approach derives context-aware features—including read coverage, RNA-seq, and k-mers. Evaluated on [Bowtie2](https://bowtie-bio.sourceforge.net/index.shtml) alignments for two reference genomes ([*Escherichia coli*](https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi?id=511145) and [*Bacillus subtilis*](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE226559)), the trained classifier reduces the overall misalignment rate by substantial margins.

## Highlights
- Simulated reads using [ART Illumina](https://www.niehs.nih.gov/research/resources/software/biostatistics/art).
- Features constructed from extensive TF-IDF statistics over k-mers.
- Features constructed by utilizing correctly aligned read coverage.
- Binary classification task with an MLP.
- Misalignment error reduced by 48.98% (*E. coli*) and 63.16% (*B. subtilis*).

## Project Members
- Ananta Raha
- Anika Tasnim

## Instructor
- Dr. Atif Hasan Rahman
