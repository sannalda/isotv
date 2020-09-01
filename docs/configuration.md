# Configuration

NanoIso has two configuration files - `environment.yaml`, which handles the necessary packages and dependences for the [conda environment](source.md), and `config.yaml`, which covers the general and specific pipeline parameters and paths.

## Pipeline Configuration

The pipeline configuration is split into three parts: general, processing and analysis. There are file paths for files and tools that need to be set before running. Specific module specific configuration is discussed in [Modules](overview.md).

Below configuration ids can be configured in the **config.yaml** file or explicitly specified in the command line.

### General

`gencode_gtf` - Reference gencode gtf file path.

`human_genome` - Reference human genome assembly file path.

### Processing

`minimap2` - Minimap2 file path ((((NEEED TO BE DOUBLE CHECKED !!!!))))

`samples` - Sample name with `.fastq` extension. For reference, the notation `dayX_Y:Z` corresponds of the *X* day and *Y* replicate from the fastq file *Z* of the experiment. However, this is only advised and not necessary.

### Analysis

`nanopore_gtf` - Path to gtf transcript file that was mapped to the *de novo* transcriptome. Required if not using NanoIso processing.

`polished_reads` - Path to reads with polished sequences. Required if not using NanoIso processing.

`prosite_dat` - Path to `prosite.dat`.

`java` - Path to java. Not necessary unless Java is not at least version 11.

`iupred2a` - Path to IUPred2A download.

`porter` - Path to Porter5 download. (((DONT KNOW IF THIS IS NECESSARY)))

`prosite_scan` - Path to `ps_scan.pl`.

`plaac` - Path to `plaac.jar`.
