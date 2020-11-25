# Source

Below outlines the steps to install NanoIso, which requires `conda` to be installed as described in [prerequisites](prerequisite.md).

1. Download the **nanoiso** pipeline into a folder named **nanoiso**:

        git clone https://github.molgen.mpg.de/annaldasula/nanoiso.git

2. Change the working directory into the new `nanoiso`:

        cd nanoiso

3. Install conda software dependencies with:

        conda env create --name nanoiso --file environment.yaml

4. Initialize the conda environment with:

        source activate nanoiso

5. To deactivate the conda environment after use:

        source deactivate
