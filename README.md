# Anvio: an analysis and sualization platform for 'omics data'

In this extension, we show how easy it is to add downstream analysis to sunbeam pipeline as an extension.

## Installation:

With your sunbeam conda environment activated,

1. Clone into your Sunbeam directory:
    ```shell
    git clone https://github.com/sunbeam-labs/sbx_anvio sunbeam/extensions/sbx_anvio
    ```

2. Install the requirements:
    ```shell
    conda install --file sunbeam/extensions/sbx_anvio/requirements.txt
    ```

## Usage

This adds a new rule, `all_anvio_scg`. Specify this as your target to use Anvio to look at the distributuion of bacterial single-copy genes in this contigs database, and roughly predict the number of genomes in it.
 

