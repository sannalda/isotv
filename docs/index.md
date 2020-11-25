# Introduction

NanoIso is snakemake pipeline used to perform individual isoform transcription and translation analysis from RNAseq data, especially from Oxford Nanopore Technologies (ONT) long read datasets. It also has capabilities to process raw reads from ONTseq data.

There are two major components to this tool:

* Processing - Mapping and quantifying full length ONT reads to a *de novo* transcriptome.
* Analysis - Individual isoform transcriptional and functional analysis.

NanoIso is specifically geared towards processing and analyzing data across time (e.g. looking for isoform changes across two or more time points). However, it can be extrapolated to analyzing isoforms across conditions. 

The [Tools](tools.md) summarizes the external tools used for this pipeline.

The [Installation](prerequisite.md) discusses hows to install the pipeline as well as all the prerequisite tools needed.

The [Modules](overview.md) covers in depth of the various processes and tools within the pipeline.

The [Tutorial](general.md) describes about how to use the pipeline, as well snakemake basics and cluster computing capabilities.
