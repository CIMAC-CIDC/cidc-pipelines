# cidc-pipelines
A repo for tracking the versions and composition of CIDC pipelines

## `v1.0.0` WES whole exome sequencing

### Components

| name     | description      | version | hash    | notes                 |
|----------|------------------|---------|---------|-----------------------|
| cidc_wes | snakemake github |         | [`9b26a3d`](https://github.com/CIMAC-CIDC/cidc-wes/commit/9b26a3d063716eb176a40a23ef5213edd3a7a785) | commit from 6/12/2019 |
| 20190709_wesGCP_jason_update.txt | job submission protocol | | `ce44437cb14f38aadabc53838ed45fa3` | md5 checksum of text file |
| wes-ver1-83 | google compute image | 1-83 | `42WmSpB8rSM=` | label fingerprint of the image |
| reference-disk | contains WES reference | ??? | ??? | ??? |

### Environments

| name     | type |    version   | notes   |
|----------|------|--------------|---------|
| pyclone  | conda | ???         |         |
| optitype | conda | ???         | locally built |


### Tools

| tool     | version      | environment | notes   |
|----------|--------------|-------------|---------|
| bwa      | 0.7.17-r1188 |         | |
| sentieon | 201808.05    |         | |
| sambamba | 0.6.8        |         | |
| sequenza | 2.1.9999b0    | pyclone  | |
| PyClone  | 0.13.1    | pyclone | |
| mosdepth |  0.2.3       |         | |
| samtools | 1.9          |         | |
| vcftools | 0.1.16       |         | |
| vep      | 91.3         |         | |
| pvacseq  | ???     |         | |
| bedtools | v2.28.0      |         | |
| Optitype | 1.3.1    | optitype | |
| snp-pileup | ???   |         | |
| vcf2maf | ??? |  | |
| bcftools | 1.9     |         | |

### References

| reference_key      | location                                                              | reference_version   | source   | date   |
|:-------------------|:-----------------|:----------------------------------------------------------------------|:--------------------|:---------|:-------|
| bwa_index_hg38          | ./ref_files/hg38/bwa_gdc/GRCh38.d1.vd1.fa                             |                     |          |        |
| genome_fasta_hg38       | ./ref_files/hg38/bwa_gdc/GRCh38.d1.vd1.fa                             |                     |          |        |
| dbsnp              | ./ref_files/hg38/snp/Homo_sapiens_assembly38.dbsnp138.vcf             |                     |          |        |
| Mills_indels       | ./ref_files/hg38/snp/Mills_and_1000G_gold_standard.indels.hg38.vcf.gz |                     |          |        |
| G1000_indels       | ./ref_files/hg38/snp/1000G_phase1.snps.high_confidence.hg38.vcf.gz    |                     |          |        |
| CDS_Bed_input      | ./ref_files/hg38/gencode27.canonical.bed                              |                     |          |        |
| target_Bed_input   | ./ref_files/hg38/target_beds/mocha.liftover.hg38.bed                  |                     |          |        |
| positions_bamtovcf | ./ref_files/hg38/target_beds/pos_bamtovcf.bed                         |                     |          |        |
| positions_SNP92    | ./ref_files/hg38/target_beds/pos_filtervcf.bed                        |                     |          |        |
| vep_data           | ./ref_files/hg38/vep                                                  |                     |          |        |
| vep_plugins        | ./ref_files/hg38/vep/VEP_plugins                                      |                     |          |        |
| vep_synonyms       | ./ref_files/hg38/vep/homo_sapiens/91_GRCh38/chr_synonyms.txt          |                     |          |        |
| vep_custom_enst    | ./ref_files/hg38/vep/myc_isoform_overrides_uniprot                    |                     |          |        |
| vep_fasta          | ./ref_files/hg38/vep/hg38.canonical.fa                                |                     |          |        |
| vep_filter         | ./ref_files/hg38/vep/ExAC_nonTCGA.r0.3.1.sites.vep.vcf.gz             |                     |          |        |
| pons               | ./ref_files/hg38/pons/lung_TCGA_cnv_pad0                              |                     |          |        |
| pons_target        | ./ref_files/hg38/pons/MDA_Broad_Miao.target.bed                       |                     |          |        |
| pons_haplotyper    | ./ref_files/hg38/pons/TNhaplotyper_PoN.vcf.gz                         |                     |          |        |
| pons_tnsnv         | ./ref_files/hg38/pons/TNsnv_PoN.vcf                                   |                     |          |        |
| facets_vcftar      | ./ref_files/hg38/snp/00-common_all.vcf.gz                             |                     |          |        |
| gc_file            | ./ref_files/hg38/clonality/hg38.gc50Base.txt.gz                       |                     |          |        |
| neoantigen_iedb    | ./ref_files/hg38/iedb                                                 |                     |          |        |
| bwa_index_hg19          | ./ref_files/hg19/bwa_indices/hg19/hg19.fa                             |                     |          |        |
| genome_fasta_hg19       | ./path/to/hg19.fasta                                                  |                     |          |        |
