## Popgen

This is a cutdown copy of the code at https://github.com/tomwhite/shiny-train/tree/sgkit/notebooks/gwss

### Create environment

```shell
mamba env create --file environment-pinned.yml
conda activate sgkit-publication-popgen
```

### Download data

```shell
./download-ag1000g-data.sh
```

### Run notebooks

```shell
jupyter notebook
```

Then run the following notebooks:
* _sgkit_import_haplotypes.ipynb_
* _sgkit_h12.ipynb_

### Upate/save environment

The pinned environment file was created with

```shell
conda env export -v --override-channels --channel conda-forge --channel defaults --channel=conda-forge/label/broken --name=sgkit-publication-popgen > environment-pinned.yml
```