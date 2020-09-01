# Source

Below describes the steps to install NanoIso, which requires `conda` to be installed as described in [prerequisites](prerequisite.md).

1. Download the **isoform_analysis** pipeline into a folder named **isoform_analysis**:

        git clone https://github.molgen.mpg.de/annaldasula/isoform_analysis.git

2. Change the working directory into the new `isoform_analysis`:

        cd isoform_analysis

3. Install conda software dependencies with:

        conda env create --name isoform_analysis --file environment.yaml

4. Initialize the conda environment with:

        source activate isoform_analysis

5. To deactivate the conda environment after use:

        source deactivate
