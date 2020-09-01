# Prerequisites

Even though NanoIso is a snakemake pipeline and python based, many of the tools that implemented are available only for linux based operating systems.

Most all software requirements are managed by the `conda` package manager and stored in a conda environment. However, few tools are not managed in conda and need to be installed seperately.

## Conda

Install `conda` as described at [https://conda.io/docs/install/quick.html](https://docs.conda.io/en/latest/miniconda.html)
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

**Note:** Newer versions of `conda` may have have package conflicts errors. If this is the case, try downgrading the conda version to `4.6.14`.
```
conda install conda=4.6.14
```

## Tools

### IUPred2A

Install IUPred2A as described at [https://iupred2a.elte.hu/download_new](https://iupred2a.elte.hu/download_new)

### InterProScan 5

Install InterProScan as described at [https://github.com/ebi-pf-team/interproscan/wiki/HowToDownload](https://github.com/ebi-pf-team/interproscan/wiki/HowToDownload).

```
mkdir my_interproscan
cd my_interproscan
wget ftp://ftp.ebi.ac.uk/pub/software/unix/iprscan/5/5.46-81.0/interproscan-5.46-81.0-64-bit.tar.gz
wget ftp://ftp.ebi.ac.uk/pub/software/unix/iprscan/5/5.46-81.0/interproscan-5.46-81.0-64-bit.tar.gz.md5

md5sum -c interproscan-5.46-81.0-64-bit.tar.gz.md5

tar -pxzf interproscan-5.46-81.0-64-bit.tar.gz
```

**Note: Involves additional requirements (e.g. PANTHER)**.

```
cd data
wget ftp://ftp.ebi.ac.uk/pub/software/unix/iprscan/5/data/panther-data-14.1.tar.gz
wget ftp://ftp.ebi.ac.uk/pub/software/unix/iprscan/5/data/panther-data-14.1.tar.gz.md5

md5sum -c panther-data-14.1.tar.gz.md5

tar -pxvzf panther-data-14.1.tar.gz
```

### Porter5

Install Porter5 as described at [https://github.com/mircare/Porter5/](https://github.com/mircare/Porter5/).

```
git clone https://github.com/mircare/Porter5/ --depth 1 && rm -rf Porter5/.git
```

**Note: Involves additional requirements (e.g. HHblits, UniRef90). HHblits should already be part of** `environment.yaml`**.**
```
wget http://wwwuser.gwdg.de/~compbiol/data/hhsuite/databases/hhsuite_dbs/old-releases/uniprot20_2016_02.tgz
tar zxvf uniprot20_2016_02.tgz
```

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
