# RNAseq Alignment and Mpileup Tutorial

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/biermanr/RNAseq_alignment_and_mpileup_codespaces_tutorial)

An interactive tutorial environment for learning RNA-seq alignment using STAR and variant calling with samtools/bcftools. Launch this repository in GitHub Codespaces to get started instantly with a fully configured bioinformatics environment.


## Quick Start

### Launch in Codespaces

1. Click the "Open in GitHub Codespaces" badge above
2. Wait 2-3 minutes for the environment to build (first time only)
3. The terminal will open with the `(rnaseq)` conda environment activated
4. Start analyzing!

### Verify Installation

Once your Codespace is ready, verify the tools are installed:

```bash
# Check STAR version
star --version

# Check samtools version
samtools --version

# Check bcftools version
bcftools --version

# Check Python environment
python --version
python -c "import pandas, matplotlib; print('Python packages OK')"
```
