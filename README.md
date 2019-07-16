# cidc-pipelines
A repo for tracking the versions and composition of CIDC pipelines

## `v1.0.0` WES whole exome sequencing

### Components

| name     | description      | version | hash    | label                 |
|----------|------------------|---------|---------|-----------------------|
| cidc_wes | snakemake github |         | [`9b26a3d`](https://github.com/CIMAC-CIDC/cidc-wes/commit/9b26a3d063716eb176a40a23ef5213edd3a7a785) | commit from 6/12/2019 |
| 20190709_wesGCP_jason_update.txt | job submission protocol | | `ce44437cb14f38aadabc53838ed45fa3` | md5 checksum of text file |
| wes-ver1-83 | google compute image | 1-83 | `42WmSpB8rSM=` | label fingerprint of the image |

### Tool catalog

| tool     | version      | notes   |
|----------|--------------|---------|
| bwa      | 0.7.17-r1188 |         |
| sentieon | 201808.05    |         |
| sambamba | 0.6.8        |         |
| sequenza | 2.1.9999b0⚠    | conda yaml doesn't specify version  |
| PyClone  | 0.13.1⚠    | conda yaml doesn't specify version |
| mosdepth |  0.2.3       |         |
| samtools | 1.9          |         |
| vcftools | 0.1.16       |         |
| vep      | 91.3         |         |
| pvacseq  | ???     |         |
| bedtools | v2.28.0      |         |
| Optitype | 1.3.1⚠    | conda yaml doesn't specify version; activates a local environment |
| snp-pileup | ???   |         |
| vcf2maf | ??? |  |
| bcftools | 1.9     |         |
