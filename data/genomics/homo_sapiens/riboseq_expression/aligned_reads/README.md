# Aligned reads for testing with Riboseq modules

Files in this directory are the result of fastq files being trimmed for adapters via Trimgalore, ribosomal rna being removed with sortmerna, and alignment being made to human genome chromosome 20, followed by coordinate sorting and indexing. This was done with the nf-core/riboseq workflow with components derived from nf-core/rnaseq. Input reads were down-sampled in a directed manner using [this script](https://github.com/nf-core/test-datasets/blob/riboseq/testdata/make_test_data.sh), essentially selecting those reads known to map to chromosome 20.