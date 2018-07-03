# LPA Server Pipeline 

This repository includes the used pipeline for the submitted article **XXX**. 

You can upload a **BAM file** and get **annotated low-level variants** in return. In the current version, indel detection and BAQ features are disabled.

Please check [this repository](https://github.com/seppinho/mutation-server) if you want to have a look at the actual source code. 

## Pipeline Steps

* Low-level Variant Detection
* Type-B Base Annotation
* Region Annotation
* Overall Statistics

## Run the LPA Pipeline

1) Install Cloudgene with the following commands

```
mkdir cloudgene
cd cloudgene
curl -s install.cloudgene.io | bash
```

2) Install the LPA workflow

```
./cloudgene gh seppinho/lpa-workflow
```

3a) Start the local web service and run
```
./cloudgene server
```
Open your web browser and enter http://localhost:8082. Use `admin` and `admin1978` to login.

3b) Run on the command line
```
./cloudgene run seppinho-lpa-workflow --input <bam-folder> --archive <fasta file>
```
## Test Data

* Download [BAM file](https://github.com/seppinho/mutation-server/raw/76e865ece25cf792d1534b0288b2c28bc1b3d013/test-data/dna/lpa-sample/bam/AK14_S12_L001_R1_001.gz_KIV2_6(-)5104bp.bam)

* Download [Reference](https://raw.githubusercontent.com/seppinho/mutation-server/76e865ece25cf792d1534b0288b2c28bc1b3d013/test-data/dna/lpa-sample/reference/kiv2_6.fasta)

## Download 1000G Paper Data
The script to download data from 1000 Genomes can be found [here](https://github.com/genepi/lpa-pipeline/tree/master/scripts).

## Contact
Plesae contact [Stefan Coassin](mailto:stefan.coassin@i-med.ac.at) and [Sebastian Schoenherr](mailto:sebastian.schoenherr@i-med.ac.at) in case of problems. 
