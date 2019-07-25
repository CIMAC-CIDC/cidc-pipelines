# cidc-pipelines
A repo for tracking the versions and composition of CIDC pipelines

## `v1.0.0` WES whole exome sequencing

### Components

| name     | description      | version | hash    | label                 |
|----------|------------------|---------|---------|-----------------------|
| cidc_wes | snakemake github |         | [`9b26a3d`](https://github.com/CIMAC-CIDC/cidc-wes/commit/9b26a3d063716eb176a40a23ef5213edd3a7a785) | commit from 6/12/2019 |
| 20190709_wesGCP_jason_update.txt | job submission protocol | | `ce44437cb14f38aadabc53838ed45fa3` | md5 checksum of text file |
| wes-ver1-83 | google compute image | 1-83 | `42WmSpB8rSM=` | label fingerprint of the image |
| reference-disk | contains WES reference | ??? | ??? | ??? |

### Tool catalog

| tool     | version      | notes   |
|----------|--------------|---------|
| bwa      | 0.7.17-r1188 |         |
| sentieon | 201808.05    |         |
| sambamba | 0.6.8        |         |
| sequenza | 2.1.9999b0    | conda yaml version?  |
| PyClone  | 0.13.1    | conda yaml version? |
| mosdepth |  0.2.3       |         |
| samtools | 1.9          |         |
| vcftools | 0.1.16       |         |
| vep      | 91.3         |         |
| pvacseq  | ???     |         |
| bedtools | v2.28.0      |         |
| Optitype | 1.3.1    | local conda environment? |
| snp-pileup | ???   |         |
| vcf2maf | ??? |  |
| bcftools | 1.9     |         |

### Reference catalog

|    | reference_key      | genome_version   | location                                                              | reference_version   | source   | date   |
|---:|:-------------------|:-----------------|:----------------------------------------------------------------------|:--------------------|:---------|:-------|
|  0 | bwa_index          | hg38             | ./ref_files/hg38/bwa_gdc/GRCh38.d1.vd1.fa                             |                     |          |        |
|  1 | genome_fasta       | hg38             | ./ref_files/hg38/bwa_gdc/GRCh38.d1.vd1.fa                             |                     |          |        |
|  2 | dbsnp              | hg38             | ./ref_files/hg38/snp/Homo_sapiens_assembly38.dbsnp138.vcf             |                     |          |        |
|  3 | Mills_indels       | hg38             | ./ref_files/hg38/snp/Mills_and_1000G_gold_standard.indels.hg38.vcf.gz |                     |          |        |
|  4 | G1000_indels       | hg38             | ./ref_files/hg38/snp/1000G_phase1.snps.high_confidence.hg38.vcf.gz    |                     |          |        |
|  5 | CDS_Bed_input      | hg38             | ./ref_files/hg38/gencode27.canonical.bed                              |                     |          |        |
|  6 | target_Bed_input   | hg38             | ./ref_files/hg38/target_beds/mocha.liftover.hg38.bed                  |                     |          |        |
|  7 | positions_bamtovcf | hg38             | ./ref_files/hg38/target_beds/pos_bamtovcf.bed                         |                     |          |        |
|  8 | positions_SNP92    | hg38             | ./ref_files/hg38/target_beds/pos_filtervcf.bed                        |                     |          |        |
|  9 | vep_data           | hg38             | ./ref_files/hg38/vep                                                  |                     |          |        |
| 10 | vep_plugins        | hg38             | ./ref_files/hg38/vep/VEP_plugins                                      |                     |          |        |
| 11 | vep_synonyms       | hg38             | ./ref_files/hg38/vep/homo_sapiens/91_GRCh38/chr_synonyms.txt          |                     |          |        |
| 12 | vep_custom_enst    | hg38             | ./ref_files/hg38/vep/myc_isoform_overrides_uniprot                    |                     |          |        |
| 13 | vep_fasta          | hg38             | ./ref_files/hg38/vep/hg38.canonical.fa                                |                     |          |        |
| 14 | vep_filter         | hg38             | ./ref_files/hg38/vep/ExAC_nonTCGA.r0.3.1.sites.vep.vcf.gz             |                     |          |        |
| 15 | vep_assembly       | hg38             | GRCh38                                                                |                     |          |        |
| 16 | pons               | hg38             | ./ref_files/hg38/pons/lung_TCGA_cnv_pad0                              |                     |          |        |
| 17 | pons_target        | hg38             | ./ref_files/hg38/pons/MDA_Broad_Miao.target.bed                       |                     |          |        |
| 18 | pons_haplotyper    | hg38             | ./ref_files/hg38/pons/TNhaplotyper_PoN.vcf.gz                         |                     |          |        |
| 19 | pons_tnsnv         | hg38             | ./ref_files/hg38/pons/TNsnv_PoN.vcf                                   |                     |          |        |
| 20 | facets_vcftar      | hg38             | ./ref_files/hg38/snp/00-common_all.vcf.gz                             |                     |          |        |
| 21 | gc_file            | hg38             | ./ref_files/hg38/clonality/hg38.gc50Base.txt.gz                       |                     |          |        |
| 22 | neoantigen_iedb    | hg38             | ./ref_files/hg38/iedb                                                 |                     |          |        |
| 23 | bwa_index          | hg19             | ./ref_files/hg19/bwa_indices/hg19/hg19.fa                             |                     |          |        |
| 24 | genome_fasta       | hg19             | ./path/to/hg19.fasta                                                  |                     |          |        |
