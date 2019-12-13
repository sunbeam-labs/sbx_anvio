# Anvio: an analysis and sualization platform for 'omics data

In this extension, we show how easy it is to add downstream analysis to sunbeam pipeline as an extension.

## Installation

To install:

    sunbeam extend https://github.com/sunbeam-labs/sbx_anvio

Legacy instructions for older Sunbeam versions are below.

## Usage

This adds a new rule, `all_anvio_scg`. Specify this as your target to use Anvio to look at the distributuion of bacterial single-copy genes in this contigs database, and roughly predict the number of genomes in it:

    sunbeam run --configfile sunbeam_config.yml --use-conda all_anvio_scg 
 
The `--use-conda` flag is required to let Snakemake know that you want to use the `sbx_anvio` conda environment.

------------

## Installation (legacy instructions for Sunbeam version <3.0)

With your sunbeam conda environment activated,

1. Clone into your Sunbeam directory:
    ```shell
    git clone https://github.com/sunbeam-labs/sbx_anvio sunbeam/extensions/sbx_anvio
    ```

