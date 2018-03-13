# LPA Mutation-Server - Detection of low-level variants

This repository includes the workflow for detection of low-level variants.

## Run LPA Mutation-Server

1) Install Cloudgene with the following commands

```
mkdir cloudgene
cd cloudgene
curl -s install.cloudgene.io | bash
```

2) Install the LPA workflow

```
./cloudgene gh seppinho/lpa-workflow@latest
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


