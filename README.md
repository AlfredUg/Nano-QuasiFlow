# Nano-QuasiFlow

A version of QuasiFlow for analysing ONT-based HIV-1 drug resistance testing data via a graphical user interface. Currently, Nano-QuasiFlow is being updated to take as input FASTQ files, since ONT machines can be set up to basecall and de-barcode sequence data (this is higly recommended).

## Major tools/libraries

### Assembly-based analysis

* Checking data quality and quality trimming: `nanoq`.
* De-novo assembled: `flye`.
* Polishing draft genomes: `medaka` and `pilon`.
* Drug resistance interpretation: `Sierralocal`.

### Reference-based analysis

* Checking data quality and quality trimming: `nanoq`.
* Mapping reads onto the reference genome: `Minimap2`
* Variant calling and generating consensus sequences: `Quasitools`
* Drug resistance interpretation: `Sierralocal`.

### Graphical user interface

* Django
* Pandas
* NumPy
* Redis
* Celery

## Usage

* Upload Long read data in FASTQ format
* Specify input parameters and submit analysis
* Generate drug resistance report
* Download consensus sequences and amino acid variant file (AAVF).

 NOTE: At the moment, AAVF is only available for reference-base analysis.
 



