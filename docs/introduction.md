# Introduction

NanoIso is snakemake pipeline used to perform individual isoform transcription and translation analysis from Oxford Nanopore Technologies (ONT) long read RNAseq datasets. It also has capabilities to process raw ONTseq data.

There are two major parts to the tool:

* Processing - Mapping and quanitfying full length ONT reads to a *de novo* transcriptome.
* Analysis - Individual isoform transcriptional and translational analysis.

The [Tools](tools.md) summarizes the external tools used for this pipeline.

The [Installation](prerequisite.md) discusses hows to install the pipeline as well as all the prerequisite tools needed.

The [Modules](overview.md) covers in depth of the various processes and tools within the pipeline.

The [Tutorial](general.md) describes about how to use the pipeline, as well snakemake basics and cluster computing capabilities.
