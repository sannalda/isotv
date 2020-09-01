# Preprocessing

The preprocessing step involves finding full length transcripts from basecalled raw reads.

[Filtlong](https://github.com/rrwick/Filtlong/) is used to filter reads by their quality, while [Pychopper](https://github.com/nanoporetech/pychopper) is used to find full length transcripts.

## Usage

Input - `RawData/X.fastq`

Output - `Results/Pychopper/X.pychop.fastq`

`snakemake`

## Configuration

Below are changes that can be configured in the **config.yaml** file or explicitly specified in the command line.

### Filtlong

`min_mean_q: 5` - Minimum read quality to keep.

### Pychopper

`porechop_heu_stringency: 0.25` - Stringency of porechop heuristic.

## Output Folder Structure

```
| -- FilteredData/
    | -- X.fastq
    ...
| -- Results/
    | -- Pychopper/
        | -- X.pychop.fastq
        ...
```
