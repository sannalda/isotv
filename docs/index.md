# Introduction

NanoIso is snakemake pipeline used to perform individual isoform transcription and translation analysis from Oxford Nanopore Technologies (ONT) long read RNAseq datasets. It also has capabilities to process raw ONTseq data.

There are two major parts to the tool:

* Processing - Mapping and quanitfying full length ONT reads to a *de novo* transcriptome.
* Analysis - Individual isoform transcriptional and functional analysis.

The [Tools](tools.md) summarizes the external tools used for this pipeline.

The [Installation](prerequisite.md) discusses the installation procedure and the required prerequisite tools.

The [Modules](overview.md) covers in depth of the various processes and tools used in the pipeline.

The [Tutorial](general.md) describes about how to use the pipeline, as well some snakemake basics and cluster computing capabilities.
