# Conda pack issue

```
$ conda --version
conda 4.10.1
```

First of all, install conda-pack, see https://conda.github.io/conda-pack/.

To reproduce the env, create the conda env. Note it will also `pip install` dependencies in the requirements.txt

```
conda env create -f environment.ml.yaml
```

Anyway, once the conda `featflow-ml-env` is created, activate, then conda pack the env into a zip.

```
conda pack -o featflow-ml-env.zip
```

Also, conda pack the env into the default tar.gz format.

```
conda pack
```

As a supplement, I run `tree` command on the conda env directory, the result can be found in `tree.txt`.

