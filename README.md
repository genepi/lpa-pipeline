# LPA Server Pipeline 

## General
This repository includes the pipeline used for the submitted article "used in paper "Chasing variants in the LPA KIV-2 repeat: An evaluated sequencing protocol, a free analysis pipeline and a first map in human samples"". 

You can upload a BAM file and get annotated variants in return. In this version. indel detection and baq are disabled.

Please check [this repository](https://github.com/seppinho/mutation-server/releases) if you want to have a look at the actual source code. 

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

## Paper Data
