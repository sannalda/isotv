# Prerequisites

Even though NanoIso is a snakemake pipeline and python based, many of the tools that implemented are available for linux based operating systems.

Most all software requirements are managed by the `conda` package manager and stored in a conda environment. However, few tools are not managed in conda and need to be installed seperately.

## Conda

Install conda as described at [https://conda.io/docs/install/quick.html](https://conda.io/docs/install/quick.html)
```
wget https://conda.io/docs/install/quick.html
bash Miniconda3-latest-Linux-x86_64.sh
```

## Tools

### IUPred2A

Install IUPred2A as described at [https://iupred2a.elte.hu/download_new](https://iupred2a.elte.hu/download_new)

### InterProScan 5

Install InterProScan as described at [https://github.com/ebi-pf-team/interproscan/wiki/HowToDownload](https://github.com/ebi-pf-team/interproscan/wiki/HowToDownload).

**Note: Involves additional requirements**.

### Porter5

Install Porter5 as described at [https://github.com/mircare/Porter5/](https://github.com/mircare/Porter5/).

**Note: Involves additional requirements**.

### Prosite Scan

Install Prosite Scan from [ftp://ftp.expasy.org/databases/prosite/ps_scan/](ftp://ftp.expasy.org/databases/prosite/ps_scan/).
```
wget ftp://ftp.expasy.org/databases/prosite/ps_scan/ps_scan_linux_x86_elf.tar.gz
wget ftp://ftp.expasy.org/databases/prosite/prosite.dat
```

### PLAAC

Install PLAAC from [https://github.com/whitehead/plaac](https://github.com/whitehead/plaac).

### Custom Scripts

For all custom scripts, below is a list of all required python packages and versions tested on:

* Bio
* pandas
* numpy
* subprocess
* argparse
* seaborn
* matplotlib
