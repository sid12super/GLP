# Scalable Genomic Sequence Processing Pipeline

This project builds an end-to-end bioinformatics pipeline to classify DNA sequences (promoters vs. non-promoters) using a CNN, with data processing.

## Workflow Overview
1.  **Data Acquisition**: Promoter and non-promoter sequences are downloaded from public databases.
2.  **Model Development**: A CNN is built and trained in a Jupyter Notebook (`notebooks/`).
3.  **Workflow Automation**: The entire pipeline is automated using Nextflow.

## Data Acquisition

This repository contains the coordinate files (`promoters.bed`, `introns.bed`) needed to generate the datasets. The full human genome file and the final FASTA files are too large to be stored here and must be generated locally.

```bash
curl -O [http://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.2bit](http://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.2bit)

## Setup and Installation

**Important**: You must have Git LFS installed to clone this repository correctly.

```bash
# 1. Install Git LFS from [https://git-lfs.com](https://git-lfs.com)

# 2. Clone the repository
git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd your-repository-name

# 3. Download the large data files
git lfs pull
