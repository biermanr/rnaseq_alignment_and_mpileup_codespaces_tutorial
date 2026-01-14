# Codespace to Facilitate RNAseq Alignment and Mpileup Tutorial

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/biermanr/RNAseq_alignment_and_mpileup_codespaces_tutorial)

An interactive tutorial environment for learning RNA-seq alignment using STAR
and variant calling with samtools/bcftools. Launch this repository in GitHub
Codespaces to get started with some common bioinformatics tools without having
to install them yourself.

This repo is just a proof of concept of how to setup codespaces with a custom
github container registry.


## Quick Start

### Launch in Codespaces

1. Click the "Open in GitHub Codespaces" badge above
2. Wait ~5 minutes for the environment to build (first time only)
3. The terminal will open with the `(rnaseq)` conda environment activated
4. Start analyzing!

### Verify Installation

Once your Codespace is ready, verify the tools are installed:

```bash
# Check STAR version
STAR --version

# Check samtools version
samtools --help

# Check bcftools version
bcftools --help
```

### Download an example .vcf.gz and inspect it

```bash
# Download a vcf.gz file
wget https://tigress-web.princeton.edu/AKEY/ibdmix_tests/cell_data/mod_chr20.vcf.gz

# Look at the first 10 header lines of the file
bcftools view mod_chr20.vcf.gz | head
```

## Notes

### GitHub codespaces info

* As of the time of writing this, all github users get 120 CPU hours per month free.
* When a user launches a new codespace, their quota gets used, not the quota of
  the owner of the repo that the codespaces was launched from.
* This could be a good setup for a class where students need to have a set of
  software tools installed to follow along with class or do an exercise themselves.
* Codespaces lets the instructor setup the environment that all students can use.

### Current limitations and future todos

* It takes ~5 minutes for the codespace to fully launch and load.
* The Docker image is >1G in size and can surely be shrunk. Maybe by
  installing the tool from source instead of conda.
* Expected utilities are missing in the environment such as vi and less.
  Could be addressed by building from an ubuntu base image.



