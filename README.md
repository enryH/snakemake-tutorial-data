# Snakemake tutorial with data

This repository hosts the final code and data needed for the [Snakemake tutorial](https://snakemake.readthedocs.io/en/stable/tutorial/tutorial.html).


Run in VScode using binder:  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/enryH/snakemake-tutorial/snakemake-tutorial?urlpath=vscode/?folder=/home/jovyan/snakemake-tutorial-data)

## To try

```bash
snakemake --help
snakemake -n # dry-run
snakemake --cores 1 # execute locally
snakemake --report report.html # after running snakemake, create a report
snakemake --dag | dot -Tpng > dag.png
snakemake -n --forceall
snakemake --forceall --use-conda # --conda-frontend mamba
```




If you want to revert changes with the possibility to replay them, use 
[`git stash`](https://git-scm.com/book/en/v2/Git-Tools-Stashing-and-Cleaning)
```bash
git stash --all
```

## CHANGELOG

- png instead of svg histogram (easier to view)
